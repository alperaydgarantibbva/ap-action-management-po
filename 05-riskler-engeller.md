# Riskler, Engeller ve Bekleyen Kararlar

> Asistan bu dosyayı her sabah okur. Burada duran bir madde çözülmeden kapanmaz, gün geçtikçe brifingte daha yukarı çıkar.

## Aktif engeller (blocker)

*İşin ilerlemesini şu anda durduran şeyler. En acil olanı üstte.*

| # | Ne | Kimi/neyi engelliyor | Kimde | Ne zamandır | Sonraki adım |
|---|---|---|---|---|---|
| B-01 | `[engel]` | `[S-00N]` | `[isim]` | `[tarih]` | `[aksiyon]` |

## Riskler

*Henüz sorun olmamış ama olabilecek şeyler.*

| # | Risk | Olasılık | Etki | Ne yapıyoruz | Kimde |
|---|---|---|---|---|---|
| R-01 | Kullanıcıdan metin olarak alınan SQL'in execute edilmesi — servis user'ın yetki genişliği ve runtime hataları güvenlik açığı yaratabilir | `[teyit edilmedi]` | Yüksek | Bilgi güvenliğinden kayıt açılması gerekiyor; Ecem Ekenoğlu ayrıca sözdizimi doğrulaması yapan bir parser önerdi. Kayıt açıldı mı bilinmiyor — 2026-09-07'de soruldu | `[teyit edilmedi]` |
| R-02 | 1 milyon event'in kısa sürede Kafka'ya basılması Kafka CPU'sunu tabana vurdurabilir | `[teyit edilmedi]` | Yüksek | Dursun Akçeşme'nin uyarısı: 50 binlik partiler şart. Yalnızca Kafka yolu seçilirse geçerli — bkz. D-01 | `[teyit edilmedi]` |
| R-03 | Sizing netleşmemiş: kaç collection, kaç milyon döküman, ~1 KB JSON, ~20 TPS, subsecond beklentisi | `[teyit edilmedi]` | Orta | 2026-09-21'de yüklenen kapsam dokümanı v2 ilk kez sayı veriyor: ~1M müşteri, müşteri başına en fazla 10 ana + 20 alt aksiyon, ~200M canlı erişilebilir kayıt, hot ~100M / warm ~100M / cold ~500M. Ama doküman kendi sayılarının çeliştiğini K-09'da kabul ediyor (200M canlı ile 100+100+500M dağılımı örtüşmüyor) ve katman büyüklükleriyle saklama sürelerinin yeniden hesaplanmasını istiyor. Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan) tarafıyla konuşulacaktı; sahibi ve tarihi hâlâ yazılı değil | `[teyit edilmedi]` |

*R-01…R-03, Alper'in 2026-09-04'te yüklediği `03-toplantilar/20260831-Architecture.md` notundan asistan tarafından çıkarıldı. Alper onaylamadı; olasılık/etki değerleri teyit alınınca güncellenecek.*

## Bekleyen kararlar

*Birinin karar vermesi gereken, verilmediği için işi yavaşlatan konular.*

| # | Karar konusu | Kim karar vermeli | Ne zamandır bekliyor | Karar gecikirse ne olur |
|---|---|---|---|---|
| D-01 | Spark çıktısının OLTP'ye taşınma yolu: Kafka'ya event basıp consumer'ın güncellemesi mi, DWH'ta günlük sil-boşalt yazılan ara tablodan ODI aktarımı mı | `[teyit edilmedi]` — Gökçer Belgüsen event, Dursun Akçeşme ODI tarafında | 2026-08-31 | Aksiyonların ekrana düşme yolu belirsiz kalır; uçtan uca akış çizilemez ve sizing çalışması eksik varsayımla yapılır |
| D-02 | Account Planning maintenance süreç sahipliği | `[teyit edilmedi]` | 2026-08-21 | S-001'in bağımlılığı; kapanmadan S-001 "Hazır" olamaz |

*D-01, Alper'in 2026-09-04'te yüklediği `03-toplantilar/20260831-Architecture.md` notundan asistan tarafından çıkarıldı; kararın kimde olduğu notta yazmıyor, 2026-09-07'de soruldu. Alper onaylamadı.*

**Bekleme süreleri (2026-09-22 itibarıyla):** D-01 22 gün, D-02 32 gün. R-01 ve R-02/R-03 de 22 gündür teyit almamış durumda. Karar sahibi yazılı olmayan tek madde D-01; sorusu iki kez cevapsız kaldığı için 2026-09-18'de bekleyen sorular tablosuna taşındı.

## Kapsam dokümanı v2 karar noktaları (K-01…K-17)

*Kaynak: `03-toplantilar/AccountPlanning-Kapsam-v2.html`, Bölüm 15 — Alper tarafından 2026-09-21 14:00'te yüklendi (commit 05ab867). Aşağıdaki tablo dokümanın kendi 15. bölümünden birebir aktarılmıştır; asistan yorum veya öneri eklemedi. Karar sahibi sütunu dokümanda "İş / Teknik / İş + Teknik" düzeyinde veriliyor, isim verilmiyor — isimler Alper tarafından yazılacak. Tabloya işlenmesi 2026-09-22 brifinginde soruldu, **Alper onaylamadı.***

**Dokümanın kendi öncelik sırası:** MVP1 kapsamının kilitlenmesi için önce **K-08, K-03, K-01 ve K-02** karara bağlanmalı — bu dördü veri modelini ve aksiyon tanım ekranını doğrudan değiştiriyor. Kalan maddeler geliştirme sürerken paralel çözülebilir.

| # | Konu | Karar bekleyen nokta | Dokümanın önerisi | Karar sahibi | Kim (isim) |
|---|---|---|---|---|---|
| K-08 | Skorlama mimarisi | Aksiyon başına skorlama SQL'i mi, merkezi tek sorgu mu — doküman ikisini birlikte anlatıyor, karar verilmemiş | Merkezi yaklaşım dinamik SQL riskini ve operasyon yükünü azaltır; aksiyona özgü istisnalar için tanımlı kaçış yolu bırakılmalı | İş + Teknik | `[yazılacak]` |
| K-03 | A grubu (holdout) görünürlüğü | Kontrol grubu aksiyonlarının PLANNED'da kalıp gösterilmemesi, PLANNED'ın "aktör planladı" anlamıyla çakışıyor | Statüden bağımsız görünürlük alanı (`is_visible` / holdout) eklenmeli; aksiyon PENDING kalmalı | Teknik | `[yazılacak]` |
| K-01 | Alt aksiyon paralelliği | Bir yerde tüm alt aksiyonların seri tasarlanacağı, başka yerde öncülü seçilmemiş olanların ana aksiyonla birlikte başlayabileceği yazıyor | Model paralelliği destekliyor; MVP1'de veri modeli paralel kurulup arayüzde seri akış zorunlu tutulabilir | İş + Teknik | `[yazılacak]` |
| K-02 | Ana aksiyonun tamamlanma koşulu | Alt aksiyonlar önkoşul olarak tanımlanıyor ama ana aksiyonun tamamlanması için beklenmiyor | Alt aksiyonlar "destekleyici adım" olarak adlandırılmalı; tamamlanmayan adımlar eksik iş raporunda izlenmeli | İş | `[yazılacak]` |
| K-04 | Statü adlandırma | Aynı statü metinde PLANLANDI, PLANNED ve PLANLANNED olarak geçiyor | Kodda tek İngilizce enum, arayüzde Türkçe etiket | Teknik | `[yazılacak]` |
| K-05 | Aktör rol kodu | Aktör/RM rolü `SIGNAL_ACTOR` olarak kodlanmış; rol sinyalle değil aksiyonla ilgili | `ACTION_ACTOR` olarak değiştirilmeli | Teknik | `[yazılacak]` |
| K-06 | Aksiyon tanım ekranı yetkisi | ACTION_OWNER'ın "kendi sinyallerini" güncelleyebildiği yazılıyor; sinyal yetkisi SIGNAL_OWNER'da | İfade "kendi aksiyon tanımları" olmalı (doküman içinde düzeltilmiş) | İş | `[yazılacak]` |
| K-07 | ACTION_OWNER yeterlilik profili | Aksiyon sorumlusuna Data Specialist / Data Scientist zorunluluğu konulurken rol dağılımı KOBİ, Ticari ve TMÇ iş birimi olarak veriliyor | SQL yazan ile iş kuralını tarif eden sorumluluk ayrılmalı ya da iş birimlerinde DSp/DSc kadrosu şart koşulmalı | İş | `[yazılacak]` |
| K-09 | Kapasite sayıları | 200M canlı erişilebilir kayıt ile 100M hot + 100M warm + ~500M cold dağılımı birbirini tam karşılamıyor | Katman tanımları ve saklama süreleri sayısal olarak yeniden hesaplanmalı | Teknik | `[yazılacak]` |
| K-10 | Sinyal pasifleştirme sonrası akış | "Sinyal pasife alınıp yeni aksiyon yaratılır" deniyor; yeni sinyalin de gerekip gerekmediği belirsiz | Zincir netleştirilmeli: yeni sinyal → yeni aksiyon. Eski sinyalin pasifi bağlı aksiyonları da pasife çektiği için sıralama tanımlanmalı | İş | `[yazılacak]` |
| K-11 | Yeni aksiyon için JCL süreci | Kaynak metinde bu konuyu anlatan cümle yarım kalmış | Rezerv JCL havuzunun büyüklüğü, tahsis kuralı ve rutine alma kriteri yazılmalı | Teknik | `[yazılacak]` |
| K-12 | Onay akışının zorunluluğu | Aktife almada üst onay "gereken durumlarda" olarak geçiyor, koşul tanımlı değil | Onay gerektiren durumlar (yeni aksiyon, SQL değişikliği, kapsam büyüklüğü) listelenmeli. Organizasyon Süreç Gelişim ekibiyle netleşecek | İş | `[yazılacak]` |
| K-13 | Sinyal adı duplikasyonu | Ad tekilliği aranmadığı için duplikasyon riski manuel kontrole bırakılmış | Ad benzerliği uyarısı ve periyodik duplikasyon raporu eklenmeli | Teknik | `[yazılacak]` |
| K-14 | Devir onay süresi | Devir talebi onaylanmazsa iptal olacağı belirtiliyor, süre tanımlı değil | Zaman aşımı parametrik tanımlanmalı, bekleyen devirler aktörün ekranında görünmeli | İş | `[yazılacak]` |
| K-15 | ACTION_APPROVER ölçeği | Rol ~10 kişi olarak veriliyor, dağılım 5 kişi üzerinden tarif ediliyor | Dağılım güncellenmeli | İş | `[yazılacak]` |
| K-16 | Aksiyon günlüğü etiketleri | Kritiklik etiketlerinin kapsamı "netleştirilecek" olarak bırakılmış | Etiket kümesi ve atama kuralı tanımlanmalı | İş | `[yazılacak]` |
| K-17 | Yeniden üretim bekleme süresi | NOT_POSSIBLE statüsünde "belirli bir süre" yeniden üretim yapılmayacağı deniyor, süre tanımlı değil | Süre aksiyon tanımında parametrik olmalı; varsayılan değer belirlenmeli | İş | `[yazılacak]` |

**K-01…K-17 ile D-01/D-02 ilişkisi:** Doküman D-01'i (Spark çıktısının OLTP'ye taşınma yolu) kapatmıyor — Bölüm 13 skorların "OLTP'ye geri yazıldığını" söylüyor ama Kafka event mi, DWH ara tablo + ODI mi olduğunu yazmıyor. D-02 (Account Planning maintenance süreç sahipliği) de dokümanda adı geçen bir karar noktası değil; doküman katman bazlı yönetişim sorumlusu (SIGNAL_OWNER, ACTION_OWNER, PERFORMANCE_OWNER, ABTEST_OWNER, MONITORING_OWNER) tanımlıyor ama maintenance süreç sahipliğini bunlardan birine bağlamıyor. İkisi de açık kalmaya devam ediyor. [teyit edilmedi]

## Haftalık kapanış notları

*Cuma günü asistanın yazdığı tek satırlık durum. Amaç: hafta hafta neyin ilerlediğini geriye dönüp görebilmek.*

| Hafta | Kapanışta durum |
|---|---|
| 2026-09-14 – 2026-09-18 | Repoya Alper'den içerik gelmedi (son commit 6a3560d, 2026-09-04). Hiçbir engel/karar kapanmadı: D-01 18, D-02 28 gündür açık. S-001 28 gündür Taslak. 17 Eylül workshop tarihi kayıt oluşmadan geçti. Paydaş bilgilendirmesinde Ağustos ve Eylül turu kaçtı. Asistan bu hafta `oncelik.md` sıralama kriterlerini ve `03-toplantilar/20260917-karar-formu-taslak.md`'yi onay beklemeden yazdı. |

## Cevap bekleyen sorular

*Asistanın sorduğu ama cevaplanmamış sorular buraya düşer. Tamamı Alper'e sorulmuştur.*

> **2026-09-21:** Tablo 53 satırda. Dört soru (17 Eylül workshop notunun D-02'yi kapatıp
> kapatmadığı, S-001'in "Beklemede"ye alınması, 17 Eylül takvim satırının ve hazırlık taslağının
> silinmesi, paydaş taslağının Eylül'e çekilmesi) ikinci kez cevapsız kaldığı için C, F ve H
> başlıklarına taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-18:** Tablo 49 satırda. Bir soru (D-01 kararını kimin vereceği) ikinci kez cevapsız
> kaldığı için H başlığına taşındı; artık brifingte sorulmuyor.
>
> **2026-09-17:** Tablo 48 satırda. İki soru (workshop hazırlık taslağının bu haliyle
> kullanılabilir olup olmadığı, `oncelik.md` sıralama kriterleri taslağı) ikinci kez cevapsız
> kaldığı için H ve E başlıklarına taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-16:** Tablo 46 satırda. İki soru (17 Eylül workshop'una Alper'in katılıp
> katılmadığı, bu hafta ekiple kayıtlı toplantı olup olmadığı) ikinci kez cevapsız kaldığı
> için H ve A başlıklarına taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-15:** Tablo 44 satırda. İki soru (risk tablosundaki üç riskin doğruluğu, repoya
> eklenmemiş yeni toplantı notu olup olmadığı) ikinci kez cevapsız kaldığı için H ve B
> başlıklarına taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-14:** Tablo 42 satırda. İki soru (31 Ağustos notundaki uçtan uca akışın tek
> sayfalık şemaya çevrilmesi, R-01'in aktif engel olarak işaretlenmesi) ikinci kez cevapsız
> kaldığı için G ve H başlıklarına taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-11:** Tablo 40 satırda. İki soru (Sprint 1 hedef cümlesi taslağı, 17 Eylül
> workshop'unda ap-action-management'ın gündemde olup olmadığı) ikinci kez cevapsız kaldığı
> için A ve H başlıklarına taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-10:** Tablo 38 satırda. İki soru (sizing için Big Data/Couchbase tarafına gidecek soru
> metni, cevapsız soruların tek kontrol listesi issue'sunda toplanması) ikinci kez cevapsız kaldığı
> için H ve I başlıklarına taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-09:** Tablo 36 satırda. Dört soru (D-01 kaydı, bilgi güvenliği kaydı, ikinci uçtan uca
> toplantı tarihi, S-001 parser kabul kriteri) ikinci kez cevapsız kaldığı için A, C ve H başlıklarına
> taşındı; artık brifingte sorulmuyorlar.
>
> **2026-09-04:** Tablo 30 satıra çıktığı için konu başlıklarına göre gruplandı. Satırlar ve
> tarihleri değişmedi, yalnızca sıralandı. Amaç: bir başlığın tamamını tek oturumda cevaplayabilmek.
> Bir başlık cevaplanınca o blok "Kapanmış maddeler"e taşınacak.

### A. Sprint ve tören takvimi (6 soru)

*Cevaplanmazsa: `ekip-ve-ritim.md` şablon değerlerinde kalır, brifing "bugün tören var mı" sorusuna cevap veremez.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | Aktif sprint hangisi ve tarihleri ne? (3 kez soruldu) |
| 2026-08-18 | Tören takvimi nasıl — refinement, planlama, review hangi gün/saat? (3 kez soruldu) |
| 2026-08-21 | Sprint 1 hangi tarihte bitiyor? (2 kez soruldu) |
| 2026-09-07 | Ecem Ekenoğlu ve Dursun Akçeşme'nin istediği ikinci uçtan uca akış toplantısı için tarih belirlendi mi? (2 kez soruldu; 2026-09-09'da tabloya taşındı) |
| 2026-09-09 | Sprint 1 için hedef cümlesi taslağını ben yazayım mı? (2 kez soruldu; 2026-09-11'de tabloya taşındı) |
| 2026-09-14 | Bu hafta ekiple kayıtlı bir toplantın var mı, varsa hangi gün? (2 kez soruldu; 2026-09-16'da tabloya taşındı) |

### B. Ekip, sahiplik ve ilerleme (4 soru)

*Cevaplanmazsa: `ekip-ve-ritim.md` ekip tablosu ve 5 epic'in "Sahip" satırı boş kalır; repoda ekibin ilerlemesine dair hiçbir kayıt oluşmaz.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | Ekipte Scrum Master kim? (3 kez soruldu) |
| 2026-08-28 | KickOff'taki 6 sahiplik rolü (Signal, Action, Strategic Priority, A/B Test, Performance, Reporting Owner) için isimler belirlendi mi? (2 kez soruldu) |
| 2026-09-04 | Bu hafta ekip tarafında kapanan bir iş oldu mu? (2 kez soruldu; 2026-09-08'de tabloya taşındı) |
| 2026-09-11 | Elinde repoya eklenmemiş yeni bir toplantı notu var mı? (2 kez soruldu; 2026-09-15'te tabloya taşındı) |

### C. S-001 (9 soru)

*Cevaplanmazsa: S-001 "Taslak"ta kalır, Definition of Ready karşılanmaz, refinement gündemine giremez. Backlog'daki tek story bu.*

| Tarih | Soru |
|---|---|
| 2026-08-21 | S-001 doğru konuyu tarif ediyor mu, bu haliyle ekibe gösterilebilir mi? (2 kez soruldu) |
| 2026-08-21 | Account Planning maintenance süreç sahipliğini bekleyen karar olarak kaydedeyim mi? (2 kez soruldu; S-001'in bağımlılığı) |
| 2026-08-25 | S-001'deki iş Account Planning tarafında mı, GT Pusula tarafında mı geliştirilecek? (2 kez soruldu; S-001'in açık sorusu) |
| 2026-08-27 | Ortak klasöre manuel SQL bırakma yolu S-001 ile kapatılacak mı, bir süre paralel mi yürüyecek? (2 kez soruldu; S-001'in açık sorusu) |
| 2026-09-02 | S-001'i iki açık sorusu kapanmadan refinement'a sokayım mı? (2 kez soruldu) |
| 2026-09-03 | S-001'i ikiye böleyim mi — (1) gönderim + otomatik doğrulama, (2) onay akışı + işlem geçmişi? (2 kez soruldu) |
| 2026-09-03 | S-001'in iki teknik açık sorusunu Umut Özdemir ve Garo Üçkardeş'e soracak kısa mesaj taslağını çıkarayım mı? (2 kez soruldu) |
| 2026-09-07 | S-001'in kabul kriterlerine sözdizimi doğrulaması (parser) maddesini ekleyeyim mi? (2 kez soruldu; 2026-09-09'da tabloya taşındı) |
| 2026-09-17 | S-001'i "Taslak"tan "Beklemede"ye alayım mı? (2 kez soruldu; 2026-09-21'de tabloya taşındı — bağımlılığı D-02 açık) |

### D. Backlog ve epic'ler (3 soru)

*Cevaplanmazsa: 5 epic ve `oncelik.md` epic tablosu "onaylanmadı" işaretiyle durur, backlog'da tek story kalır.*

| Tarih | Soru |
|---|---|
| 2026-08-24 | Vizyondaki 6 başarı kriterinden / Action Engine README'deki 5 başlıktan epic taslakları çıkarayım mı? (2 kez soruldu; 2026-08-31'de onay beklemeden çıkarıldı) |
| 2026-08-31 | Açılan 5 epic (E-01…E-05) bu haliyle onaylanıyor mu? (2 kez soruldu) |
| 2026-09-02 | E-01 CAPTURE altına ilk story taslağını çıkarayım mı? (2 kez soruldu) |

### E. Öncelik (3 soru)

*Cevaplanmazsa: haftalık hedef yazılı olmaz, `oncelik.md` sıralaması onaysız kalır.*

| Tarih | Soru |
|---|---|
| 2026-08-19 | Bu hafta ekibin bitirmesini en çok istediğin tek iş ne? (2 kez soruldu) |
| 2026-08-24 | Bu haftanın tek hedefi S-001'i "Hazır" duruma getirmek olsun mu? (2026-08-31'de tekrar soruldu) |
| 2026-09-15 | `01-backlog/oncelik.md` sıralama kriterlerinin taslağını ben yazayım mı? (2 kez soruldu; 2026-09-17'de tabloya taşındı) |

### F. Paydaş iletişimi (3 soru)

*Cevaplanmazsa: 21 paydaşın "son iletişim" sütunu boş kalır, aylık bilgilendirme sayacı başlamaz.*

| Tarih | Soru |
|---|---|
| 2026-08-28 | 21 paydaşa gidecek ilk aylık güncelleme taslağını çıkarayım mı? (2 kez soruldu; 2026-08-31'de onay beklemeden yazıldı: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi) |
| 2026-08-31 | Bu taslak gönderilebilir mi / Eylül'ün ilk haftasında gönderilecek mi? (2 kez soruldu) |
| 2026-09-17 | Paydaş güncelleme taslağının tarihini Eylül'e çekip göndermeye hazır hale getireyim mi? (2 kez soruldu; 2026-09-21'de tabloya taşındı) |

### G. Proje tanımı ve prototip kapsamı (4 soru)

*Cevaplanmazsa: `vizyon.md` kapsam sınırı ve prototip çalışmasının backlog'daki yeri belirsiz kalır.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | ap-action-management tek cümleyle neyi yönetiyor? (3 kez soruldu) |
| 2026-08-25 | accountplanning.ai üzerinde yayınlanacak prototip için hedef tarih var mı? (2 kez soruldu) |
| 2026-08-27 | Action Engine prototipi ekibin geliştirme kapsamında mı, hizalanma amaçlı ayrı bir çalışma mı? (2 kez soruldu) |
| 2026-09-10 | 31 Ağustos Architecture notundaki uçtan uca akışı tek sayfalık şemaya ben çevireyim mi? (2 kez soruldu; 2026-09-14'te tabloya taşındı) |

### H. Risk, engel ve takvim (15 soru)

*Cevaplanmazsa: aktif engel tablosu ve risk tablosu boş kalır — engel/risk olmadığı için değil, teyit alınamadığı için.*

| Tarih | Soru |
|---|---|
| 2026-08-21 | EVAM'ın sprint başına 2-3 event kısıtını risk olarak kaydedeyim mi? (2 kez soruldu) |
| 2026-08-21 | PlanItEarth workshop'u yapıldı mı, yoksa 17 Eylül'de mi? (2026-08-31'de tekrar soruldu) |
| 2026-08-28 | Şu an ekibin işini durduran bir engel var mı? (2 kez soruldu) |
| 2026-09-03 | 17 Eylül workshop'u için gündem taslağı çıkarayım mı? (2 kez soruldu; 2026-09-07'de tabloya taşındı) |
| 2026-09-07 | D-01'i (Spark çıktısının OLTP'ye taşınma yolu: Kafka event / ODI ara tablo) bekleyen karar olarak kayıtlı tutayım mı? (2 kez soruldu; 2026-09-09'da tabloya taşındı) |
| 2026-09-07 | Metin olarak alınan SQL'in execute edilmesi için bilgi güvenliğinden kayıt açıldı mı? (2 kez soruldu; 2026-09-09'da tabloya taşındı — R-01'in tek açık ucu) |
| 2026-09-08 | Sizing için Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan) tarafına gidecek tek paragraflık soru metnini çıkarayım mı? (2 kez soruldu; 2026-09-10'da tabloya taşındı — R-03'ün tek açık ucu) |
| 2026-09-09 | 17 Eylül PlanItEarth workshop'unda ap-action-management gündemde mi? (2 kez soruldu; 2026-09-11'de tabloya taşındı) |
| 2026-09-10 | R-01'i (metin olarak alınan SQL'in execute edilmesi) aktif engel / blocker olarak işaretleyeyim mi? (2 kez soruldu; 2026-09-14'te tabloya taşındı) |
| 2026-09-11 | Risk tablosundaki üç risk (R-01 SQL güvenliği, R-02 Kafka yükü, R-03 sizing) bu haliyle doğru mu? (2 kez soruldu; 2026-09-15'te tabloya taşındı) |
| 2026-09-14 | 17 Eylül PlanItEarth workshop'una sen katılıyor musun? (2 kez soruldu; 2026-09-16'da tabloya taşındı) |
| 2026-09-15 | `03-toplantilar/20260914-workshop-hazirlik-taslak.md` bu haliyle kullanılabilir mi? (2 kez soruldu; 2026-09-17'de tabloya taşındı) |
| 2026-09-16 | D-01 kararını (Kafka event mi, DWH ara tablo + ODI mi) kim verecek — Gökçer Belgüsen mi, Dursun Akçeşme mi? (2 kez soruldu; 2026-09-18'de tabloya taşındı — D-01'in karar sahibi yazılı değil) |
| 2026-09-17 | `03-toplantilar/20260917-PlanItEarth-Workshop.md` notundaki "ekip tüm geliştirme ve maintenance'dan sorumlu olacak" satırı D-02'yi kapatıyor mu? (2 kez soruldu; 2026-09-21'de tabloya taşındı — D-02 31 gündür açık) |
| 2026-09-17 | `ekip-ve-ritim.md`'deki 17 Eylül workshop satırını ve `03-toplantilar/20260914-workshop-hazirlik-taslak.md`'yi silelim mi? (2 kez soruldu; 2026-09-21'de tabloya taşındı — tarih kayıt oluşmadan geçti) |

### I. Brifing kanalı (6 soru)

*Cevaplanmazsa: brifingin gün/saat/sıklığı varsayımla yürümeye devam eder. #7–#15 arası dokuz brifing cevapsız.*

| Tarih | Soru |
|---|---|
| 2026-08-20 | Brifingleri telefonunda bildirim olarak görüyor musun? (2 kez soruldu) |
| 2026-08-20 | Brifing saati 08:30 uygun mu, 18:00 daha mı iyi? (2 kez soruldu) |
| 2026-08-25 | Soruları cevaplamak için issue yorumu mu daha kolay, doğrudan commit mi? |
| 2026-08-27 | Brifing hafta içi her gün mü çalışsın, Pazartesi/Cuma mı kalsın? (2 kez soruldu) |
| 2026-09-03 | Cevap vermeye vaktin yoksa brifingi geçici olarak durdurayım mı? (2 kez soruldu) |
| 2026-09-04 | Bugüne kadar cevapsız kalan soruları tek bir kontrol listesi issue'sunda toplayayım mı? (2 kez soruldu; 2026-09-10'da tabloya taşındı) |

## Kapanmış maddeler

*Silmeyin, buraya taşıyın. Retro'da işe yarar.*

| # | Ne | Nasıl kapandı | Tarih |
|---|---|---|---|
| | | | |

---

*Son güncelleme: 2026-09-22*
