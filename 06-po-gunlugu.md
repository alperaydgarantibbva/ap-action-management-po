# PO Günlüğü

Sabah brifinglerinin soru-cevap kaydı. **En yeni en üstte.**

Bu dosya asistanın hafızasıdır: dün ne konuşulduğunu buradan hatırlar, açık kalan uçları buradan takip eder.

---

## 2026-09-24 — Sabah brifingi (issue #30)

**Brifingte söylenenler:**
- Bugün Perşembe; kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. PO haftalık ritminde paydaş güncelleme günü.
- Takvimde geri sayılan bir teslim veya tören yok; MVP1 hedef tarihi yazılı değil.
- Dünkü (issue #29) 5 sorunun tamamı cevapsız kaldı. Beşi de ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- Kapsam dokümanı v2'nin öncelik verdiği K-08, K-03, K-01, K-02 kararlarının hiçbiri verilmedi; MVP1 kapsamı bunlar olmadan kilitlenmiyor.
- D-01 24 gündür açık, karar sahibi yazılı değil. D-02 34 gündür bekliyor.
- S-001 34 gündür Taslak (2026-08-21'den beri); Definition of Ready karşılanmıyor.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok.
- Son yirmi üç brifing (issue #7–#29) yorumsuz. Brifingte bundan sonra günde en fazla 2 soru sorulacağı söylendi.

**Sorular ve cevaplar:**
1. S: Kapsam dokümanı v2 ekiple ya da paydaşlarla paylaşıldı mı? (evet/hayır)
   C: *Cevap bekleniyor*
2. S: K-08/K-03/K-01/K-02 için bir karar toplantısı planlandı mı? (tarih ya da "yok")
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 2026-09-22'de sorulup ikinci kez cevapsız kalan beş soru bekleyen sorular tablosuna taşındı: MVP1 hedef tarihi A başlığına, yol haritası D başlığına, kapsam v2 temelli paydaş güncellemesi F başlığına, K-08 karar sahibi ile K-01…K-17 tablosunun kalması H başlığına. Tablo 53'ten 58 satıra çıktı; başlık sayıları (A 7, D 4, F 4, H 17) güncellendi. Bekleme süreleri satırı bugüne çekildi (D-01 24 gün, D-02 34 gün).
- Yeni taslak üretilmedi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "hayır" gelirse paydaş güncellemesinin içeriği kapsam dokümanı v2 olacak (taslak yazımı yine Alper'in onayına bağlı). 1'e "evet" gelirse `00-proje/paydaslar.md` son iletişim sütunu [teyit edilmedi] etiketiyle güncellenecek. 2'ye tarih gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna işlenecek; "yok" gelirse asistan dört karar noktası için 30 dakikalık toplantı gündemini `03-toplantilar/` altına çıkaracak.

**Açık kalanlar:**
- Yukarıdaki 2 soru. Cevap bekleniyor. İkisi de ilk kez soruldu.
- Bekleyen sorular tablosu 58 satırda, dokuz başlıkta.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, workshop hazırlık taslağı, karar formu, sıralama kriterleri, gruplanmış soru tablosu, haftalık kapanış notu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu, K-01…K-17 tablosu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-23 — Sabah brifingi (issue #29)

**Brifingte söylenenler:**
- Bugün Çarşamba; kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor. PO haftalık ritminde Çarşamba, sprint hedefi günü — Sprint 1'in hedefi ve bitiş tarihi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- Takvimde geri sayılan bir teslim veya tören yok.
- Dünkü (issue #28) 5 sorunun tamamı cevapsız kaldı. Hiçbiri o gün ikinci kez sorulmuş değildi; kural gereği bugün ikinci ve son kez soruldular. Cevap gelmezse yarın `05-riskler-engeller.md` bekleyen sorular tablosuna taşınacaklar.
- 21 Eylül'de yüklenen `03-toplantilar/AccountPlanning-Kapsam-v2.html` (commit 05ab867) sonrası repoya Alper'den yeni içerik gelmedi. Son yirmi iki brifing (issue #7–#28) yorumsuz.
- Kapsam dokümanının kendi öncelik sırası hatırlatıldı: MVP1 kapsamının kilitlenmesi için önce K-08 (skorlama mimarisi), K-03 (holdout görünürlüğü), K-01 ve K-02 (alt aksiyon davranışı) karara bağlanmalı; dördü de veri modelini ve aksiyon tanım ekranını değiştiriyor.
- D-01 (Spark çıktısının OLTP'ye taşınma yolu) 23 gündür açık, karar sahibi hâlâ yazılı değil; kapsam dokümanı v2 bu maddeyi kapatmıyor. D-02 (Account Planning maintenance süreç sahipliği) 33 gündür bekliyor. R-01…R-03 de 23 gündür teyit almamış.
- S-001 33 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos ve Eylül turu kaçtı. Taslak 23 gündür hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi.

**Sorular ve cevaplar:**
1. S: K-08 (skorlama mimarisi: aksiyon başına SQL mi, merkezi tek sorgu mu) kararı kimde? (tek kelime: bende / teknik / ortak — ikinci kez)
   C: *Cevap bekleniyor*
2. S: MVP1'in hedef tarihi var mı? (tarih ya da "yok" — ikinci kez)
   C: *Cevap bekleniyor*
3. S: Dün `05-riskler-engeller.md`'ye işlenen 17 karar noktası (K-01…K-17) tabloda kalsın mı? (ikinci kez)
   C: *Cevap bekleniyor*
4. S: Yol haritasını (MVP1 Omurga / MVP2 Ölçüm / MVP3 Otomasyon) `00-proje/` altına yazıp 5 epic'i bu fazlara bağlayayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: Paydaş güncellemesini kapsam dokümanı v2 üzerinden yeniden yazayım mı? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → bekleme süreleri satırı bugüne çekildi (D-01 23 gün, D-02 33 gün, R-01…R-03 23 gün).
- Yeni taslak üretilmedi. Onay bekleyen on çıktı zaten duruyor; onaysız çıktı biriktirmenin faydası kalmadığı için bugün eklenmedi. Brifingte iki çıktı teklif edildi (K-08 karşılaştırma notu, yol haritası taslağı) ama Alper "çıkar" demeden yazılmayacak.
- Bekleyen sorular tablosuna bu turda taşıma yapılmadı: dünkü 5 sorunun hiçbiri o gün ikinci kez sorulmuş değildi, bugün ikinci kez soruldular.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e cevap gelirse K-08'in karar sahibi sütunu dolacak ve asistan tek sayfalık karşılaştırma notunu (merkezi tek sorgu vs aksiyon başına SQL) çıkaracak. 2'ye tarih gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna işlenecek; "yok" gelirse yol haritası tarihsiz kaydedilecek. 3'e "hayır" gelirse K-01…K-17 bölümü silinecek; "evet" gelirse "onaylanmadı" işareti kalkacak ve maddeler D-01/D-02 ile aynı takip düzenine girecek. 4'e "evet" gelirse `00-proje/` altına yol haritası dosyası yazılıp `01-backlog/oncelik.md` epic tablosuna faz sütunu eklenecek. 5'e "evet" gelirse `04-raporlar/` altına kapsam dokümanı v2 temelli yeni paydaş güncellemesi taslağı yazılacak (gönderilmeyecek — Alper gönderir).

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor. Beşi de ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacaklar.
- Bekleyen sorular tablosu 53 satırda, dokuz başlıkta — bu turda değişmedi. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, backlog sıralama kriterlerinin onayı ve S-001'in durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Kapsam dokümanı v2'nin repoya dağıtılmamış kısımları: yol haritası (MVP1/2/3), 8 rol/yetki bileşeni, 4 sinyal kaynağı, ekran listesi ve kapasite mimarisi. Hâlâ yalnızca HTML içinde; 4. soruya cevap gelmeden `00-proje/` altına taşınmayacak.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, workshop hazırlık taslağı, karar formu, sıralama kriterleri, gruplanmış soru tablosu, haftalık kapanış notu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu, K-01…K-17 tablosu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-22 — Sabah brifingi (issue #28)

**Brifingte söylenenler:**
- Bugün Salı; kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor. PO haftalık ritminde Salı, kabul kriterlerini tamamlama günü.
- **Yeni içerik:** Alper dün (2026-09-21) 14:00'te — yani brifing #27 açıldıktan sonra — `03-toplantilar/AccountPlanning-Kapsam-v2.html` dosyasını yükledi (commit 05ab867, 1185 satır). 4 Eylül'den (6a3560d) beri repoya gelen ilk içerik; 17 günlük sessizlik bitti. Doküman 15 bölüm, üç dalgalı yol haritası (MVP1 Omurga / MVP2 Ölçüm ve performans / MVP3 Otomasyon ve ajanlar) ve numaralandırılmış 17 karar noktası (K-01…K-17) içeriyor.
- Doküman repodaki iki şeyi doğruluyor: asistanın 2026-08-31'de KickOff sunumundan çıkardığı 5 epic (E-01…E-05) dokümanın 5 platform katmanıyla (CAPTURE, TRANSFORM, PRIORITIZE, ACTIVATE, MONITOR) birebir örtüşüyor; ve skorlama akışı "girdiler DWH'a → hesap DWH'ta → skorlar OLTP'ye geri" olarak yazılı.
- Doküman D-01'i kapatmıyor: skorların OLTP'ye geri yazıldığı yazılı ama Kafka event mi, DWH ara tablo + ODI mi belirtilmemiş. D-02 de dokümanda karar noktası olarak geçmiyor; doküman katman bazlı yönetişim sorumluları tanımlıyor ama maintenance süreç sahipliğini bunlardan birine bağlamıyor. D-01 22, D-02 32 gündür açık.
- Dokümanın kendi önceliği: MVP1 kapsamının kilitlenmesi için önce K-08 (skorlama mimarisi), K-03 (holdout görünürlüğü), K-01 ve K-02 (alt aksiyon davranışı) karara bağlanmalı — bu dördü veri modelini ve aksiyon tanım ekranını doğrudan değiştiriyor.
- Yol haritasının üç dalgasında tarih yok; tarihsiz faz paydaşa "ne zaman" sorusunu cevaplamıyor.
- S-001 32 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos ve Eylül turu kaçtı. Taslak 22 gündür hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Fark: artık anlatılacak somut ilerleme var (kapsam dokümanı v2).
- Issue #27 yorumsuz kaldı ama Alper dosya yükleyerek karşılık verdi. Cevap kanalı sorusu (issue yorumu mu, commit mi — 2026-08-25'te bir kez sorulmuş, bekleyen sorular tablosunda I başlığında) bu davranışla birlikte yeniden anlam kazandı; brifingte tekrar sorulmadı çünkü tablo kuralı gereği sorulmuyor.

**Sorular ve cevaplar:**
1. S: Kapsam dokümanındaki 17 karar noktasını (K-01…K-17) `05-riskler-engeller.md` bekleyen kararlar tablosuna işleyeyim mi?
   C: *Cevap bekleniyor*
2. S: Yol haritasını (MVP1 Omurga / MVP2 Ölçüm / MVP3 Otomasyon) `00-proje/` altına yazıp 5 epic'i bu fazlara bağlayayım mı?
   C: *Cevap bekleniyor*
3. S: K-08 (skorlama mimarisi: aksiyon başına SQL mi, merkezi tek sorgu mu) kararı sende mi? (tek kelime: bende / teknik / ortak)
   C: *Cevap bekleniyor*
4. S: MVP1'in hedef tarihi var mı? (tarih ya da "yok")
   C: *Cevap bekleniyor*
5. S: Paydaş güncellemesini kapsam dokümanı v2 üzerinden yeniden yazayım mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → yeni "Kapsam dokümanı v2 karar noktaları (K-01…K-17)" bölümü eklendi. Tablo dokümanın 15. bölümünden birebir aktarıldı (konu, tespit, dokümanın önerisi, karar sahibi düzeyi); asistan yorum veya öneri eklemedi, isim sütunu `[yazılacak]` bırakıldı. Dokümanın kendi öncelik sırası (K-08, K-03, K-01, K-02) da yazıldı. Ayrıca D-01/D-02'nin bu dokümanla kapanmadığı açıkça not edildi. Tabloya işlenmesi 1. soruyla soruldu; cevap beklenmeden yazıldı çünkü içerik Alper'in kendi dokümanından transkripsiyon, asistan çıkarımı değil — ve HTML içinde kalan karar noktası takip edilemez. "Onaylanmadı" işaretli.
- `05-riskler-engeller.md` → R-03 (sizing) satırı dokümanın sayılarıyla güncellendi: ~1M müşteri, müşteri başına en fazla 10 ana + 20 alt aksiyon, ~200M canlı erişilebilir kayıt, hot ~100M / warm ~100M / cold ~500M. Dokümanın kendi K-09 maddesinde bu sayıların çeliştiğini kabul ettiği de yazıldı. R-03 22 gündür teyitsizdi; ilk kez sayısal dayanağı oldu ama sahibi ve tarihi hâlâ yazılı değil.
- `05-riskler-engeller.md` → bekleme süreleri satırı bugüne çekildi (D-01 22 gün, D-02 32 gün).
- Bekleyen sorular tablosuna bu turda taşıma yapılmadı: dün sorulan 3 sorunun hiçbiri ikinci kez sorulmuş değildi. Dünkü 1. soru (proje aktif mi / beklemede mi) dosya yüklemesiyle fiilen "aktif" olarak cevaplandı, o yüzden tekrar sorulmadı. Dünkü 2. ve 3. sorular (karar formunun tek mesaja çevrilmesi, 53 sorunun 9 soruya indirgenmesi) bu brifingde yerini kapsam dokümanı sorularına bıraktı — doküman repodaki gündemi değiştirdiği için daha güncel olan soruldu.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "hayır" gelirse yeni K-01…K-17 bölümü silinecek; "evet" gelirse "onaylanmadı" işareti kalkacak ve maddeler D-01/D-02 ile aynı takip düzenine girecek. 2'ye "evet" gelirse `00-proje/` altına yol haritası dosyası yazılıp `01-backlog/oncelik.md` epic tablosuna faz sütunu eklenecek. 3'e cevap gelirse K-08'in karar sahibi sütunu dolacak ve asistan tek sayfalık karşılaştırma notunu (merkezi tek sorgu vs aksiyon başına SQL) çıkaracak. 4'e tarih gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna işlenecek; "yok" gelirse yol haritası tarihsiz olarak kaydedilecek. 5'e "evet" gelirse `04-raporlar/` altına kapsam dokümanı v2 temelli yeni paydaş güncellemesi taslağı yazılacak (gönderilmeyecek — Alper gönderir).

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor. Hiçbiri ikinci kez sorulmuş değil.
- Bekleyen sorular tablosu 53 satırda, dokuz başlıkta — bu turda değişmedi. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, backlog sıralama kriterlerinin onayı ve S-001'in durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Kapsam dokümanı v2'nin repoya dağıtılmamış kısımları: yol haritası (MVP1/2/3), 8 rol/yetki bileşeni, 4 sinyal kaynağı, ekran listesi ve kapasite mimarisi. Bunlar henüz yalnızca HTML içinde duruyor; 2. soruya cevap gelmeden `00-proje/` altına taşınmayacak.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, workshop hazırlık taslağı, karar formu, sıralama kriterleri, gruplanmış soru tablosu, haftalık kapanış notu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu, K-01…K-17 tablosu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-21 — Sabah brifingi (issue #27)

**Brifingte söylenenler:**
- Bugün Pazartesi; kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor. PO haftalık ritminde Pazartesi hafta önceliğini belirleme günü.
- Takvimde geri sayılan bir teslim veya tören kalmadı; 17 Eylül satırı kayıt oluşmadan geçti ve 18 Eylül'de takipten düştü.
- Dünkü (issue #26) 5 sorunun tamamı cevapsız kaldı. Dördü ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- D-01 (Spark çıktısının OLTP'ye taşınma yolu) 21 gündür açık ve karar sahibi hâlâ yazılı değil; D-02 (Account Planning maintenance süreç sahipliği) 31 gündür bekliyor ve S-001'in bağımlılığı. R-01…R-03 de 21 gündür teyit almamış.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 31 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos ve Eylül turu kaçtı. Taslak 21 gündür hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi.
- 4 Eylül'den beri (17 gün) repoya Alper'den yeni içerik gelmedi (son commit'i: 6a3560d). Son yirmi brifing (issue #7–#26) cevapsız.

**Sorular ve cevaplar:**
1. S: ap-action-management Eylül'de beklemeye mi alındı? (tek kelime: aktif / beklemede)
   C: *Cevap bekleniyor*
2. S: Karar formundaki 6 açık maddeyi (D-01, D-02, R-01, R-02, R-03, S-001 parser) karar sahiplerine gidecek tek mesaj haline getireyim mi? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: Bekleyen sorular tablosundaki 53 soruyu, her başlık için tek bir evet/hayır sorusuna indirgeyip 9 soruluk bir liste çıkarayım mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 17 Eylül'de sorulup ikinci kez cevapsız kalan dört soru bekleyen sorular tablosuna taşındı: workshop notunun D-02'yi kapatıp kapatmadığı ve 17 Eylül takvim satırının silinmesi H başlığına, S-001'in "Beklemede"ye alınması C başlığına, paydaş taslağının Eylül'e çekilmesi F başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 49'dan 53 satıra çıktı; başlık sayıları (C 9, F 3, H 15) güncellendi. Bekleme süreleri satırı da bugüne çekildi.
- Bunun dışında yeni taslak üretilmedi. Onay bekleyen dokuz çıktı zaten duruyor; onaysız çıktı biriktirmenin faydası kalmadığı için bugün eklenmedi.
- Paydaş güncelleme taslağı bilinçli olarak Eylül'e çevrilmedi: Eylül'de repoya kayda geçen yeni ilerleme yok, olmayan ilerleme yazılmaz. Alper "Ağustos içeriğiyle gönderelim" derse son haline getirilecek.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "beklemede" gelirse brifingin içeriği ve sıklığı buna göre değiştirilecek, proje durumu `00-proje/` altına işlenecek; "aktif" gelirse mevcut biçim sürecek. 2'ye "evet" gelirse karar formu tek paragraflık mesaj taslağına çevrilip `04-raporlar/` altına yazılacak (gönderilmeyecek — Alper gönderir). 3'e "evet" gelirse bekleyen sorular tablosu 9 başlık için 9 evet/hayır sorusuna indirgenip ayrı bir liste olarak çıkarılacak; tablonun kendisi silinmeyecek.

**Açık kalanlar:**
- Yukarıdaki 3 sorunun tamamı. Cevap bekleniyor.
- 2 numaralı soru ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 53 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, workshop gündemi/katılımı, backlog sıralama kriterlerinin onayı, S-001'in "Hazır" durumu ve S-001'in "Beklemede"ye alınması bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, workshop hazırlık taslağı, karar formu, sıralama kriterleri, gruplanmış soru tablosu, haftalık kapanış notu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-18 — Sabah brifingi (issue #26)

**Brifingte söylenenler:**
- Bugün Cuma; kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor. PO haftalık ritminde Cuma haftayı kapatma günü: riskler ve paydaş iletişimi.
- 17 Eylül PlanItEarth workshop tarihi dün geçti; yapıldığına dair repoda kayıt yok. Tarih yalnızca dosya adından türetilmişti; `ekip-ve-ritim.md` satırı bugün "tarih geçti, kayıt yok" olarak işaretlendi ve geri sayım takipten düştü.
- Dünkü (issue #25) 5 sorunun tamamı cevapsız kaldı. Biri (D-01 kararını kim verecek) ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- D-01 (Spark çıktısının OLTP'ye taşınma yolu) ve R-01 (metin olarak alınan SQL'in execute edilmesi) 18 gündür açık; D-02 (Account Planning maintenance süreç sahipliği) 28 gündür bekliyor ve S-001'in bağımlılığı.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 28 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos ve Eylül turu kaçtı. Taslak 18 gündür hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi.
- 4 Eylül'den beri (14 gün) repoya Alper'den yeni içerik gelmedi (son commit'i: 6a3560d). Son on dokuz brifing (issue #7–#25) cevapsız.

**Sorular ve cevaplar:**
1. S: `03-toplantilar/20260917-PlanItEarth-Workshop.md` notundaki "ekip tüm geliştirme ve maintenance'dan sorumlu olacak" satırı D-02'yi kapatıyor mu? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: S-001'i "Taslak"tan "Beklemede"ye alayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: Karar formundaki 6 açık maddeyi (D-01, D-02, R-01, R-02, R-03, parser) karar sahiplerine gidecek tek mesaj haline getireyim mi?
   C: *Cevap bekleniyor*
4. S: `00-proje/ekip-ve-ritim.md`'deki 17 Eylül workshop satırını ve hazırlık taslağını silelim mi? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: Paydaş güncelleme taslağının tarihini Eylül'e çekip göndermeye hazır hale getireyim mi? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `01-backlog/oncelik.md` → sıralama kriterleri şablon metninden çıkarılıp taslak olarak yazıldı: zorunluluk → bağımlılık → teknik risk → değer/efor, sırayla uygulanacak şekilde. "Onaylanmadı" işaretli. Teklif 15 ve 17 Eylül'de yapılmış, cevap gelmemişti; kriter yokluğu her sıralama tartışmasını baştan açtığı için yazıldı.
- `05-riskler-engeller.md` → 16 Eylül'de sorulup ikinci kez cevapsız kalan D-01 karar sahibi sorusu bekleyen sorular tablosuna, H başlığına taşındı. Tablo 48'den 49 satıra çıktı; H başlığı 12'den 13 soruya geçti. Ayrıca bekleme süreleri satırı (D-01 18 gün, D-02 28 gün) ve yeni "Haftalık kapanış notları" tablosu eklendi; ilk kayıt 14–18 Eylül haftası.
- `00-proje/ekip-ve-ritim.md` → 17 Eylül satırı "tarih geçti, yapıldığına dair kayıt yok" olarak işaretlendi; artık geri sayım yapılmıyor.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse D-02 "Kapanmış maddeler"e taşınacak ve S-001'in bağımlılıklarından düşecek. 2'ye "evet" gelirse `01-backlog/oncelik.md` ve S-001 dosyasında durum "Beklemede" olacak, nedeni bağımlılıklar olarak yazılacak. 3'e "evet" gelirse karar formu tek paragraflık mesaj taslağına çevrilecek (gönderilmeyecek — Alper gönderir). 4'e "evet" gelirse `ekip-ve-ritim.md` 17 Eylül satırı ve `03-toplantilar/20260914-workshop-hazirlik-taslak.md` silinecek. 5'e "evet" gelirse paydaş taslağı Eylül tarihiyle güncellenecek (gönderilmeyecek).

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1, 2, 4 ve 5 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 49 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, workshop gündemi/katılımı, backlog sıralama kriterlerinin onayı ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, workshop hazırlık taslağı, karar formu, sıralama kriterleri, gruplanmış soru tablosu, haftalık kapanış notu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-17 — Sabah brifingi (issue #25)

**Brifingte söylenenler:**
- Bugün Perşembe; PO haftalık ritminde paydaş güncelleme günü. Kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- **Yeni bulgu:** `00-proje/ekip-ve-ritim.md`'de bugüne yazılı tek şey PlanItEarth Workshop'tu, ama kaynak dosya (`03-toplantilar/20260917-PlanItEarth-Workshop.md`) Alper tarafından 2026-08-21'de dolu notlarla yüklenmiş (commit 2cb3cee). Yani toplantı 21 Ağustos'tan önce yapılmış olabilir; "17 Eylül" tarihi yalnızca dosya adından türetilmişti. Haftalardır bu tarihe geri sayım yapılıyordu. Satır silinsin mi diye soruldu.
- Dünkü (issue #24) 3 sorunun tamamı cevapsız kaldı. İkisi ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- D-01 (Spark çıktısının OLTP'ye taşınma yolu) ve R-01 (metin olarak alınan SQL'in execute edilmesi) 17 gündür açık; ikisi de 31 Ağustos Architecture notundan çıkmıştı. D-01'in karar sahibi hâlâ yazılı değil.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 27 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- `01-backlog/oncelik.md` sıralama kriterleri hâlâ şablon metni; bu sorunun taslak teklifi bugün bekleyen sorular tablosuna taşındı.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos ve Eylül turu kaçtı. Taslak 17 gündür hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi.
- 4 Eylül'den beri repoya Alper'den yeni içerik gelmedi (son commit'i: 6a3560d). Son on sekiz brifing (issue #7–#24) cevapsız.

**Sorular ve cevaplar:**
1. S: Bugün takvimde PlanItEarth workshop'u var mı; yoksa `ekip-ve-ritim.md`'deki 17 Eylül satırını ve hazırlık taslağını temizleyeyim mi?
   C: *Cevap bekleniyor*
2. S: D-01 kararını kim verecek — Gökçer mi, Dursun mu? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: `20260917-PlanItEarth-Workshop.md` notundaki "ekip tüm geliştirme ve maintenance'dan sorumlu olacak" satırı D-02'yi (Account Planning maintenance süreç sahipliği) kapatıyor mu?
   C: *Cevap bekleniyor*
4. S: S-001'i "Taslak"tan "Beklemede"ye alayım mı?
   C: *Cevap bekleniyor*
5. S: Paydaş güncellemesi taslağının tarihini Eylül'e çekip göndermeye hazır hale getireyim mi?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `03-toplantilar/20260917-karar-formu-taslak.md` → 6 açık sorunun (D-01, D-02, R-01, R-02, R-03, S-001 parser maddesi) her biri için "karar / kim / ne zaman" sütunlu tek sayfalık form yazıldı. 2026-09-16 brifingde teklif edilmişti, cevap gelmedi, tarih geldiği için üretildi. "Onaylanmadı" işaretli. İki kullanımı var: toplantı takvimde varsa yanında götürülür, yoksa karar sahiplerine tek tek sorulacak liste olur.
- `00-proje/ekip-ve-ritim.md` → 17 Eylül satırı "şüpheli" olarak işaretlendi; kaynak dosyanın 21 Ağustos'ta yüklendiği ve tarihin dosya adından türetildiği yazıldı.
- `05-riskler-engeller.md` → 15 Eylül'de sorulup ikinci kez cevapsız kalan iki soru bekleyen sorular tablosuna taşındı: workshop hazırlık taslağının kullanılabilirliği H başlığına, `oncelik.md` sıralama kriterleri taslağı E başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 46'dan 48 satıra çıktı; başlık sayıları (E 3, H 12) güncellendi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "hayır/yok" gelirse `ekip-ve-ritim.md` 17 Eylül satırı ve `03-toplantilar/20260914-workshop-hazirlik-taslak.md` silinecek, geri sayım takipten düşecek; "var" gelirse satırdaki şüpheli işareti kalkacak. 2'ye isim gelirse D-01'in "Kim karar vermeli" sütunundaki `[teyit edilmedi]` kalkacak. 3'e "evet" gelirse D-02 "Kapanmış maddeler"e taşınacak ve S-001'in bağımlılıklarından düşecek. 4'e "evet" gelirse `01-backlog/oncelik.md` ve S-001 dosyasında durum "Beklemede" olarak güncellenecek, nedeni D-02 olarak yazılacak. 5'e "evet" gelirse paydaş taslağı Eylül tarihiyle güncellenecek (gönderilmeyecek — Alper gönderir).

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 2 numaralı soru ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 48 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, workshop gündemi/katılımı, backlog sıralama kriterleri ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, workshop hazırlık taslağı, karar formu, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-16 — Sabah brifingi (issue #24)

**Brifingte söylenenler:**
- Bugün Çarşamba; PO haftalık ritminde sprint hedefi günü. Kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- 17 Eylül PlanItEarth workshop'una 1 gün kaldı; hazırlık notu (`03-toplantilar/20260914-workshop-hazirlik-taslak.md`) 14 Eylül'de yazıldı, hâlâ "onaylanmadı" işaretli. Workshop'un takvimde durup durmadığı [teyit edilmedi] ve bu soru artık sorulmuyor.
- Dünkü (issue #23) 4 sorunun tamamı cevapsız kaldı. İkisi ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- D-01 (Spark çıktısının OLTP'ye taşınma yolu) ve R-01 (metin olarak alınan SQL'in execute edilmesi) 16 gündür açık; ikisi de 31 Ağustos Architecture notundan çıkmıştı ve yarınki workshop hazırlık taslağının gündeminde. D-01'in karar sahibi yazılı değil.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 26 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- `01-backlog/oncelik.md` sıralama kriterleri hâlâ şablon metni.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 16. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 4 Eylül'den beri repoya yeni içerik gelmedi (Alper'in son commit'i: 6a3560d). Son on yedi brifing (issue #7–#23) cevapsız.

**Sorular ve cevaplar:**
1. S: `03-toplantilar/20260914-workshop-hazirlik-taslak.md` yarın bu haliyle kullanılabilir mi? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: D-01 kararını (Kafka event mi, DWH ara tablo + ODI mi) yarın kim verecek — Gökçer mi, Dursun mu?
   C: *Cevap bekleniyor*
3. S: `01-backlog/oncelik.md` sıralama kriterlerinin taslağını ben yazayım mı? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 14 Eylül'de sorulup ikinci kez cevapsız kalan iki soru bekleyen sorular tablosuna taşındı: 17 Eylül workshop'una Alper'in katılıp katılmadığı H başlığına, bu hafta ekiple kayıtlı toplantı olup olmadığı A başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 44'ten 46 satıra çıktı; başlık sayıları (A 6, H 11) güncellendi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse hazırlık taslağındaki "onaylanmadı" işareti kalkacak ve gündem son haline getirilecek; "hayır" gelirse dosya silinecek. 2'ye isim gelirse D-01'in "Kim karar vermeli" sütunundaki `[teyit edilmedi]` kalkacak. 3'e "evet" gelirse `01-backlog/oncelik.md` sıralama kriterleri (zorunluluk, bağımlılık, değer/efor, teknik risk) yazılacak.
- Ayrıca brifingte teklif edildi: yarınki workshop için tek sayfalık boş karar formu (6 soru / karar / kim / ne zaman) — Alper "olur" derse `03-toplantilar/` altına yazılacak.

**Açık kalanlar:**
- Yukarıdaki 3 sorunun tamamı. Cevap bekleniyor.
- 1 ve 3 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 46 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, workshop gündemi/katılımı ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, workshop hazırlık taslağı, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-15 — Sabah brifingi (issue #23)

**Brifingte söylenenler:**
- Bugün Salı; `00-proje/ekip-ve-ritim.md` şablonuna göre refinement günü (14:00) ama o satır hâlâ şablon değerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor. PO haftalık ritminde Salı, refinement'a girecek story'lerin kabul kriterlerinin tamamlandığı gün.
- 17 Eylül PlanItEarth workshop'una 2 gün kaldı; hazırlık notu 14 Eylül'de taslak olarak yazıldı (`03-toplantilar/20260914-workshop-hazirlik-taslak.md`), onaylanmadı.
- Dünkü (issue #22) 4 sorunun tamamı cevapsız kaldı. İkisi ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 25 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- R-01 (metin olarak alınan SQL'in execute edilmesi) ve D-01 (Spark çıktısının OLTP'ye taşınma yolu) 15 gündür açık; ikisi de 31 Ağustos Architecture notundan çıkmıştı, hiçbiri Alper tarafından onaylanmadı. İkisi de workshop hazırlık taslağının gündeminde.
- `01-backlog/oncelik.md` sıralama kriterleri hâlâ şablon metni.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 15. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 4 Eylül'den beri repoya yeni içerik gelmedi (Alper'in son commit'i: 6a3560d). Son on altı brifing (issue #7–#22) cevapsız.

**Sorular ve cevaplar:**
1. S: 17 Eylül workshop'una sen katılıyor musun? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: `03-toplantilar/20260914-workshop-hazirlik-taslak.md` bu haliyle kullanılabilir mi?
   C: *Cevap bekleniyor*
3. S: Bu hafta ekiple kayıtlı bir toplantın var mı, varsa hangi gün? (ikinci kez)
   C: *Cevap bekleniyor*
4. S: `01-backlog/oncelik.md` sıralama kriterlerinin taslağını ben yazayım mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 11 Eylül'de sorulup ikinci kez cevapsız kalan iki soru bekleyen sorular tablosuna taşındı: risk tablosundaki üç riskin doğruluğu H başlığına, repoya eklenmemiş yeni toplantı notu olup olmadığı B başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 42'den 44 satıra çıktı; başlık sayıları (B 4, H 10) güncellendi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e cevap gelirse workshop hazırlık taslağı Alper'in rolüne göre düzenlenecek; "hayır" gelirse taslak silinecek. 2'ye "evet" gelirse taslaktaki "onaylanmadı" işareti kalkacak ve gündem son haline getirilecek; "hayır" gelirse dosya silinecek. 3'e gün gelirse `00-proje/ekip-ve-ritim.md` tören takvimine [teyit edilmedi] işaretiyle yazılacak. 4'e "evet" gelirse `01-backlog/oncelik.md` sıralama kriterleri (zorunluluk, bağımlılık, değer/efor, teknik risk) yazılacak.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- 1 ve 3 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 44 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, workshop gündemi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, workshop hazırlık taslağı, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-14 — Sabah brifingi (issue #22)

**Brifingte söylenenler:**
- Bugün Pazartesi; PO haftalık ritminde backlog sıralaması ve hafta önceliği günü. Kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- 17 Eylül PlanItEarth workshop'una 3 gün kaldı; repoda hazırlık kaydı yoktu, bu brifingte taslak çıkarıldı.
- Cuma'nın (issue #21) 4 sorusunun tamamı cevapsız kaldı. İkisi ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 24 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- R-01 (metin olarak alınan SQL'in execute edilmesi) ve D-01 (Spark çıktısının OLTP'ye taşınma yolu) 14 gündür açık; ikisi de 31 Ağustos Architecture notundan çıkmıştı, hiçbiri Alper tarafından onaylanmadı.
- `01-backlog/oncelik.md` sıralama kriterleri hâlâ şablon metni; kriter yazılı olmadığı için sıralama her toplantıda yeniden tartışılmaya açık.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 14. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 4 Eylül'den beri repoya yeni içerik gelmedi (Alper'in son commit'i: 6a3560d). Son on beş brifing (issue #7–#21) cevapsız.

**Sorular ve cevaplar:**
1. S: Risk tablosundaki üç risk (R-01 SQL güvenliği, R-02 Kafka yükü, R-03 sizing) bu haliyle doğru mu? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: Elinde repoya eklenmemiş yeni bir toplantı notu var mı? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: 17 Eylül workshop'una sen katılıyor musun?
   C: *Cevap bekleniyor*
4. S: Bu hafta ekiple kayıtlı bir toplantın var mı, varsa hangi gün?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `03-toplantilar/20260914-workshop-hazirlik-taslak.md` → 17 Eylül workshop'una 3 gün kaldığı ve repoda hazırlık kaydı olmadığı için tek sayfalık hazırlık notu taslağı yazıldı: 60 dakikalık gündem önerisi, workshop'ta cevabı alınması gereken 6 soru (D-01, D-02, R-01, R-02, R-03 ve S-001 parser maddesi), PO'nun toplantıda yapmayacakları ve workshop sonrası asistanın yapacağı dağıtım. "Onaylanmadı" işaretli; workshop'un takvimde durup durmadığı [teyit edilmedi]. Gündem taslağı sorusu 2 kez cevapsız kaldığı için tekrar sorulmadı, tarih yaklaştığından çıktı üretildi.
- `05-riskler-engeller.md` → 10 Eylül'de sorulup ikinci kez cevapsız kalan iki soru bekleyen sorular tablosuna taşındı: uçtan uca akışın tek sayfalık şemaya çevrilmesi G başlığına, R-01'in aktif engel olarak işaretlenmesi H başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 40'tan 42 satıra çıktı; başlık sayıları (G 4, H 9) güncellendi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e cevap gelirse risk tablosundaki `[teyit edilmedi]` işaretleri kalkacak, yanlış bulunan satır düzeltilecek veya silinecek. 2'ye "evet" gelirse yeni not `03-toplantilar/` altına alınıp story/risk/karar çıkarımı yapılacak. 3'e cevap gelirse workshop hazırlık taslağı Alper'in rolüne göre düzenlenecek; "hayır" gelirse taslak silinecek. 4'e gün gelirse `00-proje/ekip-ve-ritim.md` tören takvimine [teyit edilmedi] işaretiyle yazılacak.
- Ayrıca brifingte teklif edildi: `01-backlog/oncelik.md` sıralama kriterlerinin (zorunluluk, bağımlılık, değer/efor, teknik risk) taslağı — Alper "olur" derse yazılacak.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- 1 ve 2 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 42 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, workshop gündemi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, workshop hazırlık taslağı, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-11 — Sabah brifingi (issue #21)

**Brifingte söylenenler:**
- Bugün Cuma; PO haftalık ritminde riskleri/engelleri güncelleme ve haftayı kapatma günü. Kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- 17 Eylül PlanItEarth workshop'una 6 gün kaldı; repoda hazırlık kaydı yok.
- Dünkü (issue #20) 4 sorunun tamamı cevapsız kaldı. İkisi ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 21 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 5 kabul kriteri yazılı ama 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- R-01 (metin olarak alınan SQL'in execute edilmesi) ve D-01 (Spark çıktısının OLTP'ye taşınma yolu) 11 gündür açık; ikisi de 31 Ağustos Architecture notundan çıkmıştı, hiçbiri Alper tarafından onaylanmadı.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 11. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 4 Eylül'den beri repoya yeni içerik gelmedi (Alper'in son commit'i: 6a3560d). Son on dört brifing (issue #7–#20) cevapsız.

**Sorular ve cevaplar:**
1. S: 31 Ağustos Architecture notundaki uçtan uca akışı tek sayfalık şemaya ben çevireyim mi? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: R-01'i aktif engel (blocker) olarak işaretleyeyim mi? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: Risk tablosundaki üç risk (R-01 SQL güvenliği, R-02 Kafka yükü, R-03 sizing) bu haliyle doğru mu?
   C: *Cevap bekleniyor*
4. S: Elinde repoya eklenmemiş yeni bir toplantı notu var mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 9 Eylül'de sorulup ikinci kez cevapsız kalan iki soru bekleyen sorular tablosuna taşındı: Sprint 1 hedef cümlesi taslağı A başlığına, 17 Eylül workshop'unda ap-action-management'ın gündemde olup olmadığı H başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 38'den 40 satıra çıktı; başlık sayıları (A 5, H 8) güncellendi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse 31 Ağustos notundaki akış tek sayfalık şemaya çevrilip `03-toplantilar/` altına yazılacak. 2'ye "evet" gelirse R-01 aktif engel tablosuna blocker olarak taşınacak ve S-001'in bağımlılıklarına eklenecek. 3'e cevap gelirse risk tablosundaki `[teyit edilmedi]` işaretleri kalkacak, yanlış bulunan satır düzeltilecek veya silinecek. 4'e "evet" gelirse yeni not `03-toplantilar/` altına alınıp story/risk/karar çıkarımı yapılacak.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- 1 ve 2 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 40 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi, workshop gündemi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-10 — Sabah brifingi (issue #20)

**Brifingte söylenenler:**
- Bugün Perşembe; PO haftalık ritminde paydaş güncelleme günü. Kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- 17 Eylül PlanItEarth workshop'una 7 gün kaldı; repoda hazırlık kaydı yok.
- Dünkü (issue #19) 4 sorunun tamamı cevapsız kaldı. İkisi ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- S-001 20 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- R-01 (metin olarak alınan SQL'in execute edilmesi) ve D-01 (Spark çıktısının OLTP'ye taşınma yolu) 10 gündür açık; ikisi de 31 Ağustos Architecture notundan çıkmıştı, hiçbiri Alper tarafından onaylanmadı.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 10. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 4 Eylül'den beri yeni içerik gelmedi (Alper'in son commit'i: 6a3560d). Son on üç brifing (issue #7–#19) cevapsız.

**Sorular ve cevaplar:**
1. S: Sprint 1 için hedef cümlesi taslağını ben yazayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: 17 Eylül PlanItEarth workshop'unda ap-action-management gündemde mi? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: 31 Ağustos Architecture notundan uçtan uca akış taslağını ben çıkarayım mı?
   C: *Cevap bekleniyor*
4. S: R-01'i aktif engel (blocker) olarak işaretleyeyim mi?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 8 Eylül ve 4 Eylül'de sorulup ikinci kez cevapsız kalan iki soru bekleyen sorular tablosuna taşındı: sizing için Big Data/Couchbase tarafına gidecek soru metni H başlığına (R-03'ün tek açık ucu), cevapsız soruların tek kontrol listesi issue'sunda toplanması I başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 36'dan 38 satıra çıktı; başlık sayıları (H 7, I 6) güncellendi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse Sprint 1 için iki alternatif hedef cümlesi bu issue'ya yazılacak, seçilen `00-proje/ekip-ve-ritim.md` ve aktif sprint kaydına işlenecek. 2'ye cevap gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler satırındaki `[teyit edilmedi]` kalkacak; "hayır" gelirse workshop hazırlığı takipten düşecek. 3'e "evet" gelirse 31 Ağustos notundaki akış tek sayfalık şemaya çevrilip `03-toplantilar/` altına yazılacak. 4'e "evet" gelirse R-01 aktif engel tablosuna blocker olarak taşınacak ve S-001'in bağımlılıklarına eklenecek.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- 1 ve 2 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 38 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-09 — Sabah brifingi (issue #19)

**Brifingte söylenenler:**
- Bugün Çarşamba; PO haftalık ritminde sprint hedefi günü. Kayıtlı tören yok, `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- Sprint 1 aktif görünüyor ama sprint hedefi ve bitiş tarihi yazılı değil; `02-sprintler/` altında klasör yok.
- Dünkü (issue #18) 5 sorunun tamamı cevapsız kaldı. Dördü ikinci kez sorulmuştu; kural gereği bugün `05-riskler-engeller.md` bekleyen sorular tablosuna taşındı ve bir daha sorulmayacak.
- S-001 19 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- R-01 (metin olarak alınan SQL'in execute edilmesi) ve D-01 (Spark çıktısının OLTP'ye taşınma yolu) 9 gündür açık; ikisi de 31 Ağustos Architecture notundan çıkmıştı, hiçbiri Alper tarafından onaylanmadı.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 9. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 17 Eylül PlanItEarth workshop'una 8 gün kaldı; repoda hazırlık kaydı yok.
- 4 Eylül'den beri yeni içerik gelmedi (son commit Alper'den: 6a3560d). Son on iki brifing (issue #7–#18) cevapsız.

**Sorular ve cevaplar:**
1. S: Sprint 1 için hedef cümlesi taslağını ben yazayım mı?
   C: *Cevap bekleniyor*
2. S: Sizing için Big Data ve Couchbase ekiplerine gidecek tek paragraflık soru metnini çıkarayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: Bugüne kadar cevapsız kalan 36 soruyu tek bir kontrol listesi issue'sunda toplayayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
4. S: 17 Eylül PlanItEarth workshop'unda ap-action-management gündemde mi?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 7 Eylül ve 8 Eylül'de sorulup iki kez cevapsız kalan dört soru bekleyen sorular tablosuna taşındı: D-01 kaydı ve bilgi güvenliği kaydı H başlığına, ikinci uçtan uca akış toplantısının tarihi A başlığına, S-001 parser kabul kriteri C başlığına. Kural gereği üçüncü kez sorulmuyorlar. Tablo 32'den 36 satıra çıktı; başlık sayıları (A 4, C 8, H 6) güncellendi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse Sprint 1 için iki alternatif hedef cümlesi bu issue'ya yazılacak, seçilen `00-proje/ekip-ve-ritim.md` ve aktif sprint kaydına işlenecek. 2'ye "evet" gelirse `04-raporlar/` altına Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan) tarafına gidecek sizing soru metni yazılacak. 3'e "evet" gelirse gruplanmış 36 soru tek bir kontrol listesi issue'suna dönüştürülecek. 4'e cevap gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler satırındaki `[teyit edilmedi]` kalkacak ve workshop hazırlığı açılacak.

**Açık kalanlar:**
- Yukarıdaki 4 sorunun tamamı. Cevap bekleniyor.
- 2 ve 3 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 36 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-08 — Sabah brifingi (issue #18)

**Brifingte söylenenler:**
- Bugün Salı; PO haftalık ritminde refinement'a girecek story'lerin kabul kriterlerini tamamlama günü. Şablon tören takviminde refinement Salı 14:00 görünüyor ama `00-proje/ekip-ve-ritim.md` hâlâ şablon değerlerinde; bugün gerçek bir tören var mı bilinmiyor [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- S-001 18 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor. Bugün refinement varsa gündemde konuşulabilecek başka madde yok.
- 31 Ağustos Architecture notundan çıkan iki bekleyen karar (D-01 aktarım bacağı, D-02 maintenance sahipliği) ve üç risk (R-01 metin SQL'in execute edilmesi, R-02 Kafka event yükü, R-03 sizing) tabloda duruyor; hiçbiri Alper tarafından onaylanmadı.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 8. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 17 Eylül PlanItEarth workshop'una 9 gün kaldı; repoda hazırlık kaydı yok.
- 4 Eylül'den beri yeni içerik gelmedi (son commit Alper'den: 6a3560d, Architecture notu). Son on bir brifing (issue #7–#17) cevapsız.

**Sorular ve cevaplar:**
1. S: D-01'i (Kafka event / ODI ara tablo) bekleyen karar olarak kayıtlı tutayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: Metin olarak gelen SQL'in execute edilmesi için bilgi güvenliğinden kayıt açıldı mı? (ikinci kez)
   C: *Cevap bekleniyor*
3. S: Ecem ve Dursun'un istediği ikinci uçtan uca akış toplantısı için tarih belirlendi mi? (ikinci kez)
   C: *Cevap bekleniyor*
4. S: S-001'in kabul kriterlerine sözdizimi doğrulaması (parser) maddesini ekleyeyim mi? (ikinci kez)
   C: *Cevap bekleniyor*
5. S: Sizing için Big Data ve Couchbase ekiplerine gidecek tek paragraflık soru metnini çıkarayım mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 4 Eylül ve 7 Eylül'de sorulup cevapsız kalan "Bu hafta ekip tarafında kapanan bir iş oldu mu?" sorusu B başlığı altına taşındı; kural gereği üçüncü kez sorulmuyor. B başlığı "Ekip, sahiplik ve ilerleme" olarak güncellendi, tablo 32 satıra çıktı.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "hayır" gelirse D-01 kaydı geri alınacak; "evet" gelirse karar sahibi yazılacak. 2'ye "hayır" gelirse R-01 aktif engel tablosuna blocker olarak taşınacak ve S-001'in bağımlılıklarına eklenecek. 3'e tarih gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna yazılacak. 4'e "evet" gelirse S-001'e sözdizimi doğrulaması kabul kriteri eklenecek. 5'e "evet" gelirse `04-raporlar/` altına Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan) tarafına gidecek sizing soru metni yazılacak.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 1, 2, 3 ve 4 numaralı sorular ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 32 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, gruplanmış soru tablosu, D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-07 — Sabah brifingi (issue #17)

**Brifingte söylenenler:**
- Bugün Pazartesi; PO haftalık ritminde backlog sıralaması ve hafta önceliği günü. Kayıtlı tören yok; `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi].
- **Yeni içerik geldi:** Alper 2026-09-04 23:21'de `03-toplantilar/20260831-Architecture.md` dosyasını yükledi (commit 6a3560d). 28 Ağustos'tan beri gelen ilk yeni içerik; S-001'in merkezine değiyor ve brifingin çoğu buradan çıktı.
- Nottan çıkan iki açık uç: (1) Spark çıktısının OLTP'ye taşınma yolu (Kafka event / ODI ara tablo) karara bağlanmadı — Gökçer Belgüsen event, Dursun Akçeşme ODI tarafında; (2) kullanıcıdan metin olarak alınan SQL'in execute edilmesi için bilgi güvenliğinden kayıt açılması gerekiyor.
- Notta uzlaşıya varılan taraf: okuma/gösterim 55-60 milyon müşteri-ürün kaydı için tek Couchbase collection'ında JSON döküman, TTL ile düşme, SQL++ ile okuma. Üretim Spark'a (Cloudera) alınıyor, DWH yalnız kaynak kalıyor, OLTP-DWH arası tüm alışveriş bulk.
- Sizing (kaç collection, kaç milyon döküman, ~1 KB JSON, ~20 TPS, subsecond) Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan) tarafıyla konuşulacaktı; sahibi ve tarihi yazılı değil. Ecem ve Dursun uçtan uca akış çizimi ve ikinci bir toplantı istedi — planlandığına dair kayıt yok.
- S-001 17 gündür Taslak (2026-08-21'den beri); backlog'daki tek story, 4 açık sorusu ve 2 bekleyen bağımlılığı var, Definition of Ready karşılanmıyor.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 7. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- 17 Eylül PlanItEarth workshop'una 10 gün kaldı; repoda hazırlık kaydı yok.
- Son on brifing (issue #7–#16) cevapsız.

**Sorular ve cevaplar:**
1. S: Kafka event / ODI ara tablo kararını "bekleyen karar" olarak kaydedeyim mi?
   C: *Cevap bekleniyor*
2. S: SQL'in execute edilmesi için bilgi güvenliğinden kayıt açıldı mı?
   C: *Cevap bekleniyor*
3. S: Ecem ve Dursun'un istediği ikinci uçtan uca toplantı için tarih belirlendi mi?
   C: *Cevap bekleniyor*
4. S: S-001'in kabul kriterlerine sözdizimi doğrulaması (parser) maddesini ekleyeyim mi?
   C: *Cevap bekleniyor*
5. S: Bu hafta ekip tarafında kapanan bir iş oldu mu? (ikinci kez)
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 31 Ağustos Architecture notundan bir bekleyen karar (D-01 aktarım bacağı) ve üç risk (R-01 metin SQL'in execute edilmesi, R-02 Kafka event yükü, R-03 sizing belirsizliği) yazıldı. D-02 olarak Account Planning maintenance süreç sahipliği eklendi (S-001'in zaten kayıtlı bağımlılığı). Gerekçe: iki tablo da şablon satırlarında duruyordu ve elimizde ilk kez gerçek içerik var. Kararın kimde olduğu ve olasılık/etki değerleri notta yazmıyor, `[teyit edilmedi]` bırakıldı. Alper onaylamadı.
- `05-riskler-engeller.md` → 3 Eylül'de ikinci kez sorulup cevapsız kalan "17 Eylül workshop gündem taslağı" sorusu H başlığı altına taşındı; kural gereği artık sorulmuyor. Tablo 31 satırda.
- `01-backlog/stories/S-001-...md` → Bağlam bölümüne 31 Ağustos Architecture notu eklendi; notun "kurgunun kalbi dinamik SQL'lerin koşturulması" ifadesi S-001'in merkezi olduğunu doğruluyor. Kabul kriterlerine dokunulmadı — parser maddesi Alper'in cevabı beklendiği için eklenmedi.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "hayır" gelirse D-01 kaydı geri alınacak; "evet" gelirse karar sahibi yazılacak. 2'ye "hayır" gelirse R-01 aktif engel tablosuna blocker olarak taşınacak ve S-001'in bağımlılıklarına eklenecek. 3'e tarih gelirse `00-proje/ekip-ve-ritim.md` önemli tarihler tablosuna yazılacak. 4'e "evet" gelirse S-001'e sözdizimi doğrulaması kabul kriteri eklenecek. 5'e cevap gelirse ekip ilerlemesine dair repodaki ilk kayıt açılacak.
- Ayrıca "sizing: evet" gelirse Big Data ve Couchbase ekiplerine gidecek tek paragraflık soru metni `04-raporlar/` altına yazılacak.

**Açık kalanlar:**
- Yukarıdaki 5 sorunun tamamı. Cevap bekleniyor.
- 5 numaralı soru ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 31 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, gruplanmış soru tablosu, bugünkü D-01/D-02 ve R-01…R-03 kayıtları, S-001 bağlam notu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

---

## 2026-09-04 — Sabah brifingi (issue #16)

**Brifingte söylenenler:**
- Bugün Cuma; PO haftalık ritminde hafta kapanışı günü (riskler güncellenir, paydaş ihtiyacına bakılır). Kayıtlı tören yok; `00-proje/ekip-ve-ritim.md` tören takvimi hâlâ şablon değerlerinde [teyit edilmedi]. Tören takvimi sorusu 3 kez sorulduğu için artık sorulmuyor.
- Sprint 1 aktif; sprint hedefi ve bitiş tarihi hâlâ yazılı değil, `02-sprintler/` altında klasör yok.
- S-001 14 gündür Taslak (2026-08-21'den beri); kabul kriterleri yazılı ama 4 açık soru ve 2 bekleyen bağımlılık nedeniyle Definition of Ready karşılanmıyor. Backlog'daki tek story bu; bir sonraki sprinti dolduracak hazır iş yok.
- 21 paydaşın hiçbirinde "son iletişim" kaydı yok; Ağustos turu kaçtı, Eylül'ün 4. günündeyiz. Taslak hazır: `04-raporlar/2026-08-31-paydas-guncellemesi-taslak.md` — gönderilmedi, karar Alper'de. Bu soru bekleyen sorular tablosunda olduğu için tekrar sorulmadı.
- `05-riskler-engeller.md`'de kayıtlı aktif engel yok [teyit edilmedi]; engel sorusu 2 kez sorulup cevaplanmadığı için takipten düştü.
- Onay beklemeden üretilen dört çıktı (5 epic, `oncelik.md` epic tablosu, paydaş taslağı, 17 Eylül tarih satırı) hâlâ "onaylanmadı" işaretli. Repoyu ekip görüyor.
- 17 Eylül PlanItEarth workshop'una 13 gün kaldı; repoda hazırlık kaydı yok.
- Son dokuz brifing (issue #7–#15) cevapsız — hiçbirine yorum gelmedi. Alper'in son commit'i 28 Ağustos (KickOff pptx yüklemesi).

**Sorular ve cevaplar:**
1. S: 17 Eylül workshop'u için gündem taslağı çıkarayım mı? (ikinci kez)
   C: *Cevap bekleniyor*
2. S: Bu hafta ekip tarafında kapanan bir iş oldu mu?
   C: *Cevap bekleniyor*
3. S: Bugüne kadar cevapsız kalan soruları tek bir kontrol listesi issue'sunda toplayayım mı?
   C: *Cevap bekleniyor*

**Bu brifingte asistanın yaptıkları (cevap beklemeden):**
- `05-riskler-engeller.md` → 3 Eylül'de ikinci kez sorulup cevapsız kalan üç soru (brifingi durdurma, S-001'i ikiye bölme, Umut/Garo'ya gidecek mesaj taslağı) "Cevap bekleyen sorular" tablosuna taşındı; kural gereği artık sorulmuyorlar. Tablo 30 satıra çıktı.
- `05-riskler-engeller.md` → 30 satırlık düz tablo dokuz konu başlığına gruplandı (A sprint/tören, B ekip, C S-001, D backlog/epic, E öncelik, F paydaş, G proje tanımı, H risk/engel, I brifing kanalı). Her başlığın altına "cevaplanmazsa ne oluyor" satırı yazıldı. Satırlar ve tarihleri değişmedi, yalnızca sıralandı. Gerekçe: 30 soru dokuz ayrı issue'ya dağılmış durumdaydı; başlık başlık cevaplanabilir hale getirildi. Alper onaylamadı.

**Bu cevaplardan çıkacak güncellemeler:**
- 1'e "evet" gelirse `03-toplantilar/20260917-PlanItEarth-Workshop.md` altına gündem taslağı eklenecek. 2'ye cevap gelirse hafta kapanışı kaydı ve ilerleme notu yazılacak — şu an repoda ekip ilerlemesine dair hiçbir veri yok. 3'e "evet" gelirse gruplanmış 30 soru tek bir kontrol listesi issue'suna dönüştürülecek.

**Açık kalanlar:**
- Yukarıdaki 3 sorunun tamamı. Cevap bekleniyor.
- 1 numaralı soru ikinci kez soruldu; bir sonraki brifingte cevap gelmezse üçüncü kez sorulmayacak ve bekleyen sorular tablosuna taşınacak.
- Bekleyen sorular tablosu 30 satırda, dokuz başlıkta. Sprint tarihleri, sprint hedefi, tören takvimi, ekip isimleri, epic onayı, paydaş bilgilendirmesi ve S-001'in "Hazır" durumu bu sorular cevaplanmadıkça ilerlemiyor.
- Onay beklemeden üretilen çıktılar (5 epic, epic tablosu, paydaş taslağı, 17 Eylül tarih satırı, gruplanmış soru tablosu) "onaylanmadı" işaretli. Alper reddederse geri alınacak.

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
