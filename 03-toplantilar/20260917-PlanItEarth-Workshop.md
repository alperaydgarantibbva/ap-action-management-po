Katılımcılar: PlanItEarth
Konu: Account Planning Ekranları
Notlar: 

# Proje Genel Konuları:
* Account Planning ever leaving bir proje olacak, bir modül gibi çalışacak, ekip tüm geliştirme ve maintenance'dan sorumlu olacak

* Müşteri karşılama ve RM karşılama ekranları superbanker projesi kapsamında geliştirilecek. Ürün performans, ana banka, müşteri yolculuğu, müşteri memnuniyeti, Aksiyon yönetimi süreçleri Account Planning kapsamında geliştirilecek.

* RM ekranı dışında şube, bölge seviyeleri de çalışılacak

* Mikro'yu da kapsama opsiyonu mevcut, potansiyel müşteri sayısı 4mio olabilir


# Sinyal-Aksiyon yönetimi:
Sinyal, Aksiyon, Monitor tanımlama ve geçerlilik süreleri bağımsız olacak. 

Sinyal definition tablosunda Sinyal'in oluştuktan sonra ne kadar geçerli olacağı, Aksiyon definition tablosunda aksiyon'un ne kadar süre geçerli olacağı tanımlı olacak. RM aksiyonu dilediği süre kadar planlayabilir. Örnek: churn modeli sinyali 1 Temmuz tarihinde oluştu, sinyal sorumlusu definition'da 1 ay geçerli olduğunu belirtmiş, bu sinyal'e bağlı aksiyonlar 1 Temmuz - 31 Temmuz aralığında tanımlanabilir. Hali hazırda tanımlı aksiyon varsa sinyal oluşumunu takiben aksiyon oluşacaktır, ancak 15 Temmuz'da yeni bir aksiyon tanımlanmışsa geçerlilik süresi içerisinde bekleyen sinyaller için aksiyon üretilebilir. 

Aksiyon sorumlusu aksiyonun ne kadar süre içerisinde alınması gerektiğini tanım tablosunda belirler. Aksiyon oluştuktan sonra sinyal süresinden bağımsız bir şekilde daha uzun veya daha kısa bir süre tanımlanabilir. Örneğin, müşterinin dış ticaret eğilimini yakalayan bir sinyale bağlı bir aksiyon 3 ay veya daha uzun süre geçerli olabilir. Veya hızlı aksiyon gereken durumlarda sinyalin alınması sonrasında 1 hafta gibi bir süre içerisinde aksiyon alınması, gecikme durumunda sinyalin eskimesi riskine karşı kısa bir süre de belirlenebilir.

RM planlamaya aldığı bir aksiyon için yine sınırsız bir plan date girebilir. Müşteri ile görüşmesi sonrasında planlanan aksiyon için müşterinin kabul ettiği bir zaman üzerinde el sıkışmış olabilirler. Opsiyonel olarak aksiyon'a girilecek tarih soft bir şekilde sınırlanabilir (max 3 ay gibi)

* Pusula'daki metrik dinamizmi sql'ler ile sağlanıyor. İlk tasarımdaki sinya-aksiyon izolasyonu veri zenginleştirme adımında dinamik join'ler ilave komplekslik yarattığı için aksiyon'lar  sql olarak tanımlanacak ve içerisinde sinyal zenginleştirme joinleri de hazır halde iletilecek. Sinyal sorumlusu Aksiyon sorumlusu ile birlikte aksiyon SQL'ini hazırlayacak. Aksiyon Sorumlusu sql'in doğru çalışmasından sorumlu olacak.

# Aksiyon Yönetimi
* Aksiyon Modülü 3 farklı connector ve iki katmandan oluşacak.
1. Sinyal girdileri için DWH katmanından alınan sinyal+aksiyonlar Aksiyon Havuzu'nu besleyecek, her bir sinyal tipi için ayrı ODI veya Servis Call geliştirilecek.
2. Scoring için DWH katmanından a) RM Pusula skoru b) Organizasyonel öncelikler ürün lookup tablosu - fastedit c) Piyasa Verileri - TBD alınacak
3. Monitoring için her bir aksiyon tipi için canlı sistem ve/veya ODS'ten ayrı ODI veya Service Call geliştirilecek

# Scoring Yönetimi
* Scoring yapısı periyodik + on-demand. Aksiyon tanımlandıktan sonra scoring çalışacak. Scoring günlük periyodik çalışarak RM'in pusulası, piyasa bilgileri, banka stratejileri gibi değişkenleri kullanarak hesaplanacak. APKO veya regülasyon vb kararlar sonrasında scoring değişkenlerinin değişmesi gereken durumlarda on-demand de çalışması gerekecek.
* Scoring veri kaynakları: 
    1) RM pusula verileri üzerinden ilişkili üründeki hedefe uzaklı ile hesaplanacak (dwh'tan okunacak, 0-100 arası bir skor) 
    2) Organizasyonel öncelikler (ürün+servis'ler DWH'ta fast-edit olarak tutulabilir, her biri 0-100 arası gibi bir skor ile öncelikler belirlenebilir) 
    3) Müşteri memnuniyet etkisi (iki opsiyon: a. aksiyon tanımı yapılırken aksiyon yöneticisi default değerler girebilir, b. her müşteri için müşteri verisi üzerinden hesaplanabilir (tbd)  )
    4) Ürün karlılık etkisi. (iki opsiyon a. aksiyon tanımında, b. müşteri bazlı (tbd) )

# Monitoring Yönetimi
* near-real time besleme gerekliliği, RM'in güncellenen aksiyonlar için manuel giriş yapmaması gerekiyor, sürtünmeyi en aza indirmek için. Bunu ilk mvp'de bu şekilde çıkmayı planlıyoruz.
* Kaynak sistemlerden çok sayıda eş zamanlı veri okuma gerekliliği var, ODI / Servis / Kafka / CDC. Kaynak sistemlere bağımlılık yaratılmaması gerekiyor.

# SuperBanker İlişkilendirme:
* Müşteri karşılama ekranlarında mevcut ürünler + potansiyel ürünler + treshold + aksiyonlar'ların görünmesi sağlanacak. Burada iki önemli nokta 1) superbanker'a adreslenen müşteri karşılama ekranına aksiyon bilgilerinin akması (TL Nakdi, 2/5 aksiyon planlanan) 2) superbanker ürün paneli account planning aksiyon yönetim ekranlarının ilişkilendirilmesi (Ürüne tıklanınca aksiyon panelinin açılması, statü değişiklikleri vb.)

# Teknik Konular:
* Veri yapısı OLTP ve DWH olarak iki parçada ele alınmalı 
* DWH-OLTP için üç input bir output kaynağı (connector) : 1) Sinyaller, 2) Monitoring, 3) Scoring 4) Rapor/Monitoring output
* Scoring ve A/B test akışları bağımsız, paralel çalışabilir, yerleri değişebilir
* EVAM opsiyonunun Kafka beslemesi ile bağımlılığı var, mevcutta var olmayan besleme ihtiyaçları için event geliştirilmesi gerekiyor, ilgili ekip tarafından her sprintte 2-3 event ancak geliştirilebiliyor.
 