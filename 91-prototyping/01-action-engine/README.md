# Action Engine Prototyping

## 1. Proje Tanımı

Bu proje Account Planning projesinin Action Management modülünün Action Engine feature'ının prototiplemesi için kullanılacaktır.
Geliştirme ekibi ile align olabilmek adına hem ekranlar hem veritabanı geliştirlemeleri online olarak görüntülenebilecek olup "accountplanning.ai" domain üzerinden host edilecektir. Önyüzde hem fiili işleyiş hem de arka plandaki veri yapısını görsel olarak izleyebilmek mümkün olmalıdır.

## 2. Tasarım Gereksinimleri

Kullanıcı ekranı açtığında aksiyon yaşam döngüsünü farklı kullanıcılar açısından switch edebilmeli, her kullanıcının gözünden ilgili adım nasıl görünüyor görebilmeli. Aynı zamanda ilgili ekranda kullanılan veri yapısı, bağlantıları, ekrandaki seçili değişkenler, vb developer'ın ihtiyacı olan tüm veriler önyüz ile eşlenik şekilde görülebilmeli. Ekrandaki her bileşen seçildiğinde veri yapısının o bileşeni karşılık gelen kısımları vurgulanabilmeli, ekrandan bir bileşen seçtiğimde veri yapısında neler değişiyor bunu görebilmeliyim.

Bu uygulamanın veritabanı postgresql olacak, buna karşılık veri yapısı sembolik olarak DWH ve OLTP olarak iki katmandan oluşacak. Aşağıda tanımlanan fonksiyonel gereksinimler doğrultusunda hangi tablonun hangi katmanda olması gerektiğini tablo isimlendirmesinde prefix olarak göster. 

## 3. Fonksiyonel Gereksinimler

### 3.1 Genel Tanım

Proje özünde bir task management uygulamasıdır. Akış şu şekildedir: her task bir sinyalden türetilir, aksiyona dönüşür, aksiyonlar skorlanır/önceliklendirili, A/B test ayrımı ile işaretlenir, gerçekleşenleri sistemsel olarak takip edilir, ürettikler etki monitor edilir.

### 3.2 Sinyal Yönetimi

Bir sinyal tanım tablosunda 4 farklı kaynaktan gelen sinyallere ait tanımlar yer alır. Bu 4 kaynak sırasıyla; Analitik Modeller, Kural bazlı SQL'ler, Excel liste uploadları, ve form üzerinden manuel sinyal girişi. Teknik gereksinimler sebebiyle bu alan sadece tanım tablosu olarak çalışacak olup aksiyon tanımlarında referans olarak belirtilecek. Sinyal tanım tablosunda temel olarak sinyal adı, sinyal kodu, sinyal tipi (model, kural, dosya, manuel), oluşma sıklığı, oluşma tarihi, validity_period, last_updated, sorumlu user id, contact user email, vb.) kolonlarının olması beklenmektedir. 

Her sinyal belirlitilen tarihlerde oluşur, örneğin xyz analitik modeli her ayın 3'ünde çalışır. Sinyal tanım tablosunda bu bilgi oluşma sıklığı: aylık, oluşma zamanı: ayın 3'ü olarak kaydedilir. Bir de geçerlilik süresi mevcuttur; aksi belirtilmezse sinyal üretim tarihinden itibaren 1 aydır. Her sinyal için farklı frekans ve geçerlilik süresi olabilir.

### 3.3 Aksiyon Yönetimi

Aksiyon sorumlusu sinyal verilerinden türetilen aksiyon SQL'lerini tanımlamakla sorumludur. SQL'ler belirli bir formatta veri üretmelidir. Bir doğrulama mekanizması bu SQL'lerin doğrulamasını, çalışma süresini ölçerek (örnek: max 30 sn, 2mio rows max) geçerliliğini valide eder. Tanımlanan SQL'ler periyodik olarak çalıştırılarak aksiyon havuzunu besler.

Aksiyon sorumlusu aksiyon oluştururken SQL'e ilave olarak aksiyonun adı, kısa açıklaması (tooltip için), tanımlama tarihi, geçerlilik süresi, sorumlu user id, contact user email, skor bileşenleri (kpi performans etkisi, müşteri memnuniyet etkisi, karlılık etkisi, strateji uyumluluk etkisi) verilerini de tanımlar. 

Aksiyonlar bağlı oldukları sinyal'in oluşma tarihinde otomatik çalıştırılırlar. Bir kontrol mekanizması (sonraki mvp) sinyalin oluşup oluşmadığını kontrol eder, çalışmayanlar için reschedule tarihi belirler. Aksiyon sorumlusu sql'i sinyalden beslenip belirlenen formatta oluşturacak şekilde hazırladığı için kontrol mekanizması bu SQL'in geçerliliğini doğrular ve çalışmayanlar için re-schedule oluşturur.

Aksiyon üretim motoru instance'lar halinde çalışacağı için aksiyon havuzunda bu instance'lar ile kaydedilir, ilave olarak action engine run log'ları da bu instance'lar üzerinden oluşturulur.

Aksiyon üretim motoru bir aksiyonu çalıştırırken aynı aksiyon id ile içeride geçerli aksiyon seti varsa onları nasıl güncelleyeceğine aksiyon sorumlusu tarafından karar verilmesi gerekmektedir. Tercihen, mevcutları geçersiz kıl, mevcutu koru, duplicate et, vb olarak uygun seçeneği belirleyebilir (bu kısım tekrar değerlendirilebilir).


### 3.4 Aksiyon Skorlama

Aksiyon havuzuna kaydı yapılan her bir aksiyon için, skorlama engine dışarıdan alacağı veriler ile bir skor hesaplar. Örnek: **xyz ürün eğilim model sinyali** üzerinden üretilen **kredi ürün öneri aksiyonu** için a) kpi performans etkisi b) müşteri memnuniyet etkisi, c) karlılık etkisi, d) strateji uyumluluk etkisi skor bileşenleri bilgilerini dışarıdan alır. Bunun için her aksiyonun bir skorlama sorgusu da olmak zorundadır. Bu durumda aksiyon tanımı esnasından Skor SQL bilgisi de sisteme kaydedilir. Skor SQL'i şu verileri içermesi beklenir: musteri_id, aksiyon_id, hesaplama tarihi, vb. Skor sorgusu çalıştıktan sonra bir ara tabloya kaydedilir ve aktif/planlanmış/süreçte statülerindeki aksiyonların skorları bu tablodan okunur.

Skorlama süreci periodik ve on-demand çalıştırılabilir.

### 3.5 A/B Testing

Aksiyonlar üretildikten sonra skorlama ile eşzamanlı ve bağımsız olarak bir belirlenen kriterlere göre A/B grupları olarak işaretlenir. Her bir aksiyon tanımı için aksiyon sorumlusu aynı zamanda A/B test cluster bilgisini de sisteme kaydetmesi beklenir. Daha basit olması için aksiyon SQL'i içerisinde seçilen alanlar (müşteri segmenti, sektörü, aktiflik durumu vb) concatenate olarak tek bir kolonda sorgunun içerisinde yer alır.

### 3.6 Gerçekleşenler ve Etki Takibi

Aksiyon sorumlusu tanımı yaparken bu aksiyonun hangi sorgu ile takip edileceğini de yine sisteme girmesi beklenir. Bu sorgu aksiyon havuzunda aksiyon statüsü ile birleştirilerek gerçekleşme kriterini aksiyonun planlanma tarihi ile kıyaslayarak gerçekleşmenin kendiliğinden mi yoksa bir plana istinaden mi olduğunu belirler. Gerçekleşme sql'leri günlük olarak çalıştırılır ve gerçekleşen değerler aksiyon statüsünü günceller. İptal edilen veya gerçesiz kalan aksiyonlar için ayrı bir güncelleme sistemş daha sonra tasarlanacaktır. 
