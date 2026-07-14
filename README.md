# Jeofizik Mühendisliği Bölümü — Ders Yükü Dağılımı Analizi

İstanbul Üniversitesi-Cerrahpaşa, Jeofizik Mühendisliği Bölümü'nün 2025-2026
eğitim-öğretim yılı ders yükü dağılımının eşitlik/dengelilik açısından
istatistiksel analizi. Bu depo, [Ders Yükü Dağılımındaki Eşitsizlikler](https://aliosmanoncel.blogspot.com)
başlıklı yazının metodoloji ve kaynak kod kısmıdır.

## Bu depoda ne var

- **`scripts/`** — Analiz için yazılan 5 Python script'i (openpyxl tabanlı).
  Her script kendi dosya başında veri kaynağı, doğrulama durumu ve
  yöntemsel kısıtları belgeler.
- **`sonuclar/`** — Script'lerin 14.07.2026 tarihli çalıştırılmasından
  elde edilen sabit (statik) çıktılar.
- **`data/Jeofizik_Ders_Yuku_Dagilimi.xlsx`** — Analizde kullanılan veri
  seti. Orijinal olarak Doç. Dr. Savaş Karabulut tarafından derlenmiş ve
  13.07.2026'da bölüm e-posta listesine + X (Twitter) üzerinden kamuya
  gönderilmiştir (*modified after Karabulut* — bu depodaki script'ler bu
  veri seti üzerinde çalışacak şekilde yazılmıştır). Zaten kamuya açık
  paylaşılmış olduğu için, script'lerin çalıştırılabilir/tekrarlanabilir
  olması adına burada da bulundurulmaktadır.
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
  değil başka taraflara adreslenmiş belgeler olduğu için dahil edilmemiştir.

## Yöntem özeti

Ders yükü verisi, bölümün resmi web sitesinde
(jeofizikmuhendislik.iuc.edu.tr/tr/content/egitim/ders-programlari)
yayınlanan ve Bölüm Başkanı tarafından imzalanmış 4 resmi ders programı
belgesiyle (2025-2026 Güz/Bahar Lisans + Güz/Bahar Yüksek Lisans-Doktora)
tek tek karşılaştırılarak bağımsız olarak doğrulanmıştır. Detaylar için
`Dogrulama-Metodolojisi-ve-Sonuc.txt` dosyasına bakınız.

## Veri gizliliği notu

Analiz, unvan grubu ve toplu istatistikler (ortalama, min-maks, değişim
katsayısı) üzerinden yürütülmüştür. Bireysel isimler yalnızca kamuya açık
resmi ders programı belgelerinde zaten yer aldığı ölçüde ve doğrulama
amacıyla kullanılmıştır.

---
**Yazar:** Prof. Dr. Ali Osman Öncel — İstanbul Üniversitesi-Cerrahpaşa,
Jeofizik Mühendisliği Bölümü
**İlgili yazı:** https://aliosmanoncel.blogspot.com
