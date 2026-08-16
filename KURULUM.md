# Kurulum — 3 Adım

Asistanı canlıya almak için yapılması gerekenler. Toplam süre: ~10 dakika. Bir kez yapılır.

## Adım 1 — API anahtarını repoya ekle

GitHub'da bu repo → **Settings** → **Secrets and variables** → **Actions** → **New repository secret**

| Alan | Değer |
|---|---|
| Name | `ANTHROPIC_API_KEY` |
| Secret | `sk-ant-...` (mevcut Anthropic API anahtarınız) |

**Add secret** deyin. Bu anahtar şifreli saklanır, log'larda görünmez, repoyu klonlayanlar okuyamaz.

## Adım 2 — Actions'a yazma izni ver

Repo → **Settings** → **Actions** → **General** → en alttaki **Workflow permissions**

- **Read and write permissions** seçeneğini işaretleyin
- **Save** deyin

Bu olmadan asistan repoya commit atamaz ve issue açamaz.

## Adım 3 — Test edin

Repo → **Actions** sekmesi → soldaki listeden **PO Sabah Brifingi** → sağdaki **Run workflow** → **Run workflow**

1-2 dakika içinde **Issues** sekmesinde "PO Brifingi — [tarih]" başlıklı bir issue açılmış olmalı.

Açılmadıysa Actions sekmesindeki çalışma kaydına tıklayıp hatayı okuyun. En sık iki sebep: anahtar yanlış girilmiş, veya Adım 2 atlanmış.

---

# Günlük kullanım

## Telefonda kurulum (bir kez)

1. **GitHub** uygulamasını indirin, `alperaydgarantibbva` hesabıyla girin
2. Repo sayfasında sağ üstteki **Watch** → **All Activity** seçin
3. Uygulama ayarlarından bildirimleri açın

Artık her sabah 08:30'da telefonunuza bildirim düşecek.

## Nasıl çalışır

**Sabah:** Bildirim gelir → issue'yu açarsınız → 4 başlık görürsünüz: Durum, Dikkat, Sorular, Bugün.

**Cevap:** Issue'ya yorum yazarsınız. Kısa olabilir:

```
1: evet
2: 26 Ağustos
3: hayır, Ahmet'e sordum bekliyorum
4: bugün yapamam, yarın
```

**1-2 dakika sonra:** Asistan cevaplarınızı ilgili dosyalara işler, commit atar, kısa bir özet yorumu yazar ve issue'yu kapatır.

## Görev vermek

Yeni bir issue açıp ne istediğinizi yazın. Örnekler:

> Toplu aksiyon atama özelliği için story yaz. Kullanıcılar 50'ye kadar kaydı seçip tek seferde atayabilmeli.

> Salı refinement'ı için gündem hazırla, hangi story'leri konuşmalıyız?

> Yönetime gönderilecek sprint özeti taslağı çıkar.

> "Definition of Ready" ne demek, bizim projede ne olmalı?

Asistan 1-2 dakikada cevaplar ve gerekiyorsa dosyaları oluşturur.

## Davranışını değiştirmek

Asistanın nasıl davrandığını değiştirmek isterseniz `ASISTAN.md` dosyasını düzenleyin — workflow dosyalarına dokunmanıza gerek yok. Örnekler:

- Brifing çok uzunsa: "en fazla 3 soru sor" yazın
- Saat değişsin: `.github/workflows/po-sabah-brifingi.yml` içindeki `cron: '30 5 * * 1-5'` satırını değiştirin (UTC yazılır; İstanbul saatinden 3 saat çıkarın)
- Hafta sonu da çalışsın: `1-5` yerine `*` yazın

## Maliyet

| Kalem | Beklenen |
|---|---|
| Anthropic API | Ayda ~$10-25 (günde 1 brifing + birkaç cevap turu) |
| GitHub Actions | Ücretsiz kotanın içinde (~200 dk/ay kullanır, kota 2000 dk) |

API kullanımını console.anthropic.com üzerinden izleyebilirsiniz.

## Durdurmak / duraklatmak

- **Geçici:** Actions sekmesi → workflow → sağ üstteki **⋯** → Disable workflow
- **Kalıcı:** `.github/workflows/` klasörünü silin

---

# Sorun giderme

| Belirti | Sebep | Çözüm |
|---|---|---|
| Sabah issue açılmıyor | Adım 2 atlanmış | Workflow permissions → Read and write |
| "Bad credentials" hatası | API anahtarı yanlış | Secret'ı silip yeniden ekleyin |
| Yorumuma cevap gelmiyor | Yorum sahibi repo sahibi değil | `alperaydgarantibbva` hesabıyla yorum yazın |
| Asistan iki kez cevaplıyor | Bot döngüsü | `po-asistan.yml` içindeki `if:` bloğunu kontrol edin |
| Cron saati kaymış | UTC/İstanbul karışıklığı | İstanbul saatinden 3 saat çıkarıp yazın |
| Brifing içeriği boş/genel | Repo dosyaları boş | `00-proje/` altındaki dosyaları doldurun |

**Not:** GitHub'ın cron zamanlaması yoğun saatlerde birkaç dakika gecikebilir. 08:30 yerine 08:35'te gelmesi normaldir.
