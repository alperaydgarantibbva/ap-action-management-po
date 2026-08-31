# E-01 — Sinyaller dört kaynaktan tek havuzda toplanır (CAPTURE)

| | |
|---|---|
| **Durum** | Fikir |
| **Hedef** | `[teyit edilmedi]` |
| **Sahip** | Signal Owner — isim belirlenmedi `[teyit edilmedi]` |

## Ne ve neden

Bugün sinyaller analitik modellerden, SQL listelerinden, Excel dosyalarından ve RM notlarından
birbirinden bağımsız akıyor; ortak bir yapıya girmediği için takip edilemiyor. Bu epic bittiğinde
dört kaynağın tamamı aynı Signal Pool'a yazıyor olacak.

## Başarı kriteri

Vizyondaki "Sinyal Kanallarının Konsolidasyonu" kriteri: 4 ana sinyal kanalının tamamı ortak
yapıya aktarılabiliyor.

## İçindeki story'ler

| ID | Başlık | Durum |
|---|---|---|
| — | Henüz story yazılmadı | — |

## Kaynak

- KickOff sunumu, CAPTURE katmanı → `../../00-proje/kickoff-ozeti.md`
- Action Engine README'deki "sinyal yönetimi" başlığı
- 17 Eylül PlanItEarth notu: her sinyal tipi için ayrı ODI veya Servis Call geliştirilecek

## Kapsam dışı

- Yapay zeka eklentileri (vizyonda kapsam dışı)

## Riskler

- Sinyal başına ayrı entegrasyon geliştirilmesi eforu doğrusal büyütüyor `[teyit edilmedi]`
- Sinyal geçerlilik süresi tanımı (signal definition) veri modeline girmemişse aksiyon üretimi yanlış zamanlanır

## Açık kararlar

- Signal Owner rolünü kim üstlenecek
- İlk sürümde dört kanalın hangisi önce devreye alınacak

---

*Oluşturma: 2026-08-31 (asistan taslağı, Alper onaylamadı) · Son güncelleme: 2026-08-31*
