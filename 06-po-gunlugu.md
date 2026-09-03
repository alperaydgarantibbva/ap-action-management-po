# PO Günlüğü

Sabah brifinglerinin soru-cevap kaydı. **En yeni en üstte.**

Bu dosya asistanın hafızasıdır: dün ne konuşulduğunu buradan hatırlar, açık kalan uçları buradan takip eder.

---

## 2026-09-03 — Sabah brifingi (issue #15)

**Brifingte söylenenler:**
- Bugün Perşembe; PO haftalık ritminde paydaş güncelleme günü. `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde, bugün gerçek bir tören olup olmadığı bilinmiyor [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- Sprint 1 aktif; sprint hedefi ve bitiş tarihi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- S-001 13 gündür Taslak (2026-08-21'den beri); kabul kriterleri yazılı ama 4 açık soru (ikisi Alper'de, ikisi Umut Özdemir / Garo Üçkardeş'te) ve 2 bekleyen bağımlılık nedeniyle Definition of Ready karşılanmıyor. Backlog'daki tek story bu; bir sonraki sprinti dolduracak hazır iş yok.
- Ağustos paydaş güncellemesi gönderilmedi; Eylül'ün 3. günündeyiz, 21 paydaşın hiçbirinde "son iletişim" kaydı yok. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi, gönderim kararı Alper'de. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok [teyit edilmedi]; engel sorusu 2 kez sorulup cevaplanmadığı için takipten düştü.
- Onay beklemeden üretilen üç çıktı (5 epic, `oncelik.md` epic tablosu, paydaş taslağı) hâlâ "onaylanmadı" işaretli. Repoyu ekip görüyor.
- 17 Eylül PlanItEarth workshop'una 14 gün kaldı; repodaki tek tarihli madde bu, hazırlık kaydı yok.
- Son sekiz brifing (issue #7–#14) cevapsız — hiçbirine yorum gelmedi. Alper'in son commit'i 28 Ağustos (KickOff pptx yüklemesi).

**Sorular ve cevaplar:**
1. S: Brifingi geçici olarak durdurayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: S-001'i ikiye böleyim mi — (1) gönderim + otomatik doğrulama, (2) onay akışı + işlem geçmişi? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: S-001'in iki teknik açık sorusunu Umut Özdemir ve Garo Üçkardeş'e soracak kısa mesaj taslağını çıkarayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
4. S: 17 Eylül workshop'u için gündem taslağı çıkarayım mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 2 Eylül'de ikinci kez sorulup cevapsız kalan iki soru (S-001'in refinement'a girmesi, E-01 altına ilk story taslağı) "Cevap bekleyen sorular" tablosuna taşındı; kural gereği artık sorulmuyorlar. Tablo 27 satırda.
- `00-proje/ekip-ve-ritim.md` → "Önemli tarihler" tablosuna 17 Eylül PlanItEarth Workshop satırı yazıldı; kaynak `03-toplantilar/20260917-PlanItEarth-Workshop.md`, tarihin takvimde durup durmadığı `[teyit edilmedi]`. Gerekçe: repodaki tek tarihli madde bu ve tablo boştu; workshop'a 14 gün kaldı. Alper onaylamadı.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e cevap gelirse brifing workflow'unun tetiklenmesi durdurulacak veya sürdürülecek, karar `00-proje/kararlar.md`'ye yazılacak. 2'ye "evet" gelirse S-001 iki story'ye bölünüp `oncelik.md` sıralaması güncellenecek. 3'e "evet" gelirse `04-raporlar/` altına Umut/Garo'ya gidecek soru metni yazılacak; cevap gelince S-001'in iki teknik açık sorusu kapanacak. 4'e "evet" gelirse `03-toplantilar/20260917-PlanItEarth-Workshop.md` altına gündem taslağı eklenecek.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- 1, 2 ve 3 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 27 satırda. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-02 — Sabah brifingi (issue #14)

**Brifingte söylenenler:**
- Bugün Çarşamba; şablon tören takviminde sprint planlama günü (10:00), ama `00-proje/ekip-ve-ritim.md` hâlâ şablon değerlerinde; bugün gerçekten tören olup olmadığı bilinmiyor [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- Sprint 1 aktif; sprint hedefi ve bitiş tarihi hâlâ yazılı değil, `02-sprintler/` altında klasör yok. Yazılı sprint hedefi olmadan planlama yapılırsa kapsam savunulamaz.
- S-001 13 gündür Taslak; kabul kriterleri yazılı ama 4 açık soru (ikisi Alper'de, ikisi Umut Özdemir / Garo Üçkardeş'te) ve 2 bekleyen bağımlılık nedeniyle Definition of Ready karşılanmıyor. Backlog'daki tek story bu.
- Ağustos paydaş güncellemesi gönderilmedi; Eylül'ün 2. günündeyiz, 21 paydaşın hiçbirinde "son iletişim" kaydı yok. Aylık ritmin ilk turu kaçtı, ikincisi kaymaya başladı. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi.
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok [teyit edilmedi]; engel sorusu 2 kez sorulup cevaplanmadığı için takipten düştü.
- Onay beklemeden üretilen üç çıktı (5 epic, `oncelik.md` epic tablosu, paydaş taslağı) hâlâ "onaylanmadı" işaretli. Repoyu ekip görüyor.
- Repodaki tek tarihli madde 17 Eylül PlanItEarth workshop'u; 15 gün kaldı.
- Son yedi brifing (issue #7, #8, #9, #10, #11, #12, #13) cevapsız — hiçbirine yorum gelmedi. Alper'in son commit'i 28 Ağustos (KickOff pptx yüklemesi).

**Sorular ve cevaplar:**
1. S: S-001'i iki açık sorusu kapanmadan refinement'a sokayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: S-001'i ikiye böleyim mi — (1) gönderim + otomatik doğrulama, (2) onay akışı + işlem geçmişi?
   C: *Cevap bekleniyor*
3. S: S-001'in iki teknik açık sorusunu Umut Özdemir ve Garo Üçkardeş'e soracak kısa mesaj taslağını çıkarayım mı?
   C: *Cevap bekleniyor*
4. S: E-01 CAPTURE altına ilk story taslağını çıkarayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: Cevap vermeye vaktin yoksa brifingi geçici olarak durdurayım mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 1 Eylül'de ikinci kez sorulup cevapsız kalan iki soru (5 epic onayı, paydaş güncellemesinin gönderimi) "Cevap bekleyen sorular" tablosuna taşındı; kural gereği artık sorulmuyorlar. Tablo 25 satırda.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e cevap gelirse S-001'in durumu ve refinement gündemi netleşecek. 2'ye "evet" gelirse S-001 iki story'ye bölünüp `oncelik.md` sıralaması güncellenecek. 3'e "evet" gelirse `04-raporlar/` altına Umut/Garo'ya gidecek soru metni yazılacak; cevap gelince S-001'in iki teknik açık sorusu kapanacak. 4'e "evet" gelirse `01-backlog/stories/` altına E-01 için ilk story taslağı açılacak. 5'e cevap gelirse workflow tetikleme kararı ve `00-proje/kararlar.md` güncellenecek.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1 ve 4 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 25 satırda. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen üç çıktı hâlâ "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-01 — Sabah brifingi (issue #13)

**Brifingte söylenenler:**
- Bugün Salı; hafta ve ay değişti. Şablondaki tören takvimine göre Salı refinement günü, ama `00-proje/ekip-ve-ritim.md` hâlâ şablon değerlerinde; bugün tören olup olmadığı bilinmiyor [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- Sprint 1 aktif; bitiş tarihi ve sprint hedefi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- S-001 11 gündür Taslak; kabul kriterleri yazılı ama 4 açık soru (ikisi Alper'de) ve 2 bekleyen bağımlılık nedeniyle Definition of Ready karşılanmıyor. Backlog'daki tek story bu.
- Ağustos kapandı ve 21 paydaşa gidecek ilk aylık güncelleme gönderilmedi; aylık ritmin ilk turu kaçırıldı. Taslak 31 Ağustos'ta yazıldı, `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderim kararı Alper'de.
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok [teyit edilmedi]; engel sorusu 2 kez sorulup cevaplanmadığı için takipten düştü.
- 31 Ağustos'ta onay beklemeden üretilen üç çıktı (5 epic, `oncelik.md` epic tablosu, paydaş taslağı) "onaylanmadı" işaretiyle duruyor.
- Repodaki tek tarihli madde 17 Eylül PlanItEarth workshop'u; 16 gün kaldı.
- Son altı brifing (issue #7, #8, #9, #10, #11, #12) cevapsız — hiçbirine yorum gelmedi. Alper'in son commit'i 28 Ağustos (KickOff pptx yüklemesi).

**Sorular ve cevaplar:**
1. S: Açılan 5 epic (E-01…E-05) bu haliyle onaylanıyor mu? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: Paydaş güncellemesi Eylül'ün ilk haftasında gönderilecek mi? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: S-001'i iki açık sorusu kapanmadan refinement'a sokayım mı?
   C: *Cevap bekleniyor*
4. S: E-01 CAPTURE altına ilk story taslağını çıkarayım mı?
   C: *Cevap bekleniyor*
5. S: Brifing hafta içi her gün mü çalışsın, haftada tek özet mi?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 31 Ağustos'ta üçüncü/ikinci kez sorulup cevapsız kalan üç soru (17 Eylül workshop, haftanın tek hedefi, 6 sahiplik rolü isimleri) "Cevap bekleyen sorular" tablosunda kapatıldı; kural gereği artık sorulmuyorlar. Tablo 23 satırda.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse epic'lerin durumu "Fikir"den ilerletilecek ve `oncelik.md` sıralaması onaylı hale gelecek. 2'ye "evet" gelirse taslak Eylül başlığıyla güncellenip `paydaslar.md`'deki 21 satırın "son iletişim" sütunu doldurulacak ve aylık sayaç başlatılacak. 3'e cevap gelirse S-001'in durumu ve refinement gündemi netleşecek. 4'e "evet" gelirse `01-backlog/stories/` altına E-01 için ilk story taslağı açılacak. 5'e cevap gelirse workflow tetikleme günü ve `00-proje/kararlar.md` güncellenecek.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1 ve 2 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 23 satırda. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Aylık paydaş bilgilendirmesinin ilk turu (Ağustos) kaçırıldı; taslak hazır, gönderim Alper'de.
- Onay beklemeden üretilen üç çıktı hâlâ "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-08-31 — Sabah brifingi (issue #12)

**Brifingte söylenenler:**
- Bugün Pazartesi: 20 Ağustos kararına göre planlı brifing günü; PO haftalık ritminde haftanın önceliğini belirleme ve backlog sıralamasını gözden geçirme günü.
- Tören takvimi `00-proje/ekip-ve-ritim.md`'de hâlâ şablon değerlerinde; bugün tören olup olmadığı bilinmiyor [teyit edilmedi]. Bu soru 3 kez sorulduğu için artık sorulmuyor.
- Sprint 1 aktif; bitiş tarihi ve sprint hedefi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- S-001 10 gündür Taslak; Alper'e ait 2 açık soru (geliştirme tarafı, manuel SQL yolunun kapatılması) nedeniyle Definition of Ready karşılanmıyor.
- 21 paydaşın tamamında "son iletişim" sütunu boş; aylık bilgilendirme ritmi 10 gündür başlamadı ve yarın ay değişiyor.
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok [teyit edilmedi]; engel sorusu 2 kez sorulup cevaplanmadığı için bekleyen sorular tablosuna taşındı.
- Repodaki tek tarihli madde 17 Eylül PlanItEarth workshop'u; 17 gün kaldı.
- Son beş brifing (issue #7, #8, #9, #10, #11) cevapsız. Alper'in son commit'i 28 Ağustos 19:18 (KickOff pptx yüklemesi); o dosyanın metin özeti 28 Ağustos brifinginde çıkarılmıştı, yeni bilgi gelmedi.
- Kapsam belgelerde büyümeye devam ediyordu, backlog'da değil: KickOff'un 5 katmanı, Action Engine README'nin 5 başlığı ve vizyonun 6 başarı kriteri backlog'da karşılıksızdı. Bu tur kapatıldı (aşağıya bak).

**Sorular ve cevaplar:**
1. S: Açılan 5 epic (E-01…E-05) bu haliyle onaylanıyor mu?
   C: *Cevap bekleniyor*
2. S: Bu haftanın tek hedefi S-001'i "Hazır" duruma getirmek olsun mu?
   C: *Cevap bekleniyor*
3. S: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` bu haliyle gönderilebilir mi?
   C: *Cevap bekleniyor*
4. S: 17 Eylül PlanItEarth workshop'u takvimde hâlâ duruyor mu?
   C: *Cevap bekleniyor*
5. S: 6 sahiplik rolü için isimler belirlendi mi? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `01-backlog/epics/` → KickOff sunumunun 5 katmanından 5 epic taslağı açıldı: E-01 CAPTURE, E-02 TRANSFORM (S-001 bu epic'in altında), E-03 PRIORITIZE, E-04 ACTIVATE, E-05 MONITOR. Her epic vizyondaki bir başarı kriterine bağlandı; kaynak, risk ve açık karar satırları belgelerden alındı, yorum gerektiren yerler `[teyit edilmedi]` işaretlendi. Gerekçe: bu teklif 24, 25, 26 ve 28 Ağustos'ta 4 kez yapıldı, cevap gelmedi; sormaya devam etmek yerine taslak çıkarıldı. Alper onaylamadı.
- `01-backlog/oncelik.md` → "Epic yapısı" tablosu eklendi; 5 epic ile vizyon başarı kriterleri eşleştirildi. Sıra, KickOff'taki katman akışı — değer sırası değil, onaylanmadı.
- `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` → 21 paydaşa gidecek ilk aylık güncelleme taslağı yazıldı. Gerekçe: 27 ve 28 Ağustos'ta 2 kez teklif edildi, cevap gelmedi; kural gereği üçüncü kez sorulmuyor. Taslak yalnızca repodaki belgelerden yazıldı, Jira'daki gerçek ilerleme yok — bu sınır dosyanın sonunda yazılı. **Gönderilmedi**, gönderim Alper'de.
- `05-riskler-engeller.md` → 28 Ağustos'ta ikinci kez sorulup cevapsız kalan 2 soru (aktif engel var mı, paydaş güncelleme taslağı) "Cevap bekleyen sorular" tablosuna taşındı; tablo 22 satıra çıktı.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse epic'lerin durumu "Fikir"den ilerletilecek ve `oncelik.md` sıralaması onaylı hale gelecek; "hayır" gelirse taslaklar Alper'in tarifine göre yeniden yazılacak. 2'ye cevap gelirse haftanın hedefi `06-po-gunlugu.md` ve aktif sprint kaydına yazılacak. 3'e "evet" gelirse `paydaslar.md`'deki 21 satırın "son iletişim" sütunu doldurulup aylık sayaç başlatılacak. 4'e cevap gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna yazılacak. 5'e isimler gelirse `ekip-ve-ritim.md` ekip tablosu ve 5 epic'in "Sahip" satırı doldurulacak, S-001'in onay adımı netleşecek.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 5 numaralı soru ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 22 satırda. Sprint tarihleri, sprint hedefi, tören takvimi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen üç çıktı (5 epic, epic tablosu, paydaş taslağı) "onaylanmadı" işaretli duruyor. Alper reddederse geri alınacak.
- Aylık paydaş bilgilendirmesi Ağustos içinde gönderilmezse ilk tur kaçırılmış olacak; taslak hazır, karar Alper'de.

---

## 2026-08-28 — Sabah brifingi (issue #11)

**Brifingte söylenenler:**
- Bugün Cuma: 20 Ağustos kararına göre planlı brifing günü ve hafta kapanışı (riskler güncellenir, paydaş ihtiyacına bakılır).
- Alper bugün `00-proje/ActionPlanning-ActionManagement-KickOff-202709.pptx` dosyasını yükledi (16 slayt). Sunum "Step 1: Action Management" modülünü 5 katman (Capture, Transform, Prioritize, Activate, Monitor), 4 engine, 4 havuz ve 6 sahiplik rolü olarak tarif ediyor. 24 Ağustos'ta eklenen Action Engine README'nin 5 fonksiyonel başlığı ve vizyondaki 6 başarı kriteri ile örtüşüyor.
- Sunumdaki TRANSFORM katmanı S-001 ile birebir örtüşüyor: "SQL'ler Action Owner tarafından hazırlanır → sistemsel olarak kontrol edilip onaylanır → periyodik çalışacak şekilde planlanır → Action Library'ye kaydedilir."
- Kapsam belgelerde büyüyor, backlog'da değil: backlog'da hâlâ tek story var (S-001), epic yok.
- S-001 7 gündür Taslak; Alper'e ait 2 açık soru nedeniyle Definition of Ready karşılanmıyor.
- Sprint 1 aktif; bitiş tarihi ve sprint hedefi hâlâ yazılı değil, `02-sprintler/` altında klasör yok. Bu soru 3 kez sorulduğu için artık sorulmuyor.
- Tören takvimi `00-proje/ekip-ve-ritim.md`'de hâlâ şablon değerlerinde; bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok [teyit edilmedi]; 21 paydaşın tamamında "son iletişim" sütunu boş.
- Son dört brifing (issue #7, #8, #9, #10) cevapsız.

**Sorular ve cevaplar:**
1. S: Şu an ekibin işini durduran bir engel var mı? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: KickOff sunumundaki 5 katmandan 5 epic taslağı çıkarayım mı?
   C: *Cevap bekleniyor*
3. S: Sunumdaki 6 sahiplik rolü (Signal, Action, Strategic Priority, A/B Test, Performance, Reporting Owner) için isimler belirlendi mi?
   C: *Cevap bekleniyor*
4. S: 21 paydaşa gidecek ilk aylık güncelleme taslağını çıkarayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: Dosya adındaki "202709" kickoff tarihi mi?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `00-proje/kickoff-ozeti.md` → KickOff sunumunun metni çıkarıldı. Gerekçe: pptx binary olduğu için repoda aranamıyor ve story yazarken referans verilemiyordu. Sunumdaki ifadeler korundu, yorum gerektiren yerler `[teyit edilmedi]` işaretlendi. Alper onaylamadı.
- `05-riskler-engeller.md` → 27 Ağustos'ta ikinci kez sorulup cevapsız kalan 3 soru (brifing günleri, Action Engine prototipinin kapsamı, manuel SQL yolunun kapatılması) "Cevap bekleyen sorular" tablosuna taşındı; kural gereği üçüncü kez sorulmuyorlar.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e cevap gelirse `05-riskler-engeller.md` aktif engel tablosu (engel yoksa tarihli "engel yok" notu) yazılacak; 2'ye "evet" gelirse `01-backlog/epics/` altına 5 epic taslağı açılacak ve `01-backlog/oncelik.md` güncellenecek; 3'e cevap gelirse `00-proje/ekip-ve-ritim.md` ekip tablosu ve S-001'in onay adımı netleşecek; 4'e "evet" gelirse `04-raporlar/` altına aylık paydaş güncelleme taslağı açılacak; 5'e tarih gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna yazılacak.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1 ve 4 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 18 satıra çıktı. Bunlar cevaplanmadıkça sprint tarihleri, sprint hedefi, epic yapısı ve S-001'in "Hazır" durumu ilerlemiyor.
- Hafta kapanışı tamamlanmadı: engel durumu teyit edilmedi, paydaş bilgilendirme sayacı başlamadı.

---

## 2026-08-27 — Sabah brifingi (issue #10)

**Brifingte söylenenler:**
- Bugün Perşembe. 20 Ağustos kararına göre brifing günleri Pazartesi ve Cuma; workflow hafta içi her gün tetiklendiği için bu tur da plan dışı çalıştı. Yarın (28 Ağustos, Cuma) planlı brifing günü.
- PO haftalık ritminde Perşembe paydaş güncellemesi günü; `paydaslar.md` dolu olduğu için ilk aylık güncelleme taslağı çıkarılabilir durumda.
- Tören takvimi `00-proje/ekip-ve-ritim.md`'de hâlâ şablon değerlerinde; bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- Sprint 1 aktif; bitiş tarihi ve sprint hedefi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- S-001 6 gündür Taslak; kabul kriterleri yazılı ama 4 açık soru ve 2 bekleyen bağımlılık nedeniyle Definition of Ready karşılanmıyor. Açık soruların ikisinin muhatabı Alper.
- 21 paydaşın tamamında "son iletişim" sütunu boş; bilgilendirme sayacı hâlâ başlamadı.
- 24 Ağustos'ta eklenen Action Engine README'deki 5 fonksiyonel başlığın backlog'da hâlâ karşılığı yok; kapsam backlog dışında büyüyor.
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok [teyit edilmedi].
- Son üç brifing (issue #7, #8, #9) cevapsız; Alper'in son commit'i 24 Ağustos 19:01.

**Sorular ve cevaplar:**
1. S: Brifing hafta içi her gün mü çalışsın, Pazartesi/Cuma mı kalsın? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: Şu an ekibin işini durduran bir engel var mı?
   C: *Cevap bekleniyor*
3. S: 21 paydaşa gidecek ilk aylık güncelleme taslağını bugün çıkarayım mı?
   C: *Cevap bekleniyor*
4. S: Action Engine prototipi ekibin geliştirme kapsamında mı, yoksa hizalanma amaçlı ayrı bir çalışma mı? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: Ortak klasöre manuel SQL bırakma yolu S-001 ile kapatılacak mı, bir süre paralel mi yürüyecek? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `00-proje/paydaslar.md` → Tekrar eden iki satır (Haluk Bekmez, Özgül Aslan) silindi; liste 23'ten 21 kayda indi. Üç brifingtir teklif edilip cevap gelmemişti; veri tekrarı olduğu için düzeltildi.
- `05-riskler-engeller.md` → 24, 25 ve 26 Ağustos'ta ikinci kez sorulup cevapsız kalan sorular ile daha önce sorulup takipten düşen sorular "Cevap bekleyen sorular" tablosuna taşındı (11 satır eklendi).

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e cevap gelirse workflow tetikleme günü ve `00-proje/kararlar.md` güncellenecek; 2'ye cevap gelirse `05-riskler-engeller.md` aktif engel tablosu (engel yoksa tarihli "engel yok" notu) yazılacak; 3'e "evet" gelirse `04-raporlar/` altına aylık paydaş güncelleme taslağı açılacak; 4'e cevap gelirse Action Engine başlıklarının backlog'a girip girmeyeceği netleşecek; 5'e cevap gelirse S-001'in Alper'e ait bir açık sorusu kapanacak.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1, 4 ve 5 numaralı sorular ikinci kez soruldu; yarınki brifingte cevap gelmezse üçüncü kez sorulmayacak ve `05-riskler-engeller.md` tablosuna taşınacak.
- Kural gereği artık sorulmayan 8 soru bekleyen sorular tablosunda; bunlar cevaplanmadıkça sprint tarihleri, sprint hedefi, epic yapısı ve S-001'in "Hazır" durumu ilerlemiyor.
- Yarın Cuma: hafta kapanışı. Riskler/engeller güncellemesi ve paydaş güncellemesi ihtiyacı gündeme gelecek.

---

## 2026-08-26 — Sabah brifingi (issue #9)

**Brifingte söylenenler:**
- Bugün Çarşamba. Brifing ritmi Alper'in 20 Ağustos kararı gereği Pazartesi ve Cuma; workflow hafta içi her gün tetiklendiği için dün ve bugün plan dışı çalıştı.
- Tören takvimi `00-proje/ekip-ve-ritim.md`'de hâlâ şablon değerlerinde; bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- Sprint 1 aktif; bitiş tarihi ve sprint hedefi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- Backlog'da tek story var: S-001, 5 gündür Taslak. Alper'e ait 2 açık sorusu kapanmadığı için Definition of Ready karşılanmıyor.
- 24 Ağustos'ta eklenen Action Engine README'deki 5 fonksiyonel başlığın backlog'da hâlâ karşılığı yok; kapsam backlog dışında büyüyor.
- 23 paydaşın tamamında "son iletişim" sütunu boş; `paydaslar.md`'de iki satır tekrar ediyor (Haluk Bekmez, Özgül Aslan).
- `05-riskler-engeller.md` hâlâ şablon; kayıtlı aktif engel yok [teyit edilmedi].
- `03-toplantilar/20260824-tasarim.md` yalnızca görsel içeriyor, toplantı kararları yazılı değil.
- Dünkü (25 Ağustos) 5 sorunun tamamı cevapsız; issue #8 yorumsuz. Alper'in son commit'i 24 Ağustos akşamı.

**Sorular ve cevaplar:**
1. S: Action Engine README'deki 5 başlıktan epic taslaklarını çıkarayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: S-001'deki iş Account Planning tarafında mı, GT Pusula tarafında mı geliştirilecek? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: Ortak klasöre manuel SQL bırakma yolu S-001 ile kapatılacak mı, bir süre paralel mi yürüyecek?
   C: *Cevap bekleniyor*
4. S: Brifing hafta içi her gün mü çalışsın, yoksa Pazartesi/Cuma mı kalsın?
   C: *Cevap bekleniyor*
5. S: accountplanning.ai üzerinde yayınlanacak prototip için hedef tarih var mı? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- Henüz yok — cevap bekleniyor. 1'e "evet" gelirse `01-backlog/epics/` altına 5 epic taslağı açılacak; 2 ve 3'e cevap gelirse S-001'in Alper'e ait iki açık sorusu kapanacak; 4'e cevap gelirse workflow tetikleme günü ve `00-proje/kararlar.md` güncellenecek; 5'e tarih gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna yazılacak.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1, 2 ve 5 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve `05-riskler-engeller.md` içindeki "Cevap bekleyen sorular" tablosuna taşınacak.
- 25 Ağustos'ta sorulan "Action Engine prototipi ekibin geliştirme kapsamında mı?" ve "Soruları cevaplamak için issue yorumu mu, commit mi?" soruları bu turda 5 soru sınırına girmediği için sorulmadı.
- 24 Ağustos'ta sorulan 5 soru (Sprint 1 bitiş tarihi, S-001 onayı, haftanın hedefi, vizyondan epic taslakları, EVAM kısıtı + maintenance sahipliği) üçüncü kez sorulmama kuralı gereği sorulmuyor; `05-riskler-engeller.md` "Cevap bekleyen sorular" tablosuna taşınmaları gerekiyor.
- Teklif edilen ve onay bekleyen iki asistan aksiyonu: `paydaslar.md`'deki tekrar eden iki satırın silinmesi, 20 Ağustos brifing ritmi kararının `kararlar.md`'ye K-002 olarak yazılması.

---

## 2026-08-25 — Sabah brifingi (issue #8)

**Brifingte söylenenler:**
- Bugün Salı. Brifing ritmi Alper'in 20 Ağustos kararı gereği Pazartesi ve Cuma; bu tur plan dışı çalıştı [teyit edilmedi].
- Dün akşam Alper iki commit attı: `91-prototyping/01-action-engine/README.md` (Action Engine prototip tanımı; 5 fonksiyonel başlık: sinyal yönetimi, aksiyon yönetimi, skorlama, A/B testing, gerçekleşen ve etki takibi) ve `03-toplantilar/20260824-tasarim.md` (yalnızca veri modeli görseli, metin yok).
- Action Engine tanımının backlog'da karşılığı yok; backlog'da hâlâ tek story var (S-001).
- S-001 hâlâ Taslak: 4 açık soru ve 2 bekleyen bağımlılık nedeniyle Definition of Ready karşılanmıyor. Açık soruların ikisinin muhatabı Alper.
- Tören takvimi `00-proje/ekip-ve-ritim.md`'de hâlâ şablon değerlerinde; bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- Sprint 1 aktif; bitiş tarihi ve sprint hedefi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- `00-proje/paydaslar.md`'de iki satır tekrar ediyor (Haluk Bekmez, Özgül Aslan); 23 paydaşın tamamında "son iletişim" sütunu boş.
- Dünkü (24 Ağustos) 5 sorunun tamamı cevapsız; issue #7 yorumsuz.

**Sorular ve cevaplar:**
1. S: Action Engine README'deki 5 fonksiyonel başlıktan epic taslaklarını çıkarayım mı?
   C: *Cevap bekleniyor*
2. S: S-001'deki iş Account Planning tarafında mı, GT Pusula tarafında mı geliştirilecek?
   C: *Cevap bekleniyor*
3. S: Action Engine prototipi ekibin geliştirme kapsamında mı, yoksa hizalanma amaçlı ayrı bir çalışma mı?
   C: *Cevap bekleniyor*
4. S: accountplanning.ai üzerinde yayınlanacak prototip için hedef tarih var mı?
   C: *Cevap bekleniyor*
5. S: Soruları cevaplamak için issue yorumu mu daha kolay, doğrudan commit mi?
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- Henüz yok — cevap bekleniyor. 1'e "evet" gelirse `01-backlog/epics/` altına 5 epic taslağı açılacak; 2'ye cevap gelirse S-001'in açık sorusu kapanacak; 3 ve 4'e cevap gelirse `01-backlog/oncelik.md` ve `00-proje/ekip-ve-ritim.md` güncellenecek.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 24 Ağustos'ta sorulan 5 soru (Sprint 1 bitiş tarihi, S-001 onayı, haftanın hedefi, vizyondan epic taslakları, EVAM kısıtı + maintenance sahipliği) bu turda tekrarlanmadı; ikinci kez sorulmuşlardı ve üçüncü kez sorulmama kuralına takılıyorlar. Bir sonraki planlı brifingte (Cuma, 28 Ağustos) sorulmayacak, `05-riskler-engeller.md` içindeki "Cevap bekleyen sorular" tablosuna taşınacaklar.
- Teklif edilen ve cevap bekleyen üç aksiyon: 5 epic taslağının çıkarılması, S-001 kabul kriterlerine "en fazla 2 milyon satır" limitinin eklenmesi (README 3.3'te geçiyor, story'de yok), `paydaslar.md`'deki iki tekrar satırının silinmesi.
- `20260824-tasarim.md` yalnızca görsel içeriyor; toplantı kararları yazılı değil.

---

## 2026-08-24 — Sabah brifingi (issue #7)

**Brifingte söylenenler:**
- Bugün Pazartesi; brifingler Alper'in 20 Ağustos kararı gereği Pazartesi ve Cuma günleri yapılıyor.
- Tören takvimi hâlâ şablon değerlerinde; bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- Sprint 1 aktif, ancak bitiş tarihi yazılı değil ve `02-sprintler/` altında klasör yok. Sprint hedefi de yazılmamış.
- Cuma sorulan 5 sorunun tamamı cevapsız; issue #6'ya yorum gelmedi.
- Cuma akşamı (21 Ağustos 17:47) Alper `00-proje/paydaslar.md`'ye 3 satır ekledi; liste 23 kayda çıktı. İki satır tekrarlı: Haluk Bekmez ve Özgül Aslan ikişer kez yazılmış.
- 23 paydaşın tamamı "Aylık" bilgilendirme işaretli ama "son iletişim" sütunu boş; sayaç hâlâ başlamadı.
- Backlog'da tek story var: S-001, Taslak. Kabul kriterleri yazılı ama 4 açık soru ve 2 bekleyen bağımlılık nedeniyle Definition of Ready karşılanmıyor.
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok — engel olmadığı için değil, henüz girilmediği için [teyit edilmedi].

**Sorular ve cevaplar:**
1. S: Sprint 1 hangi tarihte bitiyor? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: S-001 doğru konuyu tarif ediyor mu, bu haliyle ekibe gösterilebilir mi? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: Bu haftanın tek hedefi S-001'i "Hazır" duruma getirmek olsun mu?
   C: *Cevap bekleniyor*
4. S: Vizyondaki 6 başarı kriterinden epic taslaklarını çıkarayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: EVAM'ın sprint başına 2-3 event kısıtını risk, Account Planning maintenance süreç sahipliğini bekleyen karar olarak kaydedeyim mi? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- Henüz yok — cevap bekleniyor. 1'e tarih gelirse `00-proje/ekip-ve-ritim.md` ve `02-sprintler/sprint-01/` açılacak; 5'e "evet" gelirse `05-riskler-engeller.md` güncellenecek.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1, 2, 4 ve 5 numaralı sorular ikinci kez soruldu; Cuma da cevap gelmezse üçüncü kez sorulmayacak ve `05-riskler-engeller.md` içindeki "Cevap bekleyen sorular" tablosuna taşınacak.
- Cuma sorulan "PlanItEarth workshop'u yapıldı mı, yoksa 17 Eylül'de mi?" sorusu bu turda 5 soru sınırına girmediği için sorulmadı; bir sonraki brifingte tekrar sorulacak.
- Teklif edilen ve cevap bekleyen üç aksiyon: S-001'in Alper'e ait 2 açık sorusunun cevabı, sprint-01 klasörü + sprint hedefi taslağı, `paydaslar.md`'deki tekrar eden iki satırın silinmesi.
- Alper cevaplarını issue yorumu yerine doğrudan commit ile veriyor; bu tur da aynı olabilir.

---

## 2026-08-21 — Sabah brifingi (issue #6)

**Brifingte söylenenler:**
- Bugün Cuma; Alper'in 20 Ağustos kararı gereği brifingler Pazartesi ve Cuma günleri yapılıyor.
- Alper cevaplarını issue yorumu olarak değil, doğrudan commit ile verdi: `00-proje/paydaslar.md` 21 paydaşla dolduruldu, `03-toplantilar/` altına iki toplantı notu eklendi (19 Ağustos Pusula II, PlanItEarth Workshop).
- Sprint 1 aktif olarak teyit edildi, ancak `02-sprintler/` altında klasör yok; sprint hedefi, tarihler ve review günü hâlâ yazılı değil.
- Tören takvimi hâlâ şablon değerlerinde, bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- 21 paydaşın tamamı "Aylık" bilgilendirme olarak işaretli ama "son iletişim" sütunu boş; sayaç başlamadı.

**Bu brifingte asistanın ürettikleri:**
- `01-backlog/stories/S-001-aksiyon-sql-tanimi-sistem-uzerinden.md` → Alper'in 20 Ağustos'ta istediği ilk story taslağı yazıldı. Kaynak: iki toplantı notu. Durum: Taslak, onay bekliyor.
- `01-backlog/oncelik.md` → S-001 tek kayıt olduğu için 1. sıraya yazıldı; sıralama Alper tarafından onaylanmadı.

**Sorular ve cevaplar:**
1. S: Sprint 1 hangi tarihte bitiyor?
   C: *Cevap bekleniyor*
2. S: S-001 doğru konuyu mu tarif ediyor?
   C: *Cevap bekleniyor*
3. S: EVAM'ın sprint başına 2-3 event kısıtını risk olarak kaydedeyim mi?
   C: *Cevap bekleniyor*
4. S: "Account Planning maintenance süreç sahipliği" konusunu bekleyen karar olarak kaydedeyim mi?
   C: *Cevap bekleniyor*
5. S: PlanItEarth workshop'u yapıldı mı, yoksa 17 Eylül'de mi?
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- Henüz yok — cevap bekleniyor. 3 ve 4 numaralı sorulara "evet" gelirse `05-riskler-engeller.md` güncellenecek.

**Brifingten sonra gelen:**
- Alper 08:57'de `00-proje/vizyon.md`'yi doldurdu. Bu sürümün hedefi yazılı hale geldi: Aksiyon Yönetim Yapısı ve tekil aksiyon havuzu. 6 başarı kriteri tanımlandı, kapsam dışı iki madde net (yapay zeka eklentileri; Ana Banka / Müşteri Yolculuğu / Ürün Performansları / Müşteri Memnuniyeti modülleri).
- Issue #6'ya ek not yazıldı: başarı kriterlerinin epic adayı olduğu, S-001'in bu hedefin içinde kaldığı, vizyon dosyasının "Taslak" başlığının güncellenmesi gerektiği.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1 numaralı soru (sprint tarihi) daha önce 3 kez sorulup bekleyen sorular tablosuna taşınmıştı; Sprint 1'in aktif olduğu teyit edildiği için bitiş tarihi olarak daraltılıp yeniden soruldu.
- Vizyon başarı kriterlerinden epic taslakları çıkarılsın mı — Alper'in onayı bekleniyor.
- S-001 içindeki 4 açık soru story dosyasında duruyor; refinement'a girmeden önce kapanmalı.

---

## 2026-08-20 — Sabah brifingi (issue #5)

**Brifingte söylenenler:**
- Bugün Perşembe. Tören takvimi şablon halinde olduğu için bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- PO haftalık ritmine göre Perşembe paydaş güncellemesi günü, ancak `00-proje/paydaslar.md` boş olduğu için taslak üretilemedi.
- Beş iş günü üst üste (16, 17, 18, 19, 20 Ağustos) brifinglere cevap gelmedi; issue #1, #2, #3, #4 yorumsuz açık.
- Repo hâlâ veri içermiyor: aktif sprint, story, backlog sıralaması ve paydaş listesi girilmemiş. Bu yüzden engel/kabul kriteri/paydaş uyarısı üretilemiyor.
- "Bildirim görüyor musun?" ve "08:30 uygun mu?" soruları üçüncü kez sorulmadı; kural gereği bekleyen sorular tablosuna taşındı.

**Sorular ve cevaplar:**
1. S: Proje şu an aktif bir sprint içinde mi? (ikinci kez)
   C: evet, spring 1
2. S: Günlük brifing yerine sadece Pazartesi brifing yapalım mı? (ikinci kez)
   C: Pazartesi ve Cuma olsun
3. S: Brifingleri "devam" denene kadar duraklatayım mı?
   C: her pazartesi ve cuma
4. S: Tek cümlelik bir iş tarifi verirsen ilk story taslağını asistan yazsın mı?
   C: evet yazsın. İş tarifi: kapsamın çalışmalarının tamamlanması

**Bu cevaplardan çıkan güncellemeler:**
- `05-riskler-engeller.md` → "Bu brifingleri telefonunda bildirim olarak görüyor musun?" ve "Brifing saati 08:30 uygun mu?" soruları 2 kez sorulup cevaplanmadığı için üçüncü kez sorulmadı, "Cevap bekleyen sorular" tablosuna taşındı.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- 1 ve 2 numaralı sorular ikinci kez soruldu; yarın da cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Cevapsızlığın nedeni hâlâ bilinmiyor [teyit edilmedi]. 3 numaralı soru bu belirsizliği kapatmak için soruldu.

---

## 2026-08-19 — Sabah brifingi (issue #4)

**Brifingte söylenenler:**
- Bugün Çarşamba. `ekip-ve-ritim.md`'deki "Sprint Planlama Çarşamba 10:00" satırı şablon örneği olduğu için bugün tören olup olmadığı bilinmiyor [teyit edilmedi].
- Repo hâlâ veri içermiyor: aktif sprint, story, backlog sıralaması, paydaş listesi girilmemiş. Backlog'da tek story olmadığı için kabul kriteri uyarısı üretilemiyor.
- Dört gün üst üste (16, 17, 18, 19 Ağustos) brifinglere cevap gelmedi; issue #1, #2, #3 yorumsuz açık.
- Cevapsızlığın nedeni bilinmiyor: bildirim ulaşmıyor olabilir, saat uygun olmayabilir ya da günlük ritim fazla olabilir [teyit edilmedi]. Üç olasılık ayrı ayrı soruldu.
- Kurulumdan gelen 4 temel soru (sprint, tören takvimi, Scrum Master, proje tanımı) 3 kez sorulduğu için tekrar sorulmadı; `05-riskler-engeller.md`'de bekliyor.

**Sorular ve cevaplar:**
1. S: Bu brifingleri telefonunda bildirim olarak görüyor musun? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: Bugün 10:00'da sprint planlama var mı?
   C: *Cevap bekleniyor*
3. S: Proje şu an aktif bir sprint içinde mi, yoksa henüz başlamadı mı?
   C: *Cevap bekleniyor*
4. S: Brifing saati 08:30 uygun mu, yoksa 18:00 daha iyi olur mu? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: Günlük yerine sadece Pazartesi brifing yapalım mı?
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- `05-riskler-engeller.md` → "Bu hafta ekibin bitirmesini en çok istediğin tek iş ne?" sorusu 2 kez sorulup cevaplanmadığı için üçüncü kez sorulmadı, "Cevap bekleyen sorular" tablosuna taşındı.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1 ve 4 numaralı sorular ikinci kez soruldu; yarın da cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.

---

## 2026-08-18 — Sabah brifingi (issue #3)

**Brifingte söylenenler:**
- Bugün Salı. Tören takvimi şablon halinde olduğu için bugün tören olup olmadığı bilinmiyor; dosyadaki "Refinement Salı 14:00" satırı örnek değer, gerçek değil [teyit edilmedi].
- Repo hâlâ boş: sprint bilgisi, story, backlog sıralaması ve paydaş listesi girilmemiş.
- Üç gün üst üste (16, 17, 18 Ağustos) brifinglere cevap gelmedi; issue #1 ve #2 yorumsuz açık duruyor.
- Kurulumdan beri sorulan 4 soru (sprint tarihleri, tören takvimi, Scrum Master, projenin tanımı) üçüncü güne girdi. Kural gereği bir daha sorulmadı, `05-riskler-engeller.md` içindeki "Cevap bekleyen sorular" tablosuna taşındı.
- Aktif engel, risk, kabul kriteri boş story ve cevapsız paydaş sorusu kaydı yok — çünkü henüz kayıt girilmemiş.

**Sorular ve cevaplar:**
1. S: Bu brifingleri telefonunda bildirim olarak görüyor musun?
   C: *Cevap bekleniyor*
2. S: Bugün 14:00'te refinement var mı?
   C: *Cevap bekleniyor*
3. S: Bu hafta ekibin bitirmesini en çok istediğin tek iş ne? (ikinci kez)
   C: *Cevap bekleniyor*
4. S: Brifing saati 08:30 sana uygun mu?
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- `05-riskler-engeller.md` → üç kez sorulup cevaplanmayan 4 kurulum sorusu "Cevap bekleyen sorular" tablosuna taşındı.
- Issue #3'e tek yorumda doldurulabilecek sprint/tören/ekip bilgi şablonu eklendi.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- Cevap gelmemesinin nedeni bilinmiyor: bildirim ulaşmıyor olabilir ya da saat uygun olmayabilir [teyit edilmedi].

---

## 2026-08-17 — Sabah brifingi (issue #2)

**Brifingte söylenenler:**
- Repo hâlâ şablon halinde: `vizyon.md`, `ekip-ve-ritim.md`, `paydaslar.md`, `oncelik.md` boş; aktif sprint klasörü ve story yok.
- Bugün Pazartesi. Takvimde tören görünmüyor, ancak bunun nedeni tören takviminin boş olması — gerçek durum [teyit edilmedi].
- Aktif engel, risk ve cevapsız paydaş sorusu kaydı yok.
- Issue #1 İstanbul saatiyle 00:13'te açıldığı için gözden kaçmış olabilir; 5 soru cevapsız kaldı.

**Sorular ve cevaplar:**
1. S: Aktif sprint numarası ve bitiş tarihi ne?
   C: *Cevap bekleniyor*
2. S: Bu hafta refinement veya review var mı, hangi gün?
   C: *Cevap bekleniyor*
3. S: Ekipte Scrum Master kim?
   C: *Cevap bekleniyor*
4. S: ap-action-management neyi yönetiyor — tek cümle?
   C: *Cevap bekleniyor*
5. S: Bu hafta ekibin bitirmesini en çok istediğin tek iş ne?
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- Yok — cevap bekleniyor.

**Açık kalanlar:**
- 5 sorunun tamamı. 1-4 numaralı sorular ikinci kez soruldu; bugün de cevap gelmezse üçüncü kez sorulmayacak ve `05-riskler-engeller.md` içindeki "Cevap bekleyen sorular" tablosuna taşınacak.
- 5. soru (bu haftanın önceliği) Pazartesi ritmi gereği ilk kez soruldu.

---

## 2026-08-16 — Sabah brifingi (issue #1)

**Brifingte söylenenler:**
- İlk gerçek brifing. Repo şablon halinde: `vizyon.md`, `ekip-ve-ritim.md`, `paydaslar.md`, `oncelik.md` boş; aktif sprint klasörü yok.
- Aktif engel, kabul kriteri bekleyen story ve cevapsız paydaş sorusu yok.
- Bugün Pazar; brifing hafta içi 08:30 için kurulmuş olmasına rağmen hafta sonu çalıştı — Alper'e bildirildi.

**Sorular ve cevaplar:**
1. S: Aktif sprint hangisi ve bitiş tarihi ne?
   C: *Cevap bekleniyor*
2. S: Refinement hangi gün ve saatte?
   C: *Cevap bekleniyor*
3. S: Sprint planlama ve review hangi gün?
   C: *Cevap bekleniyor*
4. S: Ekipte Scrum Master kim?
   C: *Cevap bekleniyor*
5. S: ap-action-management tek cümleyle neyi yönetiyor?
   C: *Cevap bekleniyor*

**Bu cevaplardan çıkan güncellemeler:**
- Yok — cevap gelmedi.

**Açık kalanlar:**
- 5 sorunun tamamı. Bunlar kurulum kaydından ikinci kez soruluyor; üçüncü kez sorulmayacak, cevap gelmezse `05-riskler-engeller.md` içindeki "Cevap bekleyen sorular" tablosuna taşınacak.

---

## 2026-08-16 — Kurulum

**Durum:** PO çalışma alanı kuruldu. Henüz proje verisi girilmedi.

**Sonraki brifingte sorulacaklar:**

1. Aktif sprint hangisi, tarihleri ne? (`00-proje/ekip-ve-ritim.md` boş)
2. Ekipte kim var, roller ne? (`00-proje/ekip-ve-ritim.md` boş)
3. Tören takvimi nasıl — refinement, planlama, review hangi gün? (`00-proje/ekip-ve-ritim.md` boş)
4. ap-action-management tek cümleyle ne yapıyor, hangi problemi çözüyor? (`00-proje/vizyon.md` boş)
5. Şu an en kritik 3 paydaş kim? (`00-proje/paydaslar.md` boş)

---

<!--
Yeni gün eklerken bu şablonu kullan, EN ÜSTE ekle:

## YYYY-AA-GG

**Brifingte söylenenler:**
- [özet]

**Sorular ve cevaplar:**
1. S: [soru]
   C: [cevap]

**Bu cevaplardan çıkan güncellemeler:**
- [dosya] → [ne eklendi]

**Açık kalanlar:**
- [cevaplanmayan soru]
-->
