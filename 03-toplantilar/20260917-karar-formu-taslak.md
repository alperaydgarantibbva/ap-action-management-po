# Açık Kararlar — Tek Sayfalık Karar Formu (TASLAK)

> **Durum: Alper onaylamadı.** Asistan 2026-09-17'de yazdı. Kaynak:
> `20260831-Architecture.md`, `20260917-PlanItEarth-Workshop.md`, `05-riskler-engeller.md`.
> 2026-09-16 brifingde teklif edilmişti; cevap gelmedi, tarih geldiği için üretildi.
>
> **İki kullanımı var:** (1) 17 Eylül workshop'u takvimde gerçekten varsa toplantıya
> bununla girilir; (2) yoksa D-01 ve D-02 sahiplerine tek tek sorulacak liste olarak
> kullanılır. Toplantının takvimde durup durmadığı **[teyit edilmedi]**.
>
> PO kuralı: buraya çözüm değil **soru** götürülür. Kararı teknik sahipler verir;
> senin işin kararın *kimde* olduğunu ve *ne zamana* bağlandığını yazıya geçirmek.

## Form

Her satır için tek hedef: boş üç kutuyu doldurmak. Karar çıkmazsa en azından
"kim" ve "ne zaman" dolsun — karar sahibi ve tarih yazılmayan konu bir daha gündeme gelmiyor.

| # | Karar / soru | Karar | Kim verir | Ne zamana kadar |
|---|---|---|---|---|
| D-01 | Spark çıktısı OLTP'ye nasıl taşınacak: Kafka'ya event basıp consumer mı güncelleyecek, DWH'ta günlük sil-boşalt yazılan ara tablodan ODI aktarımı mı? | | | |
| R-02 | Kafka seçilirse 50 binlik partiler kuralı yeterli mi; 1 milyon event için hedef süre ne? | | | |
| R-01 | Metin olarak alınan SQL'in execute edilmesi için bilgi güvenliğinden kayıt açıldı mı; açılmadıysa kim açacak? | | | |
| S-001 | Ecem Ekenoğlu'nun önerdiği sözdizimi doğrulaması (parser) kapsamda mı — S-001'in kabul kriterine girmeli mi? | | | |
| R-03 | Sizing sorusunu Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan) tarafına kim soracak, ne zaman? | | | |
| D-02 | Account Planning maintenance sürecinin sahibi kim? | | | |

**D-02 için not:** `20260917-PlanItEarth-Workshop.md` içinde "Account Planning ever
leaving bir proje olacak, bir modül gibi çalışacak, ekip tüm geliştirme ve
maintenance'dan sorumlu olacak" yazıyor. Bu satır D-02'yi kapatıyor olabilir ama
"ekip" bir isim değil; süreç sahibinin adı hâlâ yazılı değil. 2026-09-17 brifingde soruldu.

## Bu form doldurulursa ne kapanır

- D-01 ve D-02 → bekleyen kararlar tablosundan "Kapanmış maddeler"e taşınır.
- R-01, R-02, R-03 → olasılık/etki değerleri ve sahipleri netleşir, `[teyit edilmedi]` kalkar.
- S-001 → parser maddesi karara bağlanırsa açık sorularından biri kapanır; D-02 de
  kapanırsa Definition of Ready kontrolü yeniden çalıştırılabilir.

## Toplantıda yapmayacakların

- Teknik kararı sen verme; kararı kimin ve ne zaman vereceğini yazıya bağla.
- Tahmin/efor sorma — onu ekip verir.
- Yeni kapsam açılırsa (Mikro, superbanker entegrasyonu) sprint hedefine hizmet
  etmiyorsa backlog'a al, aynı toplantıda karara bağlama.

---

*Oluşturma: 2026-09-17 — asistan taslağı, onay bekliyor.*
