# 17 Eylül PlanItEarth Workshop — Hazırlık Notu (TASLAK)

> **Durum: Alper onaylamadı.** Bu notu asistan 2026-09-14'te, workshop'a 3 gün kala
> hazırladı. Kaynak: `20260917-PlanItEarth-Workshop.md` ve `20260831-Architecture.md`.
> Workshop'un takvimde durup durmadığı ve ap-action-management'ın gündemde olup
> olmadığı **[teyit edilmedi]** — iki kez soruldu, cevap gelmedi.
> Alper "gerek yok" derse bu dosya silinecek.

## Amaç

31 Ağustos Architecture toplantısında açık kalan iki konu (aktarım bacağı kararı,
güvenlik kaydı) 14 gündür kararsız duruyor. Bu workshop, o toplantıda Ecem Ekenoğlu
ve Dursun Akçeşme'nin istediği "uçtan uca akış + tüm ekipler bir arada" toplantısının
yerine geçebilir. PO olarak buraya çözüm değil, **karar alınacak soru listesi** ile
gidilir — kararı teknik sahipler verir.

## Önerilen gündem (60 dk)

| Süre | Konu | Çıktı |
|---|---|---|
| 10 dk | Uçtan uca akış: DWH → Spark → (?) → OLTP → Couchbase → ARC ekranları | Akışın tek sayfada ortak kabulü |
| 15 dk | **D-01 — Aktarım bacağı:** Kafka event mi, DWH ara tablo + ODI mi? | Karar ve karar sahibi |
| 10 dk | **R-01 — Güvenlik:** metin SQL'in execute edilmesi için bilgi güvenliği kaydı | Kaydı kimin açacağı + tarih |
| 10 dk | **R-03 — Sizing:** collection sayısı, döküman sayısı, ~1 KB JSON, ~20 TPS, subsecond | Big Data / Couchbase tarafına gidecek soru metni ve sahibi |
| 10 dk | **D-02 — Account Planning maintenance süreç sahipliği** | İsim |
| 5 dk | Kapanış: kim ne yapacak, bir sonraki toplantı gerekli mi | Aksiyon listesi |

## Workshop'ta cevabı alınması gereken 6 soru

Bunlar cevaplanırsa repodaki 2 bekleyen karar ve 3 risk kapanır ya da netleşir.

1. Spark çıktısı OLTP'ye nasıl taşınacak — Kafka event mi, DWH'ta günlük sil-boşalt
   ara tablodan ODI aktarımı mı? Bu kararı kim veriyor? (D-01)
2. Kafka seçilirse 50 binlik partiler kuralı yeterli mi, 1 milyon event için hedef
   süre ne? (R-02)
3. Metin olarak alınan SQL'in execute edilmesi için bilgi güvenliğinden kayıt açıldı
   mı; açılmadıysa kim açacak? (R-01)
4. Ecem Ekenoğlu'nun önerdiği sözdizimi doğrulaması (parser) kapsamda mı — S-001'in
   kabul kriterine girmeli mi? (S-001)
5. Sizing için Big Data (Can Tezgöçer, Veysel) ve Couchbase (İlhami, Adem Arslan)
   tarafına soru kim soracak, ne zaman? (R-03)
6. Account Planning maintenance sürecinin sahibi kim? (D-02 — S-001'in bağımlılığı)

## PO olarak yapmayacakların

- Teknik kararı sen verme; kararı **kimin** vereceğini ve **ne zaman** vereceğini yazıya bağla.
- Tahmin/efor sorma — ekip verir.
- Yeni kapsam açılırsa ("Mikro da dahil olsun", "superbanker entegrasyonu") sprint
  hedefine hizmet etmiyorsa backlog'a al, aynı toplantıda karara bağlama.

## Workshop sonrası (asistan yapar)

- Notu `03-toplantilar/` altına al, karar çıkanları `00-proje/kararlar.md`'ye,
  risk/engel çıkanları `05-riskler-engeller.md`'ye dağıt.
- D-01 ve D-02 kapanırsa bekleyen kararlar tablosundan "Kapanmış maddeler"e taşı.
- S-001'in açık soruları kapanırsa Definition of Ready kontrolünü tekrar çalıştır.

---

*Oluşturma: 2026-09-14 — asistan taslağı, onay bekliyor.*
