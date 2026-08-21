# S-001 — Aksiyon sorumlusu tanım SQL'ini sistem üzerinden gönderip durumunu takip edebilir

| | |
|---|---|
| **Durum** | Taslak |
| **Epic** | `[atanmadı]` |
| **Jira** | `[hazır olduğunda]` |
| **Tahmini büyüklük** | `[ekip verecek]` |
| **Hedef sprint** | `[teyit edilmedi]` |

> Bu taslağı asistan yazdı (2026-08-21). Kaynak: `03-toplantilar/20260819-Pusula-II.md` ve
> `03-toplantilar/20260917-PlanItEarth-Workshop.md`. Alper onaylamadan "Hazır" sayılmaz.

## Kim, ne, neden

**Kim olarak** aksiyon/sinyal sorumlusu (iş birimi)
**Şunu yapabilmek istiyorum:** tanım SQL'imi ortak klasöre dosya bırakarak değil, sistem üzerinden gönderip hangi aşamada olduğunu görebilmek
**Çünkü:** bugün sürecin nerede takıldığı, kimin hangi sürümü gönderdiği ve neden reddedildiği kayıt altında değil; her geçiş elle takip ediliyor

## Bağlam

19 Ağustos Pusula II görüşmesinde Umut Özdemir ve Garo Üçkardeş, metrik SQL'lerinin
"manuel ortak folder'a bırakılan dosyalar" ile yürüdüğünü ve **bunun sistem üzerinden bir sürece
dönüştürülmesi gerektiğini** açıkça belirtti. Aynı görüşmede GT Pusula ekibinin sorgu kontrolü için
kullandığı mevcut sürecin reuse edilebileceği söylendi.

## Kabul kriterleri

- [ ] Aksiyon sorumlusu SQL'ini sistem üzerinden gönderdiğinde kayıt listede "Gönderildi" durumuyla, gönderen kullanıcı ve gönderim tarihi ile görünür.
- [ ] Gönderilen SQL otomatik çalıştırılır; çalışma süresi 30 saniyeyi aşarsa gönderi reddedilir ve ret nedeni ("süre limiti aşıldı", ölçülen süre ile) kayda yazılır.
- [ ] Çıktı beklenen 30 kolonluk şemaya uymuyorsa gönderi reddedilir ve eksik/fazla kolonlar tek tek listelenir. (Kolonların dolu olması şart değildir, sadece şema uyumu kontrol edilir.)
- [ ] Kontrolör gönderiyi onayladığında durum "Geçişe hazır" olur; onay veya ret her seferinde kullanıcı + tarih ile işlem geçmişinde görünür.
- [ ] Bir SQL'in tüm sürümleri geçmişte saklanır; sorumlu, önceki sürümü ve o sürümün ret nedenini görebilir.

## Kapsam dışı

- SQL performans tuning'in kendisi — tuner manuel yapmaya devam eder, sistem yalnızca süre ölçer.
- Sinyal zenginleştirme join'lerinin otomatik üretilmesi. (Workshop kararı: join'ler aksiyon SQL'inin içinde elle hazırlanır.)
- Monitoring ve scoring SQL'leri — önce aksiyon tanımı akışı çıkar, diğerleri sonra değerlendirilir.

## Bağımlılıklar

| Neye bağlı | Durum |
|---|---|
| GT Pusula ekibinin mevcut sorgu kontrol süreci — reuse edilecek mi | bekliyor |
| Account Planning maintenance süreç sahipliği kararı | bekliyor |

## Açık sorular

- [ ] 30 saniye limiti kesin ret sebebi mi, yoksa uyarı verip kontrolöre mi bırakılmalı? — kime: Umut Özdemir / Garo Üçkardeş
- [ ] SQL tuner adımı bu akışın içinde bir onay basamağı mı olacak, yoksa dışarıda mı kalacak? — kime: GT Pusula ekibi
- [ ] Ortak klasöre manuel dosya bırakma yolu bu story ile kapatılacak mı, bir süre paralel mi yürüyecek? — kime: Alper
- [ ] Bu iş Account Planning kapsamında mı yoksa GT Pusula tarafında mı geliştirilecek? — kime: Alper

## Notlar

Story 3 günden uzun sürecek gibi duruyorsa bölünmeli. Muhtemel bölünme çizgisi:
(1) gönderim + otomatik doğrulama, (2) onay akışı + işlem geçmişi.

---

*Oluşturma: 2026-08-21 · Son güncelleme: 2026-08-21*
