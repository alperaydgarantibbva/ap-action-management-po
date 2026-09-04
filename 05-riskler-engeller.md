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
| R-01 | `[risk]` | Yüksek/Orta/Düşük | Yüksek/Orta/Düşük | `[önlem]` | `[isim]` |

## Bekleyen kararlar

*Birinin karar vermesi gereken, verilmediği için işi yavaşlatan konular.*

| # | Karar konusu | Kim karar vermeli | Ne zamandır bekliyor | Karar gecikirse ne olur |
|---|---|---|---|---|
| D-01 | `[konu]` | `[isim]` | `[tarih]` | `[sonuç]` |

## Cevap bekleyen sorular

*Asistanın sorduğu ama cevaplanmamış sorular buraya düşer. Tamamı Alper'e sorulmuştur.*

> **2026-09-04:** Tablo 30 satıra çıktığı için konu başlıklarına göre gruplandı. Satırlar ve
> tarihleri değişmedi, yalnızca sıralandı. Amaç: bir başlığın tamamını tek oturumda cevaplayabilmek.
> Bir başlık cevaplanınca o blok "Kapanmış maddeler"e taşınacak.

### A. Sprint ve tören takvimi (3 soru)

*Cevaplanmazsa: `ekip-ve-ritim.md` şablon değerlerinde kalır, brifing "bugün tören var mı" sorusuna cevap veremez.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | Aktif sprint hangisi ve tarihleri ne? (3 kez soruldu) |
| 2026-08-18 | Tören takvimi nasıl — refinement, planlama, review hangi gün/saat? (3 kez soruldu) |
| 2026-08-21 | Sprint 1 hangi tarihte bitiyor? (2 kez soruldu) |

### B. Ekip ve sahiplik (2 soru)

*Cevaplanmazsa: `ekip-ve-ritim.md` ekip tablosu ve 5 epic'in "Sahip" satırı boş kalır.*

| Tarih | Soru |
|---|---|
| 2026-08-18 | Ekipte Scrum Master kim? (3 kez soruldu) |
| 2026-08-28 | KickOff'taki 6 sahiplik rolü (Signal, Action, Strategic Priority, A/B Test, Performance, Reporting Owner) için isimler belirlendi mi? (2 kez soruldu) |

### C. S-001 (7 soru)

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

### H. Risk, engel ve takvim (3 soru)

*Cevaplanmazsa: aktif engel tablosu ve risk tablosu boş kalır — engel/risk olmadığı için değil, teyit alınamadığı için.*

| Tarih | Soru |
|---|---|
| 2026-08-21 | EVAM'ın sprint başına 2-3 event kısıtını risk olarak kaydedeyim mi? (2 kez soruldu) |
| 2026-08-21 | PlanItEarth workshop'u yapıldı mı, yoksa 17 Eylül'de mi? (2026-08-31'de tekrar soruldu) |
| 2026-08-28 | Şu an ekibin işini durduran bir engel var mı? (2 kez soruldu) |

### I. Brifing kanalı (5 soru)

*Cevaplanmazsa: brifingin gün/saat/sıklığı varsayımla yürümeye devam eder. #7–#15 arası dokuz brifing cevapsız.*

| Tarih | Soru |
|---|---|
| 2026-08-20 | Brifingleri telefonunda bildirim olarak görüyor musun? (2 kez soruldu) |
| 2026-08-20 | Brifing saati 08:30 uygun mu, 18:00 daha mı iyi? (2 kez soruldu) |
| 2026-08-25 | Soruları cevaplamak için issue yorumu mu daha kolay, doğrudan commit mi? |
| 2026-08-27 | Brifing hafta içi her gün mü çalışsın, Pazartesi/Cuma mı kalsın? (2 kez soruldu) |
| 2026-09-03 | Cevap vermeye vaktin yoksa brifingi geçici olarak durdurayım mı? (2 kez soruldu) |

## Kapanmış maddeler

*Silmeyin, buraya taşıyın. Retro'da işe yarar.*

| # | Ne | Nasıl kapandı | Tarih |
|---|---|---|---|
| | | | |

---

*Son güncelleme: 2026-09-04*
