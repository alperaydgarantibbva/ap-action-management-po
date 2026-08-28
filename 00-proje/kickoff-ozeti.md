# KickOff Sunumu — Metin Özeti

> **Kaynak:** `ActionPlanning-ActionManagement-KickOff-202709.pptx` (Alper, 2026-08-28 yükledi, 16 slayt).
> Bu dosyayı asistan sunumun metninden çıkardı. Amaç: pptx bir binary dosya, repoda aranamıyor
> ve story yazarken referans verilemiyordu. Aşağıdaki başlıklar sunumdaki ifadelerdir;
> yorum eklenmemiştir. Yorum gerektiren yerler `[teyit edilmedi]` ile işaretlendi.

## Konumlandırma

Account Planning — "AI-Native Portfolio Management Platform".

Ölçek: 616K+ müşteri (SME + BEI), ~1.900 RM, portföylerin %50+'sinde yeniden atama.

Tarif edilen dört problem: dağınık araç ve veri, kaybolan kurumsal hafıza, belirsiz aksiyon
öncelikleri, zayıf geri bildirim döngüsü. Hedef: portföy yönetimini raporlama odaklıdan
aksiyon odaklıya taşımak.

## Step 1 — Action Management (bu sürümün kapsamı)

Sunum bu modülü **5 katman, 4 engine, 4 havuz** olarak tarif ediyor. Ölçek notu: 30+ analitik
model, 200+ ayrık sinyal.

| # | Katman | Ne yapar | Havuz | Sahiplik rolleri |
|---|---|---|---|---|
| 1 | CAPTURE | 4 kaynaktan sinyal toplama: modeller, SQL'ler, Excel yükleme, RM girişi | Signal Pool | Signal Owner |
| 2 | TRANSFORM | Sinyalleri zenginleştirme SQL'leri ile çalıştırılabilir aksiyona çevirme | Action Pool / Action Library | Action Owner |
| 3 | PRIORITIZE | Skorlama motoru: RM KPI'ları, organizasyonel öncelikler, müşteri eğilimi, karlılık (her biri %25) | — | Strategic Priority Owner, Performance Owner |
| 4 | ACTIVATE | A/B test split (%10 kontrol / %90 uygulama), gerçekleşme takibi | Lifecycle Pool / Realization Library | A/B Test Owner, Action Owner |
| 5 | MONITOR | RM / şube / bölge / ürün seviyesinde performans izleme ve geri besleme | Reporting Pool | Performance Owner, Reporting Owner |

Her katmanda ortak yönetişim başlıkları tekrarlanıyor: Quality Control ve Audit / Change Management.

## Backlog açısından önemli iki nokta

- **TRANSFORM katmanı S-001 ile birebir örtüşüyor.** Sunum bu adımı şöyle tarif ediyor:
  "SQL Queries prepared by Action Owners → Queries are checked and approved systematically →
  Queries are scheduled to run periodically → Qualified queries are stored into the Action Library."
  S-001'in kabul kriterleri bu dört adımın ilk üçünü kapsıyor.
- **Altı sahiplik rolü tanımlı ama isimler sunumda yok:** Signal Owner, Action Owner,
  Strategic Priority Owner, A/B Test Owner, Performance Owner, Reporting Owner.
  S-001'deki "kontrolör kim" sorusu Action Owner rolüne bağlı. `[teyit edilmedi]`

## Kapsam dışı olarak konumlanan başlıklar (slayt 15 — "Next Steps")

RM Co-Pilot ve Auto-Pilot yetenekleri: müşteri/portföy özetleyiciler, sektörel içgörüler,
chatbot'lar, uzman danışmanlar, agentic pipeline, toplantı hazırlığı ve sesli not asistanları.
Bunlar `00-proje/vizyon.md`'deki "bu sürümde hedeflenmeyen" maddesiyle uyumlu.

---

*Oluşturma: 2026-08-28 · Asistan tarafından sunum metninden çıkarıldı, Alper onaylamadı.*
