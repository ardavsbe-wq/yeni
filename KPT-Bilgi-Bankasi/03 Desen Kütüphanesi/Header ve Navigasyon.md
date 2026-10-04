---
tür: desen
bileşen: header-navigasyon
etiketler: [desen, navigasyon]
---

# Header ve Navigasyon

> [!summary] Kural özeti
> Birinci seviye menü **hedef kitle + keşif** üzerine kurulur (Jakob yasası: Türk alıcı Nike, Trendyol, FLO düzenine alışkın). Kategori ve marka ikinci seviyede, mega menü içinde.

## Gözlenen desenler

- **Nike TR:** üst yardımcı bar ("Mağaza Bul | Yardım | Bize Katıl | Oturum Aç") · ana menü: `Yeni` `Erkek` `Kadın` `Çocuk` `Spor` · sağda arama kutusu, favori, sepet. Altında tek satır bilgi şeridi.
- **New Balance TR:** üst siyah şerit (dil, para birimi TRY, "İade", "Yardım") · menü: `Yeniler` `Erkek` `Kadın` `Çocuk` `İndirim` (kırmızı) `Blog` · arama kutusu · "Giriş | Üyelik" · sepet rozeti.
- **END.:** kayan duyuru şeridi · `MEN / WOMEN` geçişi · ikinci satır: `New In` `Brands` `Footwear` `Clothing` `Accessories` `Lifestyle` `Active` `Launches` `Sale` (kırmızı).
- **Sneakersnstuff:** tek satır büyük harf: `NEW ARRIVALS` `UPCOMING RELEASES` `SNEAKERS` `CLOTHING` `ACCESSORIES` `BRANDS` `EDITORIALS` `SNS STORES` `SALE`.

## KPT için spesifikasyon

**Masaüstü header (64–72 px, sticky; aşağı kaydırınca gizlenir, yukarı kaydırınca görünür)**
1. Duyuru şeridi (36 px, `--ink` zemin, `--paper` metin): değer önerisi (bkz. [[Hero ve Banner Desenleri]]).
2. Satır: logo (sol) · menü (orta): `Yeni gelenler` · `Erkek` · `Kadın` · `Çocuk` · `Markalar` · `İndirim` (varsa, tek kırmızı/bordo öğe) · sağda arama kutusu (en az 280 px genişlik, placeholder "Model, marka veya numara ara") · favori · hesap · sepet (adet rozeti).
3. **Mega menü** (Erkek/Kadın/Çocuk için aynı şablon): sütun 1 "Ayakkabı" (Sneaker, Koşu, Basketbol, Yürüyüş, Outdoor, Terlik & Sandalet) · sütun 2 "Giyim" (Mont, ...) · sütun 3 "Markalar" (logo listesi) · sütun 4 "Numaranla alışveriş" (beden ızgarası kısayolu) · sağda 1 görsel karo (öne çıkan model). Hover gecikmesi 150–250 ms; tıkla-aç da çalışır; Esc kapatır.

**Mobil header (56 px)**
- Logo · arama ikonu · favori · sepet · hamburger.
- Hamburger çekmece: tam yükseklik, sol kayan; üstte arama; ardından `Yeni gelenler`, `Erkek ›`, `Kadın ›`, `Çocuk ›`, `Markalar ›`, `İndirim`; altında `Numaranla başla` kısayolu, `Favorilerim`, `Hesabım`, `Yardım`. Alt menüler kayarak açılır (geri oku ile).
- **Tek bir açma/kapama mantığı** (mevcut sitede iki script çakışıyor, bkz. [[KPT Store Denetimi]]): `aria-expanded`, odak tuzağı, Esc ile kapanma, arka plan kaydırma kilidi.

## Erişilebilirlik

- "İçeriğe atla" linki; menü `nav[aria-label="Ana menü"]`; mega menü butonları `aria-expanded` + `aria-controls`.
- Dokunma hedefleri ≥44×44 px (mevcut sitede doğru).

İlgili: [[Mobil Deneyim]] · [[Arama]] · [[E-ticaret UX Verileri]]
