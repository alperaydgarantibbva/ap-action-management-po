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
| R-03 | Sizing netleşmemiş: kaç collection, kaç milyon döküman, ~1 KB JSON, ~20 TPS, subsecond beklentisi | `[teyit edilmedi]` | Orta | Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan) tarafıyla konuşulacaktı; sahibi ve tarihi yazılı değil | `[teyit edilmedi]` |

*R-01…R-03, Alper'in 2026-09-04'te yüklediği `03-toplantilar/20260831-Architecture.md` notundan asistan tarafından çıkarıldı. Alper onaylamadı; olasılık/etki değerleri teyit alınınca güncellenecek.*

## Bekleyen kararlar

*Birinin karar vermesi gereken, verilmediği için işi yavaşlatan konular.*

| # | Karar konusu | Kim karar vermeli | Ne zamandır bekliyor | Karar gecikirse ne olur |
|---|---|---|---|---|
| D-01 | Spark çıktısının OLTP'ye taşınma yolu: Kafka'ya event basıp consumer'ın güncellemesi mi, DWH'ta günlük sil-boşalt yazılan ara tablodan ODI aktarımı mı | `[teyit edilmedi]` — Gökçer Belgüsen event, Dursun Akçeşme ODI tarafında | 2026-08-31 | Aksiyonların ekrana düşme yolu belirsiz kalır; uçtan uca akış çizilemez ve sizing çalışması eksik varsayımla yapılır |
| D-02 | Account Planning maintenance süreç sahipliği | `[teyit edilmedi]` | 2026-08-21 | S-001'in bağımlılığı; kapanmadan S-001 "Hazır" olamaz |

*D-01, Alper'in 2026-09-04'te yüklediği `03-toplantilar/20260831-Architecture.md` notundan asistan tarafından çıkarıldı; kararın kimde olduğu notta yazmıyor, 2026-09-07'de soruldu. Alper onaylamadı.*

## Cevap bekleyen sorular

*Asistanın sorduğu ama cevaplanmamış sorular buraya düşer. Tamamı Alper'e sorulmuştur.*

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

### A. Sprint ve tören takvimi (5 soru)

*Cevaplanmazsa: `ekip-ve-ritim.md` şablon değerlerinde kalır, brifing "bugün tören var mı" sorusuna cevap veremez.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | Aktif sprint hangisi ve tarihleri ne? (3 kez soruldu) |
| 2026-08-18 | Tören takvimi nasıl — refinement, planlama, review hangi gün/saat? (3 kez soruldu) |
| 2026-08-21 | Sprint 1 hangi tarihte bitiyor? (2 kez soruldu) |
| 2026-09-07 | Ecem Ekenoğlu ve Dursun Akçeşme'nin istediği ikinci uçtan uca akış toplantısı için tarih belirlendi mi? (2 kez soruldu; 2026-09-09'da tabloya taşındı) |
| 2026-09-09 | Sprint 1 için hedef cümlesi taslağını ben yazayım mı? (2 kez soruldu; 2026-09-11'de tabloya taşındı) |

### B. Ekip, sahiplik ve ilerleme (3 soru)

*Cevaplanmazsa: `ekip-ve-ritim.md` ekip tablosu ve 5 epic'in "Sahip" satırı boş kalır; repoda ekibin ilerlemesine dair hiçbir kayıt oluşmaz.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | Ekipte Scrum Master kim? (3 kez soruldu) |
| 2026-08-28 | KickOff'taki 6 sahiplik rolü (Signal, Action, Strategic Priority, A/B Test, Performance, Reporting Owner) için isimler belirlendi mi? (2 kez soruldu) |
| 2026-09-04 | Bu hafta ekip tarafında kapanan bir iş oldu mu? (2 kez soruldu; 2026-09-08'de tabloya taşındı) |

### C. S-001 (8 soru)

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

### D. Backlog ve epic'ler (3 soru)

*Cevaplanmazsa: 5 epic ve `oncelik.md` epic tablosu "onaylanmadı" işaretiyle durur, backlog'da tek story kalır.*

| Tarih | Soru |
|---|---|
| 2026-08-24 | Vizyondaki 6 başarı kriterinden / Action Engine README'deki 5 başlıktan epic taslakları çıkarayım mı? (2 kez soruldu; 2026-08-31'de onay beklemeden çıkarıldı) |
| 2026-08-31 | Açılan 5 epic (E-01…E-05) bu haliyle onaylanıyor mu? (2 kez soruldu) |
| 2026-09-02 | E-01 CAPTURE altına ilk story taslağını çıkarayım mı? (2 kez soruldu) |

### E. Öncelik (2 soru)

*Cevaplanmazsa: haftalık hedef yazılı olmaz, `oncelik.md` sıralaması onaysız kalır.*

| Tarih | Soru |
|---|---|
| 2026-08-19 | Bu hafta ekibin bitirmesini en çok istediğin tek iş ne? (2 kez soruldu) |
| 2026-08-24 | Bu haftanın tek hedefi S-001'i "Hazır" duruma getirmek olsun mu? (2026-08-31'de tekrar soruldu) |

### F. Paydaş iletişimi (2 soru)

*Cevaplanmazsa: 21 paydaşın "son iletişim" sütunu boş kalır, aylık bilgilendirme sayacı başlamaz.*

| Tarih | Soru |
|---|---|
| 2026-08-28 | 21 paydaşa gidecek ilk aylık güncelleme taslağını çıkarayım mı? (2 kez soruldu; 2026-08-31'de onay beklemeden yazıldı: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi) |
| 2026-08-31 | Bu taslak gönderilebilir mi / Eylül'ün ilk haftasında gönderilecek mi? (2 kez soruldu) |

### G. Proje tanımı ve prototip kapsamı (3 soru)

*Cevaplanmazsa: `vizyon.md` kapsam sınırı ve prototip çalışmasının backlog'daki yeri belirsiz kalır.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | ap-action-management tek cümleyle neyi yönetiyor? (3 kez soruldu) |
| 2026-08-25 | accountplanning.ai üzerinde yayınlanacak prototip için hedef tarih var mı? (2 kez soruldu) |
| 2026-08-27 | Action Engine prototipi ekibin geliştirme kapsamında mı, hizalanma amaçlı ayrı bir çalışma mı? (2 kez soruldu) |

### H. Risk, engel ve takvim (8 soru)

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

*Son güncelleme: 2026-09-11*
