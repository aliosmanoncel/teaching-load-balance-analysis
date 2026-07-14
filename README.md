# Jeofizik Mühendisliği Bölümü — Ders Yükü Dağılımı Analizi

`Python` · `MIT License` · `CC BY 4.0` · `Open Science` · `Reproducible Research`

**Sürüm:** v1.0
**Son güncelleme:** 14 Temmuz 2026
**Durum:** İlk kamuya açık sürüm

İstanbul Üniversitesi-Cerrahpaşa, Jeofizik Mühendisliği Bölümü'nün 2025-2026
eğitim-öğretim yılı ders yükü dağılımına ilişkin istatistiksel analiz.
Bu depo, [Ders Yükü Dengesi: Resmî Veriler Işığında Bir İnceleme](https://aliosmanoncel.blogspot.com/p/teaching-load-balance.html)
başlıklı yazının metodoloji ve kaynak kod kısmıdır ([kısa özet/teaser yazı](https://aliosmanoncel.blogspot.com/2026/07/teaching-load-balance.html) da mevcuttur).
Bu çalışma, Ocak 2025'te yayımlanan [Ders Yükü Dağılımındaki Eşitsizlikler](https://aliosmanoncel.blogspot.com/2025/01/education.html)
başlıklı ilk incelemenin güncellenmiş ve genişletilmiş sürümüne dayanmaktadır.

## Depo Yapısı

| Dizin / Dosya | Açıklama |
|---|---|
| `scripts/` | Python analiz script'leri (5 dosya, openpyxl tabanlı) |
| `data/` | Analizde kullanılan veri seti (`Jeofizik_Ders_Yuku_Dagilimi.xlsx`) |
| `sonuclar/` | Script'lerin 14.07.2026 tarihli çalıştırılmasından elde edilen statik çıktılar |
| `Dogrulama-Metodolojisi-ve-Sonuc.txt` | Doğrulama süreci ve sonucu |
| `requirements.txt` | Python bağımlılıkları |
| `CITATION.cff` | Akademik atıf bilgileri |
| `LICENSE` / `LICENSE-CONTENT.md` | Hibrit lisans (kod / veri-metin) |

Veri seti (`data/Jeofizik_Ders_Yuku_Dagilimi.xlsx`), 13.07.2026 tarihinde
Doç. Dr. Savaş Karabulut tarafından bölüm e-posta listesi ve X (Twitter)
üzerinden kamuya açık olarak paylaşılmıştır. Bu depodaki script'ler bu
veri seti üzerinde çalışacak şekilde hazırlanmıştır; analizin yeniden
üretilebilirliğini desteklemek amacıyla veri seti bu depoda da yer
almaktadır.

Not: Bu depo yalnızca kaynak kod, veri ve doğrulama belgelerini içerir.
Konuyla ilgili blog yazıları burada değil, doğrudan
[aliosmanoncel.blogspot.com](https://aliosmanoncel.blogspot.com) üzerinde
yayınlanmaktadır.

## Hızlı Başlangıç

Gereksinim: **Python ≥ 3.11**

```bash
git clone https://github.com/aliosmanoncel/teaching-load-balance-analysis.git
cd teaching-load-balance-analysis
pip install -r requirements.txt
cd scripts
python zorunlu_dersi_olmayanlar.py
```

⚠️ Script'ler `../data/Jeofizik_Ders_Yuku_Dagilimi.xlsx` göreli yolunu
kullanır; bu nedenle **`scripts/` dizini içinden** çalıştırılmalıdır,
depo kök dizininden değil. Diğer script'ler de aynı şekilde çalışır ve
konsola sonuç yazdırır (bkz. `sonuclar/` içindeki örnek çıktılar).

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

## Sınırlılıklar

Bu analiz yalnızca kamuya açık ders programlarına dayanmaktadır. Ders
görevlendirmelerinin idari gerekçeleri, uzmanlık alanları veya kurum
içi karar süreçleri bu deponun kapsamı dışındadır.

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

> **Açık Bilim İlkesi**
> Bu çalışma, şeffaflık, doğrulanabilirlik ve yeniden üretilebilirlik
> ilkeleri doğrultusunda hazırlanmıştır. Kodlar, veri ve metodoloji
> mümkün olan en geniş ölçüde açık olarak paylaşılmıştır.

> **Sorumluluk Reddi**
> Bu depoda yer alan analiz ve değerlendirmeler yazara aittir. Kurumsal
> bir görüş veya resmî açıklama niteliği taşımaz.

## Atıf (Citation)

Bu çalışmaya atıf yapmak için bkz. [`CITATION.cff`](CITATION.cff).

---
**Yazar:** Prof. Dr. Ali Osman Öncel — İstanbul Üniversitesi-Cerrahpaşa,
Jeofizik Mühendisliği Bölümü
**İlgili yazı (tam analiz):** https://aliosmanoncel.blogspot.com/p/teaching-load-balance.html
**İlgili yazı (özet):** https://aliosmanoncel.blogspot.com/2026/07/teaching-load-balance.html
**Orijinal inceleme (Ocak 2025):** https://aliosmanoncel.blogspot.com/2025/01/education.html
