# Ürün Vizyonu — ap-action-management

> **Durum:** Taslak — Alper tarafından doldurulacak.
> Asistan bu dosyayı okuyup boş kalan yerleri sabah brifinglerinde sorabilir.

## Tek cümlelik özet

Bu proje tüzel müşterilere ait analitik ve operasyonel sinyalleri akıllı aksiyonlara dönüştüren ve bu aksiyonların müşteri ve banka stratejisine uyumlu bir şekilde planlanarak yönetimini sağlayan bir **Portföy Yönetim Platformu**'dur.


## Çözülen problem

**Bugün ne oluyor?** 

Farklı kanallardan elde edilen veriler, yine farklı kanallar üzerinden müşteri ve RM’lerle dağınık ve parçalı biçimde paylaşılmaktadır. Bu yapı; aksiyonların uçtan uca takibini, geri bildirimlerin sistematik olarak toplanmasını ve kurumsal hafızanın oluşmasını engellemektedir. 


**Bu neden bir sorun?** 

Bu durum; değerli veri sinyallerinin müşteriye zamanında ve doğru öncelikle ulaştırılamamasına, müşteri geri bildirimlerinin sistematik olarak saklanamaması nedeniyle gerçek ihtiyacın doğru tespit edilememesine ve uzun soluklu müşteri ilişkileri geliştirmek yerine ürün odaklı, reaktif bir satış yaklaşımının öne çıkmasına neden olmaktadır. Sonuç olarak müşteri ihtiyaçlarını daha iyi anlayan, proaktif ve sürdürülebilir bir ilişki modeli oluşturma potansiyeli tam olarak hayata geçirilememektedir.

## Kullanıcılar

| Kullanıcı tipi | Ne yapıyor | Ondan ne bekliyoruz |
|---|---|---|
| Müşteri ilişkileri yöneticileri (RM) | mail, excel, pusula sisteminden gelen listeler üzerinden ürün satışı odaklı ilişki yönetiliyor | Müşterinin ihtiyaçlarını geniş perspektiften anlayabilmeleri, banka önceliklerini ve bireysel performans ihtiyaçlarını da göz önünde bulundurarak müşterileri ile uzun vadeli planlı ilişki kurabilmeleri |

## Bu sürümde hedeflenen

- Bu sürümde projenin omurgasını oluşturan Aksiyon Yönetim Yapısının oluşturulması hedeflenmektedir. Bu yapı sayesinde dağınık sinyaller tek bir havuzda toplanarak hem iş birimleri hem de RM'ler için tekil bir aksiyon kaynağı oluşturmak.

## Bu sürümde hedeflenmeyen

- Ana yapıyı destekleyecek yapay zeka eklentileri kapsam dışında bırakılmıştır
- Tüzel Bankacılık stratejisinin ana unsurları olan Ana Banka, Müşteri Yolculuğu, Ürün Performansları, Müşteri Memnuniyet modülleri kapsam dışında bırakılmıştır.


## Başarı kriterleri

| Kriter                                 | Nasıl ölçülür                                                                                                                | Hedef                                                                                   |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| **Sinyal Kanallarının Konsolidasyonu** | Analitik modeller, kural bazlı listeler, Excel yüklemeleri ve RM notlarından gelen sinyallerin ortak yapıya aktarılabilmesi  | **4 ana sinyal kanalının tamamının entegrasyonu**                                       |
| **Merkezi Aksiyon Yönetimi**           | Tanımlanan aksiyonların tek bir Aksiyon Havuzu üzerinden oluşturulması ve yönetilebilmesi                                    | **Aksiyon tanımlama ve oluşturma süreçlerinin %100 merkezi yapı üzerinden yürütülmesi** |
| **Aksiyon Önceliklendirme**            | Aksiyonların belirlenen skor/önceliklendirme metodolojisine göre sıralanabilmesi                                             | **Uygun aksiyonların %100’ünün skorlanarak önceliklendirilmesi**                        |
| **A/B Test Yetkinliği**                | Aksiyonların kontrollü test ve kontrol gruplarıyla çalıştırılabilmesi ve sonuçlarının karşılaştırılabilmesi                  | **A/B test akışının uçtan uca devreye alınması**                                        |
| **Aksiyon Yaşam Döngüsü Yönetimi**     | Aksiyonların oluşturulma, atama, takip, sonuçlandırma ve geri bildirim adımlarının ilgili ekranlar üzerinden yönetilebilmesi | **Aksiyon yaşam döngüsünün uçtan uca sistem üzerinden yönetilebilir hale gelmesi**      |
| **Gerçek Zamanlı Aksiyon Güncelliği**  | Tamamlanan aksiyonların durum bilgisinin merkezi yapıya aktarılma süresi ve başarı oranı                                     | **Tamamlanan aksiyonların gerçek zamanlıya yakın ve otomatik olarak güncellenmesi**     |


## Bilinen kısıtlar

- Veri ve sistem entegrasyonları: Farklı kaynaklardan gelen verilerin yapısal ve teknik farklılıkları entegrasyon sürelerini etkileyebilir.
- Veri kalitesi ve standardizasyon: Sinyallerin ve RM geri bildirimlerinin ortak bir veri modelinde standardize edilmesi gerekebilir.
- Mevcut sistem bağımlılıkları: Aksiyon yaşam döngüsünün uçtan uca yönetimi, mevcut CRM ve ilgili sistemlerin entegrasyon kabiliyetlerine bağlıdır.
- Gerçek zamanlılık: Kaynak sistemlerin teknik yetkinlikleri nedeniyle bazı aksiyon ve geri bildirimlerin gerçek zamanlı güncellenmesi mümkün olmayabilir.
- KVKK ve veri yönetişimi: Müşteri verilerinin kullanımı, saklanması ve aksiyon üretiminde değerlendirilmesi mevcut veri yönetişimi, yetkilendirme ve KVKK kuralları çerçevesinde ele alınmalıdır.
- Model ve önceliklendirme: Skorlama/önceliklendirme yapısının etkinliği geri bildirim birikimine bağlı olarak zaman içerisinde olgunlaşacaktır.
- İş birimi bağımlılıkları: Aksiyon tanımları, önceliklendirme kriterleri ve geri bildirim mekanizmalarının oluşturulması ilgili iş birimlerinin katılımını gerektirir.
- Takvim ve kapsam: Entegrasyon ve ekran geliştirmelerinin kapsamı, ilgili ekiplerin kapasitesi ve mevcut teknoloji yol haritalarıyla uyumlu şekilde fazlandırılabilir.

---

*Son güncelleme: 2026/08/21*
