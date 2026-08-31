# Backlog Sıralaması

> **Neden bu dosya var:** Sıralamanın *gerekçesi* yazılı değilse her toplantıda yeniden tartışılır. Bir satırlık gerekçe, saatlerce tartışmayı önler.

## Sıralama

| # | ID | Başlık | Durum | Neden bu sırada | Hedef sprint |
|---|---|---|---|---|---|
| 1 | [S-001](stories/S-001-aksiyon-sql-tanimi-sistem-uzerinden.md) | Aksiyon sorumlusu tanım SQL'ini sistem üzerinden gönderip durumunu takip edebilir | Taslak | 19 Ağustos Pusula görüşmesinde "sistem üzerinden sürece dönüştürülmeli" diye açıkça istendi; aksiyon havuzunu besleyen akışın önkoşulu | `[teyit edilmedi]` |
| 2 | | | | | |
| 3 | | | | | |

*Sıralama Alper tarafından onaylanmadı — S-001 backlog'daki tek kayıt olduğu için 1. sıraya yazıldı.*

## Epic yapısı

*(2026-08-31'de asistan tarafından KickOff sunumundaki 5 katmandan çıkarıldı. Alper onaylamadı.
Sıra, sunumdaki katman akışıdır — değer sırası değil.)*

| ID | Epic | Vizyondaki başarı kriteri | İçindeki story |
|---|---|---|---|
| [E-01](epics/E-01-capture-sinyal-toplama.md) | Sinyaller dört kaynaktan tek havuzda toplanır | Sinyal Kanallarının Konsolidasyonu | — |
| [E-02](epics/E-02-transform-aksiyon-uretimi.md) | Sinyaller sistem üzerinden çalıştırılabilir aksiyona dönüşür | Merkezi Aksiyon Yönetimi | S-001 |
| [E-03](epics/E-03-prioritize-skorlama.md) | Aksiyonlar skorlanarak önceliklendirilir | Aksiyon Önceliklendirme | — |
| [E-04](epics/E-04-activate-yasam-dongusu.md) | Aksiyonlar A/B testli çalıştırılır, yaşam döngüsü takip edilir | A/B Test Yetkinliği + Yaşam Döngüsü Yönetimi | — |
| [E-05](epics/E-05-monitor-performans-izleme.md) | Aksiyon performansı RM/şube/bölge/ürün seviyesinde izlenir | Gerçek Zamanlı Aksiyon Güncelliği | — |

**Durum tanımları:**
- **Hazır** — Kabul kriterleri yazılı, ekip anladı, sprinte alınabilir.
- **Taslak** — Fikir var, kabul kriterleri eksik. Refinement'a girmeli.
- **Beklemede** — Bir karara, bir bağımlılığa veya bir paydaş cevabına takılı. Nedeni "Neden bu sırada" sütununda yazmalı.

## Sıralama kriterleri

*(Bu projede neye göre önceliklendiriyoruz? Bir kez yazın, sonra her tartışmada buraya bakın.)*

1. `[örn. Yasal/uyum zorunluluğu olan işler önce]`
2. `[örn. En çok kullanıcıyı etkileyen iş]`
3. `[örn. Diğer işleri açan bağımlılık]`
4. `[örn. Teknik risk — erken denenmeli]`

## Bilinçli olarak ertelenenler

*(Yapılmayacak değil, şimdilik yapılmayacak olanlar. Paydaş "buna ne oldu?" diye sorduğunda buraya bakın.)*

| ID | Başlık | Neden ertelendi | Ne zaman yeniden bakılacak |
|---|---|---|---|
| | | | |

---

*Son güncelleme: `[tarih]`*
