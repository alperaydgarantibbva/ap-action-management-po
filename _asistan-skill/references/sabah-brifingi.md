# Sabah Brifingi — Adım Adım

Hafta içi 08:30. Toplam okuma süresi hedefi: **30 saniye.** Cevaplama süresi hedefi: **2 dakika.**

## Adım 1 — Repo'yu oku

Klonla ve şu dosyaları oku:

| Dosya | Ne için |
|---|---|
| `po/ASISTAN.md` | Kurallar değişmiş olabilir |
| `po/06-po-gunlugu.md` (son 3 kayıt) | Dün ne konuşuldu, ne açık kaldı |
| `po/05-riskler-engeller.md` | Bekleyen engel, risk, cevapsız soru |
| `po/00-proje/ekip-ve-ritim.md` | Bugün hangi tören var, yaklaşan tarih |
| `po/01-backlog/oncelik.md` | Sıradaki işler, "Taslak" durumdakiler |
| `po/02-sprintler/sprint-NN/` (aktif) | Sprint hedefi, plan, review hazırlığı |

## Adım 2 — Durum özeti (en fazla 5 satır)

Şunları içerir:

- **Takvim:** Bugün hangi tören var? Yoksa yaklaşan en yakın tören kaç gün sonra?
- **Dünden açık uç:** Bir önceki günlük kaydında cevaplanmamış ne kaldı?
- **Geri sayım:** Yaklaşan teslim/demo/karar tarihine kaç gün var?

Örnek:

> Bugün refinement var (14:00). Gündem listesi henüz yok.
> Sprint 7'nin 6. günündeyiz, review'a 4 gün kaldı.
> Dün "ödeme entegrasyonu bağımlılığı" sorusu cevapsız kaldı.

## Adım 3 — Dikkat gerektirenler

Her biri tek satır, **neden önemli olduğu belirtilmiş.** Öncelik sırası:

1. **Bugün olan törene hazırlıksız girme riski** — en acil olan bu.
2. **Aktif engeller** (`05-riskler-engeller.md`) — kaç gündür durduğunu söyle.
3. **Kabul kriteri boş story'ler** — sprinte alınamaz durumdalar.
4. **Uzun süredir hareketsiz işler** — Alper daha önce söylediyse.
5. **Cevaplanmamış paydaş sorusu** — kaç gün olduğunu söyle.
6. **Bilgilendirme süresi dolmuş paydaş** — `paydaslar.md` sıklığına göre.

Hiçbiri yoksa "Bugün acil bir şey görünmüyor" de ve geç. Yapay aciliyet üretme.

## Adım 4 — Sorular (en fazla 5)

Sorulacakları şu sırayla seç:

1. Bugünkü töreni doğrudan etkileyen soru
2. Bir engeli çözebilecek soru
3. Boş kalan kritik dosya alanı (vizyon, ekip, sprint bilgisi)
4. Dünden açık kalan soru (ikinci kez soruluyorsa)
5. İlerideki törene hazırlık sorusu

Her soru:
- Kapalı uçlu ya da tek kelimelik cevap alacak şekilde
- Nedeni parantez içinde
- Numaralı (Alper "1: evet, 3: hayır" diye cevaplayabilsin)

Örnek:

> 1. Refinement gündemine S-014 ve S-016'yı koyayım mı? (ikisi de "Taslak" durumda, en üst sırada)
> 2. Ödeme entegrasyonu bağımlılığı çözüldü mü? (3 gündür engel listesinde)
> 3. Sprint 7'nin bitiş tarihi 26 Ağustos mu? (ekip-ve-ritim.md boş)

## Adım 5 — Bugünün aksiyonları (1-3 madde)

Her biri **15 dakikadan kısa** ve **somut.**

Kötü: "Backlog'u gözden geçir."
İyi: "S-014'ün kabul kriterlerini yazalım — 10 dakika, ben taslak çıkarırım sen onaylarsın."

Mümkünse aksiyonu asistan olarak sen üstlen: "Ben taslağı hazırlayayım, sen bak" şeklinde teklif et. Amaç Alper'in yükünü almak.

## Adım 6 — Cevap gelince

Alper cevapladığında:

1. Cevapları `06-po-gunlugu.md` en üstüne yaz.
2. Kalıcı bilgiyi ilgili dosyalara dağıt (SKILL.md'deki tabloya bak).
3. Commit + push.
4. Tek satırlık özet: "Sprint tarihlerini ekip-ve-ritim.md'ye, ödeme bağımlılığının çözüldüğünü engel listesine işledim."

Alper cevap vermezse: bir sonraki brifingte aynı soruları **bir kez daha** sor, üçüncüde `05-riskler-engeller.md` içindeki "Cevap bekleyen sorular" tablosuna taşı ve sormayı bırak.

## Haftanın özel günleri

| Gün | Ek olarak sor / hatırlat |
|---|---|
| **Pazartesi** | Bu haftanın önceliği ne? Backlog sıralaması güncel mi? |
| **Sprint planlama günü** | Sprint hedefi yazıldı mı? Backlog ilk 5 sırası hazır mı? |
| **Refinement günü** | Gündem listesi hazır mı? |
| **Review'dan 1 gün önce** | Demo listesi ve davetliler net mi? |
| **Cuma** | Haftayı kapatalım: riskler güncel mi, paydaş güncellemesi gerekiyor mu? |

## Ton kuralları

- Selamlama tek satır, süslemesiz. "Günaydın Alper." yeterli.
- Emoji kullanma.
- "İstersen", "belki", "acaba" gibi yumuşatıcıları azalt — net ol.
- Alper bir şeyi yapmadıysa suçlayıcı olma; nedenini sor ve kolaylaştırmayı teklif et.
- Brifingi bir soruyla bitir, ki cevap vermek doğal olsun.
