# PO Rehberi — Koçluk Notları

Alper ilk kez PO. Bu dosya, ona yol gösterirken kullanılacak temel bilgi ve sık yapılan hatalar.

## PO'nun asıl işi nedir?

Üç cümlede: **Ne yapılacağına karar vermek, nedenini herkese anlatmak, ekibin doğru şeyi yapabilmesi için soruları cevaplamak.**

PO'nun işi *olmayan* şeyler: işleri kime atandığını yönetmek (bu ekibin işi), nasıl yapılacağına karar vermek (bu ekibin işi), toplantıları yürütmek (bu Scrum Master'ın işi).

**İlk kez PO olanların en sık hatası:** proje yöneticisi gibi davranıp işleri takip etmeye çalışmak. Sizin işiniz takip değil, *yön*.

## Sprint hedefi

Sprint hedefi tek cümledir ve sprint sonunda "başardık mı?" sorusuna evet/hayır cevabı verir.

- İyi: "Kullanıcılar aksiyonları toplu olarak atayabilecek."
- Kötü: "S-014, S-015, S-016 tamamlanacak." (Bu bir liste, hedef değil.)

**Neden gerekli:** Sprint ortasında yeni bir istek geldiğinde tek savunma mekanizmanız budur. "Bu hedefe hizmet ediyor mu?" Etmiyorsa backlog'a gider.

## Definition of Ready — story ne zaman hazır?

- [ ] Başlık işlevi anlatıyor
- [ ] Kim / ne / neden net
- [ ] En az 2 test edilebilir kabul kriteri
- [ ] Açık soru yok (veya kalanlar bloke etmiyor)
- [ ] Ekip okumuş, "anladık" demiş
- [ ] Bağımlılıklar belirtilmiş
- [ ] 3 günden uzun sürmeyecek büyüklükte

Eksik maddeyle sprinte alınan story sprint ortasında durur ve o sprintin yarısını yer.

## Kabul kriteri yazımı

Kural: **bir başkası okuyup "oldu / olmadı" diyebilmeli.**

| Kötü | İyi |
|---|---|
| Hızlı olmalı | 50 kayıt için 2 saniyeden kısa sürede tamamlanır |
| Kullanıcı dostu olsun | Toplu atama en fazla 3 tıklamayla yapılır |
| Hata vermemeli | Yetkisiz kullanıcı denediğinde "yetkiniz yok" mesajı görür ve işlem yapılmaz |
| Raporlanabilir olmalı | Yapılan toplu atamalar işlem geçmişinde kullanıcı ve tarih bilgisiyle listelenir |

**Faydalı format (Given-When-Then):**
"`[durum]` iken, kullanıcı `[eylem]` yaptığında, `[sonuç]` olur."

## Backlog önceliklendirme

Bu projede sıralama kriterleri `po/01-backlog/oncelik.md` içinde yazılı. Genel yaklaşım:

1. **Zorunluluk** — yasal, uyum, kurumsal dayatma
2. **Bağımlılık** — başka işleri açan işler önce
3. **Değer/efor oranı** — az emekle çok fayda önce
4. **Risk** — belirsiz teknik konular erken denenmeli (geç öğrenilen kötü haber pahalıdır)

**Kritik alışkanlık:** Sıralamanın gerekçesini bir satırla yazın. Yazmazsanız her toplantıda yeniden tartışılır.

## Törenler ve PO'nun hazırlığı

| Tören | PO ne getirir | PO ne yapmaz |
|---|---|---|
| **Daily** | Cevap bekleyen soruları cevaplar | Kimin ne yaptığını sorgulamaz |
| **Refinement** | Konuşulacak story listesi, kabul kriteri taslakları | Tahmin vermez (ekip verir) |
| **Planlama** | Sprint hedefi, sıralı backlog | Kapasiteyi belirlemez (ekip belirler) |
| **Review** | Demo listesi, davetli listesi, geri bildirim soruları | Sunumu tek başına yapmaz |
| **Retro** | Katılır, dinler | Yürütmez (Scrum Master yürütür) |

## Sık yapılan 8 hata

1. **Sprint hedefi yazmamak** → her istek sprinte girer, sprint anlamsızlaşır.
2. **Kabul kriteri olmadan story vermek** → ekip tahmin eder, yanlış şey çıkar, yeniden yapılır.
3. **Sprint ortasında iş sokmak** → "küçük bir şey" diye başlar, sprint hedefi kaçar.
4. **Sorulara geç cevap vermek** → ekip bloke kalır. PO'nun soruya aynı gün cevap vermesi kuraldır.
5. **Kararın gerekçesini yazmamak** → 2 ay sonra aynı tartışma baştan yapılır.
6. **Kötü haberi geciktirmek** → paydaş güveni, gecikmenin kendisinden çok geç haber verilmesinden zarar görür.
7. **Review'a hazırlıksız girmek** → ekip iyi iş çıkarmıştır ama görünmez kalır.
8. **Her isteğe "evet" demek** → PO'nun asıl gücü neye "hayır" dediğidir. "Hayır" değil "şimdi değil" deyin ve ertelenenler listesine yazın.

## Terim sözlüğü

| Terim | Anlamı |
|---|---|
| **Backlog** | Yapılacak işlerin öncelik sırasına dizilmiş listesi |
| **Refinement** | Backlog'daki işlerin ekiple konuşulup netleştirildiği toplantı |
| **Definition of Ready** | Bir işin sprinte alınabilmesi için taşıması gereken şartlar |
| **Definition of Done** | Bir işin "bitti" sayılabilmesi için taşıması gereken şartlar |
| **Blocker** | İşin ilerlemesini tamamen durduran engel |
| **Velocity** | Ekibin bir sprintte ortalama ne kadar iş bitirdiği |
| **Scope creep** | Kapsamın fark edilmeden büyümesi |
| **Spike** | Bir belirsizliği araştırmak için ayrılan zaman kutusu |
| **Epic** | Birden fazla sprinte yayılan büyük iş parçası |
| **Retro** | Ekibin çalışma şeklini iyileştirmek için yaptığı toplantı |

## Alper'e özel notlar

- Jira'yı asistan göremiyor. Alper'in sabah brifinginde verdiği bilgiler asistanın tek veri kaynağı — bu yüzden brifingi cevaplamak "asistanı beslemek" demek. Ara sıra bunu hatırlat.
- Alper çok yoğun. Bir işi ondan istemek yerine mümkün olduğunca taslağını hazırlayıp onaya sun.
- Repo'yu ekip görüyor. Yazılan her şey ekibe açık — bunu unutmadan yaz.
