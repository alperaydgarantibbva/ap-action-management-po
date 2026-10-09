# Karar Günlüğü

Verilen kararlar, gerekçeleriyle birlikte. **En yeni en üstte.** Buradan hiçbir şey silinmez; karar değiştiyse yeni bir kayıt açılır ve eskisine "Durum: değişti → [tarih]" notu düşülür.

Bu dosyanın amacı: 3 ay sonra "biz bunu neden böyle yapmıştık?" sorusuna 30 saniyede cevap verebilmek.

---

## K-002 — Sabah brifingi yalnızca Pazartesi ve Cuma açılacak

- **Tarih:** 2026-08-21
- **Karar:** Sabah brifingi her iş günü değil, yalnızca Pazartesi ve Cuma açılacak.
- **Gerekçe:** Alper'in yoğunluğu; günlük brifing cevaplanamıyor. Alper'in kendi ifadesi: "Pazartesi ve Cuma olsun", "her pazartesi ve cuma".
- **Alternatifler:** Yalnızca Pazartesi (asistan önerdi, Alper Cuma'yı da ekledi); brifingi duraklatmak.
- **Kim verdi:** Alper — cevabı issue yerine doğrudan `06-po-gunlugu.md`'nin 2026-08-20 kaydına yazdı (commit c5329e2).
- **Etkilenen:** `ASISTAN.md` bölüm 3, `.github/workflows/po-sabah-brifingi.yml` cron satırı
- **Durum:** Aktif. Asistan bu cevabı 2026-10-09'a kadar fark etmedi ve 7 hafta boyunca her gün brifing açtı. 2026-10-09'da `ASISTAN.md`'ye kural eklendi. Cron satırının `'30 5 * * 1,5'` yapılması Alper'de, çünkü bot tarafından değiştirilen cron workflow'u çalıştırmıyor.

---

## K-001 — PO çalışma alanı GitHub'da tutulacak

- **Tarih:** 2026-08-16
- **Karar:** Backlog notları, toplantı notları, paydaş planı ve sprint hazırlıkları `po/` klasöründe, Markdown olarak tutulacak. Jira iş takibi için gerçeğin kaynağı olmaya devam edecek.
- **Gerekçe:** Kurumsal Jira şirket ağı dışına kapalı; PO'nun dışarıdan erişebileceği ve bir asistanla birlikte çalışabileceği tek ortam GitHub.
- **Alternatifler:** Yerel bilgisayarda dosya (telefondan erişilemez, ekip göremez), harici bir uygulama (veri GitHub dışına çıkar).
- **Kim verdi:** Alper
- **Durum:** Aktif

---

<!--
Yeni karar eklerken bu şablonu kullan:

## K-NNN — [Kararın tek cümlelik özeti]

- **Tarih:** YYYY-AA-GG
- **Karar:** [Ne karar verildi]
- **Gerekçe:** [Neden. Bu satır en önemlisi.]
- **Alternatifler:** [Nelere hayır dendi ve neden]
- **Kim verdi:** [İsim]
- **Etkilenen:** [Story/epic/paydaş]
- **Durum:** Aktif / Değişti → K-NNN / İptal
-->
