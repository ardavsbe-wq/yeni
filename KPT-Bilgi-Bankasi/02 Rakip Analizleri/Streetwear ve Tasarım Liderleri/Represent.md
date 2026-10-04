---
tür: rakip-analizi
site: Represent
url: https://representclo.com/
ülke: UK (incelenen: ABD mağazası, otomatik yönlendirme)
segment: premium streetwear marka DTC
erişim: tam
incelenme: 2026-10-04
incelenen-sayfalar: [https://representclo.com/, https://representclo.com/pages/represent-home, https://representclo.com/collections/footwear-all, https://representclo.com/products/rep-cap-distressed-leather-dark-brown]
etiketler: [rakip, streetwear, tasarim-lideri]
---

# Represent

> [!summary] Özet
> Kendini "Luxury British Streetwear" olarak tanımlayan marka; iki alt marka (Represent ana koleksiyon ve 247 Activewear) ve ayakkabı serisi satıyor. En güçlü 3 yanı: (1) ana sayfada **iki markayı yan yana koyan 50/50 bölünmüş tam ekran kapı**, (2) marka sayfasında **"tam ekran banner → 8 ürünlük yatay şerit → altı çizili SHOP linki"** ritminin 8 kez tekrarı, (3) tek font (STK Bureau) ve **siyah / beyaz / #F7F7F7** üçlüsüyle kurulan sade ama ticari olarak güçlü arayüz. KPT için en değerli ders: editoryal banner'ı **hemen altında alışverişe dönüştüren şerit**, hikâye ile ticareti aynı ekranda birleştiriyor.

## Kimlik ve konumlandırma
- Başlık etiketi: "Luxury British Streetwear | Official US Store® | REPRESENT".
- Header'ın solunda alt markalar düğme olarak: "Represent", "247", "Outlet"; sağda "Retail", "The Vault", "Prestige" (sadakat programı).
- Ürün açıklamaları koleksiyon hikâyesiyle yazılmış: "Part of the JAWBREAKER FW26 Mainline collection, it carries the tension between utility and rebellion that defines the season."

## Görsel dil

### Renk paleti
| Rol | Hex | Kullanım yeri |
|---|---|---|
| Ana metin / ana CTA | #000000 | Tüm başlıklar, "ADD TO CART" zemini |
| Koyu CTA (sepet) | #0D0E0E (`--primary-dark`) | "SECURE CHECKOUT" butonu |
| Zemin | #FFFFFF | Sayfa |
| Ürün kartı / beden kutusu zemini | #F7F7F7 | Kart görsel alanı (CSS `bg-[#f7f7f7]`), beden butonları |
| İkincil metin | #737373 | Renk adı ("Dark Brown"), "4 Colors" |
| Footer yasal | #575757 @0.8 | Alt linkler |
| Hero CTA zemini | #000000 @0.3 + `backdrop-filter: blur(24px)` | Banner butonları |
| Hero CTA çerçeve | 1px #FFFFFF @0.3 | Banner butonları |
| Ücretsiz kargo çubuğu | #468847 (ekran görüntüsünden) | Sepet çekmecesi ilerleme çizgisi |
| Satış kırmızısı | #D70909 | Tek bir rozet (ana sayfa) |

**Az renkle premium:** Arayüzde renk yalnızca 15px yuvarlak renk swatch'larında (#4B3621, #D2B48C, #808080…) ve fotoğraflarda var. Fotoğraflar desatüre, gri-yeşil perde veya beton duvar önünde; bu sayede siyah/beyaz arayüzle uyumlu.

### Tipografi
- **Aile:** STKBureau (tüm metin; 117–163 öğenin tamamı).
- **Ölçek:** 10px (yasal, rozet), 11px (PDP açıklama, ağırlık 300, satır 17.6px), **12px (gövde, kart, buton: baskın boyut)**, 14px (bölüm altı "SHOP …" linki, uppercase), 16px (hero üst satır, ağırlık 300; PLP H1 "Footwear" 500), 24px (mobil hero başlık), **32px (banner başlığı, ağırlık 500, satır 32px, harf aralığı -1.6px = -0.05em)**.
- **Ağırlıklar:** 300 (açıklama, hero üst satırı), 400 (gövde), 500 (ürün adı, başlık), 700 ("STYLE WITH", "YOU MAY ALSO LIKE" uppercase).
- **Harf aralığı:** gövde 0.133px (~0.011em), footer 0.36px; büyük başlıkta negatif -1.6px (sıkı, modern grotesk).
- **Büyük harf:** CTA'lar ("DISCOVER", "SHOP NOW", "ADD TO CART"), bölüm başlıkları; ürün adları normal yazım.

### Hareket ve hover
- **Banner CTA metin kaydırma:** Her butonun içinde metin iki kez var; ikinci kopya `translateY(40px)` ile gizli. Hover'da ikisi `transform 0.5s` ile yukarı kayar (yeni metin aşağıdan gelir). Buton yüksekliği 40px, `overflow: hidden`.
- Kart: `opacity 0.3s ease` ile ikinci görsele geçiş (kartta 2 görsel), `all 0.2s cubic-bezier(0,0,0.2,1)` swatch'lar.
- Kaydırınca header'daki "REPRESENT" wordmark'ı **"R" monogramına** küçülür; marka sayfasında aşağı kaydırırken header gizlenir.
- Ana sayfada hero metni yapışkan (görsel kayarken başlık ve butonlar sabit kalıyor).

## Header ve navigasyon
- Yükseklik 46px, şeffaf (hero üzerinde beyaz metin, iç sayfalarda siyah). Duyuru şeridi yok.
- Sol: "Represent", "247" (yanında küçük şimşek ikonu), "Outlet" (12px düğmeler, 12px iç boşluk). Orta: wordmark. Sağ: "Retail", "The Vault", "Prestige", "US / USD", bildirim, kaydedilenler, arama, hesap, çanta ikonları.
- Mobil: hamburger, arama, bildirim | logo | kaydet, hesap, çanta.
- Mega menü: incelenemedi (otomasyonda "Represent" düğmesi tıklanamadı).

## Ana sayfa ve banner/hero örnekleri

![[represent-home-desktop.jpg]]
*Ana sayfa: iki alt markayı 50/50 bölen tam ekran kapı.*

**Hero A – Ana sayfa bölünmüş kapı (`/`)**
- Düzen: iki panel, her biri 720x900px (**4:5**), tam ekran yükseklik; mobilde alt alta 390x422px (~0.92).
- Sol görsel: gri perde önünde ayakta model, "OWNERS CLUB" sweatshirt, kargo pantolon (stüdyo, soğuk gri ton). Sağ görsel: beton duvar ve endüstriyel boru önünde koşu kıyafetli model (247).
- Metin bloğu her panelde sol hizalı, x=87px, dikeyde ortanın biraz altında (y≈386–513px):
  - Üst satır: **"British Luxury Menswear"** / **"On A Mission"** (16px, ağırlık 300, #FFFFFF)
  - Başlık: **"Represent"** / **"247 Activewear"** (32px, 500, 32px satır)
  - İki CTA yan yana, 17px aralık: **"DISCOVER"** + **"OWNERS FALL WINTER '26"** ve **"EXPLORE"** + **"247 X CADENCE"**. Stil: 40px yükseklik, 0 24px iç boşluk, 12px uppercase, #000000 @0.3 zemin + 24px arka plan bulanıklığı, 1px #FFFFFF @0.3 çerçeve, 2px radius ("buzlu cam").
- Sayfada hero'dan sonra yalnızca footer var (sayfa 1263px).

![[represent-banner-hero.jpg]]
*Marka sayfası (/pages/represent-home) açılış banner'ı: ortalanmış küçük metin bloğu görselin alt kısmında.*

**Hero B – Marka sayfası açılış banner'ı**
- Tam genişlik **1440x900 (16:10)**, gri perde önünde kadın + erkek model, ayakta tam boy.
- Metin bloğu **ortalanmış, alt üçte birde** (y=705–822px): üst satır **"Now Live"** (12px), başlık **"Owners Fall Winter"** (32px/500/-1.6px), tek CTA **"SHOP MENS & WOMENS"** (buzlu cam buton, 187x40px).
- Görsel kişiler merkezde, metin modellerin bacak hizasında; metin küçük olduğu için yüzleri kapatmıyor.

**Banner ritmi (marka sayfası, yukarıdan aşağı, sayfa 18.157px):**
1. Banner 900px "Now Live / Owners Fall Winter" → CTA "SHOP MENS & WOMENS"
2. Ürün şeridi 522px (8 ürün, yatay kaydırma, kart ~271px genişlik, 3:4 görsel) → altı çizili ok'lu link **"→ SHOP OWNERS FALL WINTER '26"** (14px uppercase)
3. Banner 900px **"Introducing Fall Winter '26 : Jawbreaker"** → iki CTA "SHOP NOW" + "DISCOVER STORY"
4. Şerit (The Work Jacket, Riot Puffer…) → "SHOP FALL WINTER '26"
5. Banner **"Introducing : Graphics Collection"** → "SHOP NOW" + "DISCOVER" → şerit → "SHOP GRAPHICS"
6. Banner **"Discover : The New Arrivals"** → "SHOP NOW" → şerit
7. 2x2 kategori ızgarası (her hücre 720px genişlik, alt solda 16px/500 uppercase etiket: "T-SHIRTS", "HOODIES", "SHORTS", "FOOTWEAR"); FOOTWEAR görseli: duvar önünde elde tutulan bir çift sneaker
8. Uzun banner 1773px **"Discover : Summer '26"** → şerit
9. Banner 690px **"Discover : Champions Collection"** → şerit
10. İki panel yan yana: "Spring Summer '26 / Owners Club / EXPLORE" ve "Elevated Basics / Initial / DISCOVER"
11. Banner **"Discover : Heaton Collection"** → "SHOP NOW" + "THE STORY" → şerit
12. "EXPLORE COLLECTIONS": New Arrivals, Bestsellers, Summer '26, Prestige 2.0

![[represent-banner-rail.jpg]]
*Banner'ın hemen altında ürün şeridi: editoryal anlatım ile alışveriş aynı kaydırmada.*

> [!tip] Desen: "Hikâye + raf"
> Her editoryal banner'ın altına aynı koleksiyondan 8 ürünlük yatay şerit ve tek bir altı çizili "→ TÜMÜNÜ GÖR" linki. Banner 16:10 tam genişlik, şerit kartları 3:4, kart zemini #F7F7F7, kartlar arası 1px beyaz çizgi.

## Kategori sayfası (PLP)
- Başlık bloğu: **"Footwear"** (16px/500) + üst simge sayı "31", açıklama satırı (12px/300), "View All | Footwear" alt kategori sekmeleri.
- Izgara yoğunluk değiştirici (1 / 2 / 4 sütun ikonları) solda, "Filter & Sort" sağda (çekmece).
- Masaüstü 4 sütun **kenardan kenara**, kartlar 359x479px (3:4), aralarında 1px beyaz boşluk; mobil 2 sütun.
- Kart anatomisi: sağ üstte kaydet ikonu (45x45), sağ altta "+" hızlı ekle; altında 14px iç boşlukla ad (12px/500, sol) + fiyat (sağ), renk adı (#737373), 15px yuvarlak swatch'lar + "4 Colors". Tükendi: fiyat yerine "SOLD OUT". Rozet: "Restocked", "New Arrival", "US Exclusive" (10px, #575757).
- Alt: "Viewing 1 - 31 out of 31 products", ardından SEO metni.

## Ürün sayfası (PDP)

![[represent-pdp-desktop.jpg]]
*PDP: solda 720x900 tek görsel slider (1 / 5 sayaç), sağda geniş beyaz bilgi alanı.*

- Galeri: sol yarı 720x900 (4:5) slider, ok düğmeleri, sol altta "1 / 5" sayaç (beyaz kutu), sağ altta tam ekran ikonu.
- Bilgi sütunu 472px: ad (12px/500) + fiyat aynı satırda; "Color 4 · Dark Brown" + 4 renk küçük görseli (65x80); "Size" + US8–US13 butonları (58x40, #F7F7F7, radius 2px); seçince "Size US9 **Low stock**" uyarısı ve "TRY ON IN-STORE" butonu çıkıyor.
- **ADD TO CART:** 472x52px, #000000, beyaz 12px/500 uppercase, radius 0. Altında ikonlu güven satırları (her biri ok'lu): "Free Standard Shipping", "Ships from the USA", "Earn 345 Prestige Points", "Make 4 interest-free payments of $86.25 USD fortnightly" (Afterpay logosu).
- Accordion yerine yan yana iki sekme: "+ Product Details", "+ Shipping & returns". Açıklama: hikâye paragrafı + 11 maddelik özellik listesi + "Composition" + "Product Care" + stil kodu.
- Çapraz satış: "STYLE WITH" (4 ürün) ve "YOU MAY ALSO LIKE" (sekmeler: SUGGESTED / PANTS / T-SHIRTS, "LOAD MORE").
- Mobil: tam genişlik siyah yapışkan "ADD TO CART" alt çubuğu.

## Sepet ve satın alma kolaylığı
- Sağdan 440px çekmece, arka plan bulanıklaştırılıyor. Başlık "YOUR CART¹", altında yeşil (#468847) ilerleme çizgisi + "You've unlocked free standard shipping".
- Özet kutusu (açık gri zemin, ekran görüntüsünden): Subtotal, "Standard Shipping: Free" (yeşil), "Gift cards & promotional codes applied at checkout".
- Ürün satırı: görsel, ad, fiyat, beden, renk, −/+ adet, kaydet ve sil ikonları. "OTHERS ALSO BOUGHT" yatay karusel ("+" hızlı ekle).
- Alt sabit: "TOTAL", siyah **"SECURE CHECKOUT 🔒"** (404x52), altında Visa, Mastercard, Amex, PayPal, Apple Pay, Afterpay, UnionPay, Klarna logoları.

## Mobil deneyim
Ana sayfa panelleri alt alta; hero başlığı 24px'e düşüyor; PLP 2 sütun ve "read more" ile kısaltılan açıklama; PDP'de yapışkan siyah sepete ekle çubuğu.

## Güven ve ikna unsurları
| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| "Low stock" seçilen bedende | PDP | Kıtlık | Evet (gerçek stokla) |
| Ücretsiz kargo ilerleme çubuğu | Sepet çekmecesi | Hedef gradyanı | Evet: "₺X daha ekle, kargo bedava" |
| Taksit satırı (Afterpay) | PDP CTA altı | Ağrı azaltma | Evet: "3 taksit" / "peşin fiyatına 6 taksit" |
| Sadakat puanı satırı | PDP | Kazanç çerçevesi | Sonra |
| "Restocked" rozeti | Kart | Sosyal kanıt / talep | Evet |
| "TRY ON IN-STORE" | PDP | Risk azaltma | Mağaza varsa |

## Performans ve teknik gözlem
Shopify + Tailwind; görseller speedsize CDN'den. Ana sayfa 445 istek / 4,5 MB; marka sayfası 577 istek / **16,8 MB** (ağır). Çerez penceresinde yalnızca "ACCEPT & CLOSE" ve "PREFERENCES" vardı, reddet seçeneği yok (araç kabul etti).

## Güçlü yanlar / Zayıf yanlar
- **Güçlü:** Banner + şerit ritmi; buzlu cam CTA ve metin kaydırma hover'ı; PDP güven satırları; sepet çekmecesinin eşik göstergesi.
- **Zayıf:** Marka sayfası 16,8 MB; ana sayfada ürün yok, bir tık fazla; 12px'e sıkışmış hiyerarşi (ad, renk, fiyat aynı boyutta).

## KPT için çıkarımlar
- **Uygula:** Hero altında 8 ürünlük yatay şerit + altı çizili "→ KOLEKSİYONU GÖR"; PDP'de CTA altına 3 ikonlu güven satırı (kargo, iade, taksit); sepet çekmecesinde ücretsiz kargo eşik çubuğu; seçilen bedende "Son 2 çift".
- **Uyarla:** Bölünmüş kapı → "Erkek | Kadın" veya "Sneaker | Outdoor (Columbia)" 50/50 hero; buzlu cam CTA'yı KPT'nin bordosuyla değil, `rgba(23,27,28,.3)` + 1px `rgba(255,255,255,.3)` ile; başlıkta -0.05em sıkı harf aralığı.
- **Kaçın:** 16 MB'lık uzun editoryal sayfa; reddet seçeneği olmayan çerez penceresi.

İlgili: [[Hero ve Banner Desenleri]], [[Renk ve Tipografi]], [[Kategori Sayfası ve Filtreler]], [[Ürün Sayfası]], [[Sepet ve Ödeme]], [[Güven Sinyalleri]], [[KPT Store Denetimi]]

## Ekran görüntüleri
Gömülü: `represent-home-desktop.jpg`, `represent-banner-hero.jpg`, `represent-banner-rail.jpg`, `represent-pdp-desktop.jpg`.

## Kaynaklar
- https://representclo.com/ (2026-10-04 gözlem)
- https://representclo.com/pages/represent-home (2026-10-04 gözlem)
- https://representclo.com/collections/footwear-all (2026-10-04 gözlem)
- https://representclo.com/products/rep-cap-distressed-leather-dark-brown (2026-10-04 gözlem)
