---
tür: desen
bileşen: hero-ve-banner
etiketler: [desen, ana-sayfa, banner]
---

# Hero ve Banner Desenleri

> [!summary] Kural özeti
> Hero tek bir işi yapar: ürünü net göster, tek cümleyle neden önemli olduğunu söyle, tek birincil eyleme yönlendir. Hero en fazla **1 ekran** yüksekliğinde olur ve altında hemen kategori/hedef kitle girişleri gelir. Otomatik dönen karusel kullanılmaz.

## Gözlenen desenler (rakipler)

| Site | Hero kurgusu | Ders |
|---|---|---|
| Nike TR | Tam genişlik video/fotoğraf, ortada tek satır büyük harf başlık ("EVERY. DAY. SPEED."), 1 cümle alt metin, tek beyaz hap buton "İncele" | Tek mesaj, tek buton |
| Sneakersnstuff | Hero yok; 3 sütunlu editoryal fotoğraf ızgarası, her karoda sol üstte beyaz kutu içinde "MARKA →" ve altında "belirli çıkış adı" etiketi | Ürün/çıkış odaklı karolar doğrudan ürüne götürür |
| New Balance TR | Yaşam tarzı fotoğrafı karuseli (ok ve nokta), üstte kayan duyuru | Gerçek ayakta (on-feet) fotoğraf güven verir; karusel zayıf |
| END. | Bölünmüş hero (sol renkli panel + sağ kampanya fotoğrafı), üstte kayan değer önerisi şeridi | Bölünmüş düzen metni fotoğraftan ayırır, okunurluğu korur |
| Kith | Karanlık tam ekran video, sol altta serif başlık "15 Years Together.", 2 çerçeveli buton | Marka hikâyesi; ama girişte modal pencere engel |

Ayrıntılar: [[Nike Türkiye]], [[Sneakersnstuff]], [[New Balance Türkiye]], [[END. Clothing]], [[Kith]], [[Aimé Leon Dore]], [[Represent]].

## KPT için spesifikasyon

**Masaüstü (≥1024 px)**
- Yükseklik: `min(88vh, 760px)`; altındaki bölüm ilk ekranda en az 80 px görünmeli (devam ipucu).
- Düzen: 12 sütunlu ızgarada görsel 7 sütun, metin 5 sütun **veya** tam genişlik fotoğraf + sol altta metin bloğu (fotoğrafın sol alt %40'ı sakin olmalı).
- Görsel: **gerçek** ürün/ayakta fotoğrafı; WebP/AVIF, en geniş 2400 px, ≤250 KB; `<img fetchpriority="high">` (CSS arka plan değil); `width/height` öznitelikleri ile CLS sıfır.
- Metin: eyebrow (12–13 px, büyük harf, 0,08em aralık, örn. "NEW BALANCE") · başlık 56–72 px, 700–800 ağırlık, en fazla 2 satır (örn. "9060. Karakteri tabanında.") · alt metin en fazla 1 cümle, 16–18 px · fiyat (opsiyonel) · **1 birincil buton** (bordo `--accent`, 48–52 px yükseklik, "Ürünü incele") + en fazla 1 ikincil metin linki ("Tüm New Balance →").
- Hareket: yok veya tek bir yavaş fade-in (≤300 ms); `prefers-reduced-motion` desteklenir.

**Mobil (<768 px)**
- Görsel üstte 4:5 oran, metin altta; başlık 32–40 px; buton tam genişlik 52 px.
- Hero toplam yüksekliği ≤ 1 ekran (844 px cihazda ≤ 760 px).

**3 model vitrini (mevcut showcase'in yerine)**
- Ekrana sabitlenen (pinned) kaydırma yerine: hero altında 3 sütunlu (mobilde yatay kaydırmalı) "Öne çıkan modeller" kartları; her kart: 4:5 fotoğraf, marka, model, fiyat, "İncele".
- 360° görünüm istenirse yalnızca PDP'de ve kullanıcı başlatınca: 24–36 kare, çapraz geçiş yok, sürükle-döndür.

## Banner türleri ve şablonları

| Tür | Konum | Anatomi | Örnek metin (KPT sesiyle) |
|---|---|---|---|
| Duyuru şeridi | Header üstü, 36–40 px | Tek satır, ortalı, 13 px; en fazla 3 dönüşümlü mesaj, durdurulabilir | "1.500 TL üzeri ücretsiz kargo · 30 gün ücretsiz iade · %100 orijinal" (gerçek politikalarla) |
| Kategori karoları | Hero altı | 3–4 karo, 4:5 fotoğraf, sol altta etiket "Erkek →" | "Erkek" · "Kadın" · "Çocuk" · "Yeni gelenler" |
| Marka/çıkış karosu | Ana sayfa ortası | SNS tarzı: fotoğraf + beyaz kutu etiket "MARKA →" + model adı | "ADIDAS → / Samba OG" |
| Kampanya bandı | Ana sayfa ortası | Bölünmüş: renkli panel (metin) + fotoğraf | "Sezon sonu: seçili modellerde %30'a varan indirim" (indirim yönetmeliğine uygun, bkz. [[Türkiye E-ticaret Pazarı]]) |
| Hizmet şeridi | Footer üstü | 3–4 ikon + kısa metin | "Doğru numarayı bul" · "30 gün iade" · "Taksit" · "Mağazadan değişim" |

## Kaçınılacaklar

- Otomatik dönen karusel ve otomatik ilerleyen hero (kullanıcılar çoğunlukla görmezden gelir, erişilebilirlik riski; bkz. [[E-ticaret UX Verileri]]).
- Ürün görselinde çapraz geçişli sprite (mevcut KPT hatası, bkz. [[KPT Store Denetimi]]).
- Markalı ürünlerin AI ile yeniden çizilmiş görselleri (güven ve marka kullanım hakları riski).
- Metni fotoğrafın karmaşık bölgesine bindirmek; gerekirse %40–60 koyu degrade.
- Girişte modal/pop-up (Kith örneği).

İlgili: [[Görsel Tasarım ve Trendler 2026]] · [[Satın Alma Psikolojisi]] · [[Dönüşüm Vaka Çalışmaları]]
