# PO Çalışma Alanı — ap-action-management

Bu repo, ürün sahibi (PO) çalışmasının **arka planını** tutar: neden bu işi yapıyoruz, kime söz verdik, neye karar verdik, neyi ertelemeye karar verdik.

> **Henüz kurulum yapılmadıysa:** [KURULUM.md](KURULUM.md) — 3 adım, ~10 dakika.

## Burada bir asistan çalışıyor

Bu repoda GitHub Actions üzerinde çalışan bir PO asistanı var. Hafta içi her sabah 08:30'da bir brifing issue'su açar; PO cevaplar; asistan cevapları ilgili dosyalara işler ve commit atar.

`PO Asistani` imzalı commit görürseniz kaynağı budur. Asistanın davranış kuralları [ASISTAN.md](ASISTAN.md) dosyasında yazılı ve herkese açık.

## Jira ile ilişkisi

| | Jira | Bu klasör |
|---|---|---|
| **Ne tutar** | İşin kendisi: story'ler, durumlar, atamalar, sprint panosu | İşin arkasındaki düşünce: gerekçe, karar, bağlam, paydaş beklentisi |
| **Gerçeğin kaynağı** | İş durumu ve ilerleme için | Karar ve gerekçe için |
| **Kim günceller** | Ekip | PO (asistan desteğiyle) |

**Çakışma olursa:** İşin *durumu* için Jira geçerlidir. İşin *nedeni* için burası geçerlidir.

Bu klasör Jira'nın yerine geçmez ve Jira'dan veri kopyalamaz. Story'ler burada yazılıp olgunlaştırılır, hazır olduğunda Jira'ya taşınır.

## Klasör haritası

```
po/
├── ASISTAN.md              → Asistanın çalışma talimatları
├── 00-proje/
│   ├── vizyon.md           → Ürün vizyonu, hedefler, başarı kriterleri
│   ├── paydaslar.md        → Paydaş haritası ve iletişim planı
│   ├── ekip-ve-ritim.md    → Ekip, törenler, takvim
│   └── kararlar.md         → Karar günlüğü (kronolojik, silinmez)
├── 01-backlog/
│   ├── oncelik.md          → Sıralama ve gerekçesi
│   ├── epics/              → Büyük iş parçaları
│   └── stories/            → Her story ayrı dosya
├── 02-sprintler/
│   └── sprint-NN/          → Plan, refinement notları, günlük log, review hazırlığı
├── 03-toplantilar/         → YYYY-AA-GG-toplanti-adi.md
├── 04-raporlar/            → Paydaş güncellemeleri, yönetim özetleri
├── 05-riskler-engeller.md  → Açık riskler, blocker'lar, bekleyen kararlar
├── 06-po-gunlugu.md        → Günlük brifing soru-cevapları
└── _sablonlar/             → Boş şablonlar
```

## Ekip için notlar

- **Okumaya değer ilk üç dosya:** `00-proje/vizyon.md`, `01-backlog/oncelik.md`, `05-riskler-engeller.md`.
- **Bir kararın nedenini merak ediyorsanız** `00-proje/kararlar.md` dosyasına bakın. Kararlar tarih sırasıyla ve gerekçeleriyle durur.
- **Bir story'nin neden böyle yazıldığını** anlamak için `01-backlog/stories/` altındaki ilgili dosyaya bakın; kabul kriterleri ve açık sorular orada.
- **Katkı vermek isterseniz** doğrudan düzenleyip commit atabilirsiniz. Karar niteliğindeki değişiklikler için `kararlar.md` dosyasına da bir satır ekleyin.

## Yazım kuralları

- Dosyalar Markdown, Türkçe.
- Tarih formatı: `YYYY-AA-GG` (örn. 2026-08-16).
- Story dosya adı: `S-NNN-kisa-baslik.md` (örn. `S-014-toplu-aksiyon-atama.md`).
- Epic dosya adı: `E-NN-kisa-baslik.md`.
- Hiçbir şey silinmez; geçersiz kalan içerik `~~üstü çizili~~` yapılır veya "Durum: iptal" notu düşülür.
