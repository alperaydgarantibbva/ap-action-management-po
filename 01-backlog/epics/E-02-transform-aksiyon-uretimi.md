# E-02 — Sinyaller sistem üzerinden çalıştırılabilir aksiyona dönüşür (TRANSFORM)

| | |
|---|---|
| **Durum** | Fikir |
| **Hedef** | `[teyit edilmedi]` |
| **Sahip** | Action Owner — isim belirlenmedi `[teyit edilmedi]` |

## Ne ve neden

Aksiyon tanım SQL'leri bugün ortak klasöre elle bırakılıyor; kim ne gönderdi, çalıştı mı,
onaylandı mı takip edilemiyor. Bu epic bittiğinde SQL'ler sistem üzerinden gönderiliyor,
sistemsel kontrolden geçiyor, periyodik çalışacak şekilde planlanıyor ve Action Library'ye
kaydediliyor olacak.

## Başarı kriteri

Vizyondaki "Merkezi Aksiyon Yönetimi" kriteri: aksiyon tanımlama ve oluşturma süreçlerinin
%100'ü merkezi yapı üzerinden yürüyor.

## İçindeki story'ler

| ID | Başlık | Durum |
|---|---|---|
| [S-001](../stories/S-001-aksiyon-sql-tanimi-sistem-uzerinden.md) | Aksiyon sorumlusu tanım SQL'ini sistem üzerinden gönderip durumunu takip edebilir | Taslak |

## Kaynak

- KickOff sunumu, TRANSFORM katmanı: "SQL Queries prepared by Action Owners → checked and approved
  systematically → scheduled to run periodically → stored into the Action Library"
- 19 Ağustos Pusula II görüşmesi: "sistem üzerinden sürece dönüştürülmeli"

## Kapsam dışı

- Skorlama ve önceliklendirme (E-03)

## Riskler

- Manuel SQL yolu kapatılmazsa iki yol paralel yürür ve merkezi yapı boş kalır (soru cevapsız)
- 2 milyon satır limiti Action Engine README 3.3'te geçiyor, S-001'in kabul kriterlerinde yok

## Açık kararlar

- S-001'deki geliştirme Account Planning tarafında mı, GT Pusula tarafında mı yapılacak
- "Sistemsel onay" adımını hangi rol yapacak

---

*Oluşturma: 2026-08-31 (asistan taslağı, Alper onaylamadı) · Son güncelleme: 2026-08-31*
