# Jeofizik Mühendisliği Bölümü — Ders Yükü Dağılımı Analizi

İstanbul Üniversitesi-Cerrahpaşa, Jeofizik Mühendisliği Bölümü'nün 2025-2026
eğitim-öğretim yılı ders yükü dağılımının eşitlik/dengelilik açısından
istatistiksel analizi. Bu depo, [Ders Yükü Dengesi: Resmî Veriler Işığında Bir İnceleme](https://aliosmanoncel.blogspot.com/p/teaching-load-balance.html)
başlıklı yazının metodoloji ve kaynak kod kısmıdır ([kısa özet/teaser yazı](https://aliosmanoncel.blogspot.com/2026/07/teaching-load-balance.html) da mevcuttur).
Bu çalışma, Ocak 2025'te yayımlanan [Ders Yükü Dağılımındaki Eşitsizlikler](https://aliosmanoncel.blogspot.com/2025/01/education.html)
başlıklı ilk incelemenin güncellenmiş ve genişletilmiş sürümüne dayanmaktadır.

## Bu depoda ne var

- **`scripts/`** — Analiz için yazılan 5 Python script'i (openpyxl tabanlı).
  Her script kendi dosya başında veri kaynağı, doğrulama durumu ve
  yöntemsel kısıtları belgeler.
- **`sonuclar/`** — Script'lerin 14.07.2026 tarihli çalıştırılmasından
  elde edilen sabit (statik) çıktılar.
- **`data/Jeofizik_Ders_Yuku_Dagilimi.xlsx`** — Analizde kullanılan veri
  seti. Bu veri seti, 13.07.2026 tarihinde Doç. Dr. Savaş Karabulut
  tarafından bölüm e-posta listesi ve X (Twitter) üzerinden kamuya açık
  olarak paylaşılmıştır. Bu depodaki script'ler, kamuya açık olarak
  paylaşılan bu veri seti üzerinde çalışacak şekilde hazırlanmıştır.
  Veri seti kamuya açık olarak paylaşılmış olduğundan, analizin yeniden
  üretilebilirliğini sağlamak amacıyla bu depoda da yer almaktadır.
- **`Dogrulama-Metodolojisi-ve-Sonuc.txt`** — Ders yükü verisinin, bölümün
  kendi resmi web sitesinde yayınlanan imzalı ders programlarıyla nasıl
  bağımsız olarak doğrulandığının özeti.

Not: Bu depo yalnızca kaynak kod, veri ve doğrulama belgelerini içerir.
Konuyla ilgili blog yazıları burada değil, doğrudan
[aliosmanoncel.blogspot.com](https://aliosmanoncel.blogspot.com) üzerinde
yayınlanmaktadır.

## Bu depoda BİLEREK bulunmayanlar

- **Kurum içi resmi yazışmalar** (Dekanlık yazıları, Bölüm Başkanlığı'nın
  üçüncü kişilere yazdığı resmi yanıtlar): Bunlar bu deponun yazarına
  hitaben düzenlenmemiş belgeler olduğu için dahil edilmemiştir.

## Yöntem özeti

Ders yükü verisi, bölümün resmi web sitesinde
(jeofizikmuhendislik.iuc.edu.tr/tr/content/egitim/ders-programlari)
yayınlanan ve Bölüm Başkanı tarafından imzalanmış 4 resmi ders programı
belgesiyle (2025-2026 Güz/Bahar Lisans + Güz/Bahar Yüksek Lisans-Doktora)
satır bazında karşılaştırılarak bağımsız olarak doğrulanmıştır. Detaylar için
`Dogrulama-Metodolojisi-ve-Sonuc.txt` dosyasına bakınız.

## Veri gizliliği notu

Analiz, unvan grubu ve toplu istatistikler (ortalama, min-maks, değişim
katsayısı) üzerinden yürütülmüştür. Kişi adları yalnızca kamuya açık
resmi ders programı belgelerinde zaten yer aldığı ölçüde ve doğrulama
amacıyla kullanılmıştır.

## Lisans

Hibrit lisanslama kullanılmıştır:
- **Kod** (`scripts/`) → [MIT](LICENSE)
- **Veri, analiz metni, sonuçlar, PDF/Word çıktıları** → [CC BY 4.0](LICENSE-CONTENT.md)

## Güncellenebilirlik

Bu depo, analizin yeniden üretilebilirliğini (reproducibility) desteklemek
amacıyla hazırlanmıştır. Kod, veri ve metodoloji açık olarak paylaşılmıştır.
Analizde kullanılan kamuya açık veriler değiştiğinde veya yeni resmî
belgeler yayımlandığında, depo ve ilgili blog yazıları güncellenebilir.

---
**Yazar:** Prof. Dr. Ali Osman Öncel — İstanbul Üniversitesi-Cerrahpaşa,
Jeofizik Mühendisliği Bölümü
**İlgili yazı (tam analiz):** https://aliosmanoncel.blogspot.com/p/teaching-load-balance.html
**İlgili yazı (özet):** https://aliosmanoncel.blogspot.com/2026/07/teaching-load-balance.html
**Orijinal inceleme (Ocak 2025):** https://aliosmanoncel.blogspot.com/2025/01/education.html
