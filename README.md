# Jeofizik Mühendisliği Bölümü — Ders Yükü Dağılımı Analizi

`Python` · `MIT License` · `CC BY 4.0` · `Open Science` · `Reproducible Research`

İstanbul Üniversitesi-Cerrahpaşa, Jeofizik Mühendisliği Bölümü'nün 2025-2026
eğitim-öğretim yılı ders yükü dağılımına ilişkin istatistiksel analiz.
Bu depo, [Ders Yükü Dengesi: Resmî Veriler Işığında Bir İnceleme](https://aliosmanoncel.blogspot.com/p/teaching-load-balance.html)
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
  olarak paylaşılmıştır. Bu depodaki script'ler bu veri seti üzerinde
  çalışacak şekilde hazırlanmıştır. Analizin yeniden üretilebilirliğini
  desteklemek amacıyla veri seti bu depoda da yer almaktadır.
- **`Dogrulama-Metodolojisi-ve-Sonuc.txt`** — Ders yükü verisinin, bölümün
  kendi resmi web sitesinde yayınlanan imzalı ders programlarıyla nasıl
  bağımsız olarak doğrulandığının özeti.
- **`requirements.txt`** — Script'lerin çalışması için gereken Python
  paketleri (`pip install -r requirements.txt`).
- **`CITATION.cff`** — Bu çalışmaya akademik atıf yapmak için gereken
  bilgiler (GitHub'ın "Cite this repository" özelliğini etkinleştirir).

Not: Bu depo yalnızca kaynak kod, veri ve doğrulama belgelerini içerir.
Konuyla ilgili blog yazıları burada değil, doğrudan
[aliosmanoncel.blogspot.com](https://aliosmanoncel.blogspot.com) üzerinde
yayınlanmaktadır.

## Bu depoda yer almayan belgeler

- **Kurum içi resmi yazışmalar** (Dekanlık yazıları, Bölüm Başkanlığı'nın
  üçüncü kişilere yazdığı resmi yanıtlar): Bunlar bu deponun yazarına
  hitaben düzenlenmemiş belgeler olduğu için dahil edilmemiştir.

## Yöntem özeti

Doğrulama, birbirinden bağımsız iki veri kaynağının karşılaştırılması
esasına dayanmaktadır. Ders yükü verisi, bölümün resmi web sitesinde
(jeofizikmuhendislik.iuc.edu.tr/tr/content/egitim/ders-programlari)
yayınlanan ve Bölüm Başkanı tarafından imzalanmış 4 resmi ders programı
belgesiyle (2025-2026 Güz/Bahar Lisans + Güz/Bahar Yüksek Lisans-Doktora)
satır bazında karşılaştırılarak bağımsız olarak doğrulanmıştır. Detaylar için
`Dogrulama-Metodolojisi-ve-Sonuc.txt` dosyasına bakınız.

## Veri gizliliği notu

Analiz, unvan grupları ve toplu istatistiksel göstergeler (ortalama,
minimum–maksimum, değişim katsayısı) üzerinden yürütülmüştür. Kişi
adları yalnızca kamuya açık resmî ders programlarında yer aldığı
ölçüde ve doğrulama amacıyla kullanılmıştır.

## Lisans

Hibrit lisanslama kullanılmıştır:
- **Kod** (`scripts/`) → [MIT License](LICENSE)
- **Veri, analiz metni, sonuçlar, PDF/Word çıktıları** → [CC BY 4.0 International](LICENSE-CONTENT.md)

## Güncellenebilirlik

Bu depo, analizin yeniden üretilebilirliğini (reproducibility) desteklemek
amacıyla hazırlanmıştır. Kod, veri ve metodoloji açık olarak paylaşılmıştır.
Analizde kullanılan kamuya açık veriler değiştiğinde veya yeni resmî
belgeler yayımlandığında, depo ve ilgili blog yazıları güncellenebilir.

Bu depo, blog yazısının yerine geçmez; blog yazısında yer alan
değerlendirmelerin teknik altyapısını, veri setini ve analiz kodlarını
belgelemek amacıyla hazırlanmıştır.

Öneriler, hata bildirimleri ve metodolojiye ilişkin katkılar
[GitHub Issues](https://github.com/aliosmanoncel/teaching-load-balance-analysis/issues)
bölümü üzerinden paylaşılabilir.

## Atıf (Citation)

Bu çalışmaya atıf yapmak için bkz. [`CITATION.cff`](CITATION.cff).

---
**Yazar:** Prof. Dr. Ali Osman Öncel — İstanbul Üniversitesi-Cerrahpaşa,
Jeofizik Mühendisliği Bölümü
**İlgili yazı (tam analiz):** https://aliosmanoncel.blogspot.com/p/teaching-load-balance.html
**İlgili yazı (özet):** https://aliosmanoncel.blogspot.com/2026/07/teaching-load-balance.html
**Orijinal inceleme (Ocak 2025):** https://aliosmanoncel.blogspot.com/2025/01/education.html
