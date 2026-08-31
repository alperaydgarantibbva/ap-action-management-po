# E-05 — Aksiyon performansı RM, şube, bölge ve ürün seviyesinde izlenir (MONITOR)

| | |
|---|---|
| **Durum** | Fikir |
| **Hedef** | `[teyit edilmedi]` |
| **Sahip** | Reporting Owner — isim belirlenmedi `[teyit edilmedi]` |

## Ne ve neden

Aksiyon tamamlandığında sonucu merkezi yapıya dönmezse geri bildirim döngüsü kapanmıyor ve
skorlama olgunlaşmıyor. Bu epic bittiğinde tamamlanan aksiyonların durumu otomatik olarak
merkezi yapıya akıyor ve RM / şube / bölge / ürün kırılımında izlenebiliyor olacak.

## Başarı kriteri

Vizyondaki "Gerçek Zamanlı Aksiyon Güncelliği" kriteri: tamamlanan aksiyonlar gerçek zamanlıya
yakın ve otomatik olarak güncelleniyor.

## İçindeki story'ler

| ID | Başlık | Durum |
|---|---|---|
| — | Henüz story yazılmadı | — |

## Kaynak

- KickOff sunumu, MONITOR katmanı: Reporting Pool, RM / şube / bölge / ürün seviyesinde izleme
- Action Engine README'deki "gerçekleşen ve etki takibi" başlığı
- 17 Eylül PlanItEarth notu: her aksiyon tipi için canlı sistem ve/veya ODS'ten ayrı ODI veya
  Service Call geliştirilecek

## Kapsam dışı

- Yönetim raporlama ekranlarının Superbanker tarafındaki karşılıkları `[teyit edilmedi]`

## Riskler

- Vizyondaki kısıt: bazı kaynak sistemler gerçek zamanlı güncellemeyi teknik olarak desteklemiyor olabilir
- Aksiyon tipi başına ayrı entegrasyon eforu doğrusal büyüyor `[teyit edilmedi]`

## Açık kararlar

- "Gerçek zamanlıya yakın" hangi gecikme değeri olarak ölçülecek (dakika? saat? gün sonu?)

---

*Oluşturma: 2026-08-31 (asistan taslağı, Alper onaylamadı) · Son güncelleme: 2026-08-31*
