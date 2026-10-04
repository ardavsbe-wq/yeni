---
tür: rakip-analizi
site: Aimé Leon Dore
url: https://www.aimeleondore.com/
ülke: US
segment: premium streetwear / lifestyle marka DTC
erişim: tam
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.aimeleondore.com/, https://www.aimeleondore.com/collections/footwear, https://www.aimeleondore.com/products/ald-new-balance-1300]
etiketler: [rakip, streetwear, tasarim-lideri, new-balance]
---

# Aimé Leon Dore

> [!summary] Özet
> Queens, New York çıkışlı (2014) lifestyle markası; New Balance, Clarks, The North Face işbirlikleriyle premium sneaker kitlesine satıyor. En güçlü 3 yanı: (1) ana sayfanın **tek ekranlık, metinsiz, sesli/sessiz tam ekran film** olması, (2) tüm sitede **tek font (Söhne), tek ağırlık (400), 10–12px** ile kurulan sessiz tipografi, (3) **#F6F6F6 zeminli, tek tip 4:5 ürün fotoğrafı** disiplini. KPT için ders: premium algı renk ve büyük başlıkla değil, **kısıtla** (az öğe, küçük tip, bol beyaz, tutarlı fotoğraf) kuruluyor. KPT'nin New Balance kataloğu bu dille doğrudan sergilenebilir.

## Kimlik ve konumlandırma
- Meta açıklama: "Created in 2014, Aimé Leon Dore is a fashion and lifestyle brand based out of New York City."
- Ürün adlandırması işbirliğini öne çıkarır: "ALD / New Balance Made in USA 1300" ($220), "ALD / New Balance RC56" ($165), "ALD / Clarks Suede Wallabee" ($230). Ayakkabı PLP'sinde 46 üründen ~20'si New Balance.
- Marka anlatımı ürün sayfasında değil, ana sayfa filminde ve menüdeki "EXPLORE" sekmesinde (editoryal) yaşıyor.

## Görsel dil

### Renk paleti (hesaplanmış stillerden)
| Rol | Hex | Kullanım yeri |
|---|---|---|
| Ana metin / CTA dolgu | #181818 | Tüm metin, "ADD TO BAG" ve "NEXT: HEADWEAR" buton zemini |
| Zemin | #FFFFFF | Sayfa, header (iç sayfalarda) |
| Ürün fotoğraf zemini | #F6F6F6 | Fotoğrafın içinde (CSS değil, JPG'ye gömülü) |
| Çizgi / ayırıcı | #E5E5E5 | Header alt çizgisi 1px, mobil filtre kutuları |
| Seçenek hover | #EFEFEF | Beden açılır listesinde hover satırı |
| Menü çekmecesi zemini | #373737 (ekran görüntüsünden ölçüldü) | Sol menü paneli |
| Menü linki | #C4C4C4 @0.7 | Çekmecedeki kategori linkleri |
| Hero üzeri metin | #FFFFFF | Video üstündeki logo, tarih satırı, ikonlar |

**Az renkle premium:** Sitede vurgu rengi yok. Renk tamamen ürün ve film karelerinden geliyor (hero videoda sıcak kahve/ahşap tonları). Arayüz yalnızca #181818 / #FFFFFF / #F6F6F6 üçlüsü.

### Tipografi
- **Aile:** Söhne (CSS adı "Sohne"), sitede 120+ metin öğesinin tamamı; yalnızca PLP/PDP alt butonlarında "DIN W01 Regular".
- **Ağırlık:** Her yerde 400. Kalın yazı yok.
- **Ölçek (masaüstü):** 10px (ürün adı, fiyat, açıklama, accordion), 12px (H1 ürün adı, breadcrumb, sıralama), 17px (yalnızca gizli H1 logo metni). Logo SVG wordmark 130x21px.
- **Harf aralığı:** Gövde 0.5–0.6px; büyük harf menü 1.4px (10px uppercase); buton 1.0–1.1px (DIN 10–11px uppercase).
- **Satır yüksekliği:** 10px metinde 14.1px (1.41).
- Mobilde ürün adı 11px / 0.55px, fiyat 10px / 0.7px.
- Büyük harf yalnızca navigasyon ve butonlarda; ürün adları normal yazım.

### Fotoğraf stili
- **Ürün:** Stüdyo, çift ayakkabı 3/4 açıdan, #F6F6F6 düz zemin, yumuşak gölge, ürün kadrajın ~%60 genişliği. Oran 4:5 (600x750 kaynak). PDP galerisi 7 kare: 3/4 çift, çift, üstten, arkadan, yakın detay, iç taban üstten, dış taban.
- **Marka:** Sinematik film (24 fps), sıcak loş ışık, mekân hikâyesi (plak arşivi, DJ masası).

### Hareket
- Genel geçiş: `all 0.5s ease` (52 öğe), ürün kartı görselleri `transform 0.2s ease`, `all 0.4s linear`.
- Kaydırınca header'daki "AIMÉ LEON DORE" wordmark'ı **çiçekli arma amblemine** dönüşüyor (masaüstü ve mobil).
- PLP kartında 7 görsellik gizli kaydırıcı var; hover'da görünür değişim yakalanmadı.

## Header ve navigasyon
- Yükseklik 61px, `position: fixed`; ana sayfada şeffaf ve beyaz ikonlu, iç sayfalarda #FFFFFF + 1px #E5E5E5 alt çizgi.
- Düzen: solda hamburger (16x17px), ortada logo, sağda arama / hesap / çanta ikonları. Üst duyuru şeridi yok.
- Menü: soldan açılan 450px koyu çekmece (#373737), üstte iki sekme "SHOP" / "EXPLORE" (her biri 225x61px), arka planda soluk arma filigranı. Linkler 10px, uppercase, 1.4px aralık, 35px satır aralığıyla: ALL PRODUCTS, NEW ARRIVALS, WOMENS / boşluk / TEES & POLOS … GIFT CARDS (19 öğe). Altta e-posta alanı + "Subscribe".

## Ana sayfa ve banner/hero örnekleri

![[ald-hero-desktop.jpg]]
*Masaüstü ana sayfa: tam ekran film (video karesi kompozit olarak eklendi; headless tarayıcı H.264 oynatamadığı için kare ffmpeg ile çıkarıldı), üstte beyaz logo ve canlı tarih satırı.*

**Hero 1 (sayfanın tamamı):**
- **Görsel türü:** Vimeo MP4 video, 1920x1080, 24 fps, 32,9 sn, autoplay + loop + muted. İçerik: ALD x New York Yankees parçalarıyla plak arşivi önünde iki DJ (lifestyle film).
- **Kırpma/oran:** Video 1613x927 boyutunda viewport'tan taşacak şekilde ölçekli (16:9 kaynak, viewport'u kaplayan "cover" etkisi). Sayfa yüksekliği 931px: **ana sayfada kaydırma yok, başka bölüm yok.**
- **Başlık metni:** Yok. Tek metin, logonun altında ortalanmış canlı tarih/saat satırı: **"Queens, NY | Saturday, October 03, 2026 | 21:48 EST"** (Söhne 10px, 0.6px, #FFFFFF, y=61–96px).
- **CTA:** Yok. Sol altta 30x30px yuvarlak beyaz ses aç/kapa düğmesi (25px kenar boşluğu).
- **Metin-görsel ilişkisi:** Metin neredeyse yok; film tek başına marka anlatımı. Alışveriş yalnızca hamburger menüden.

**Bölüm sırası:** Yalnızca hero (footer bile ana sayfada görünmüyor).

> [!example] KPT için hero çevirisi
> Tam ekran, 15–30 sn, sessiz başlayan bir atölye filmi (ayakkabı temizleme, bağcık takma, kutu açma), üstte tek satır 10–12px "İstanbul | 4 Ekim 2026 | 14:05" tipi canlı yer/saat satırı. Video 1080p H.264 + WebM, ≤4 MB, poster kare zorunlu.

## Kategori sayfası (PLP)

![[ald-plp-desktop.jpg]]
*Ayakkabı PLP: 4 sütun, #F6F6F6 zeminli 4:5 görseller, kartta yalnızca ad ve fiyat.*

- Izgara: CSS grid `337px x 4`, sütun aralığı 14px, sayfa kenar boşluğu 25px; görsel 337x421 (4:5), kart toplam 497px yükseklik. Mobil 2 sütun, görsel ~190px genişlik, aralık ~8px.
- Kart anatomisi: görsel → 20px boşluk → tek satırda solda ürün adı (10px, #181818), sağda fiyat. Rozet, swatch, yıldız, "yeni" etiketi **yok**. Kadın ürünlerinde adın üstünde "Women's".
- Tükendi: fiyat yerine "SOLD OUT".
- Üst çubuk: "Shop All > Footwear +" breadcrumb (12px), sağda "Sort: Recommended" ve "Refine". Mobil filtre: "Size", "Color", "View Options", "Hide sold out products", "My Sizes" (kayıtlı beden).
- Sayfalama yok: tüm 46 ürün tek sayfada; en altta tam genişlik siyah "NEXT: HEADWEAR" butonu (335x60px, DIN 11px uppercase 1.1px) sonraki kategoriye geçiriyor.

## Ürün sayfası (PDP)

![[ald-pdp-desktop.jpg]]
*Masaüstü PDP: üç sütun; solda bilgi, ortada dikey kaydırılan galeri, sağda beden ve sepet.*

- **Üç sütunlu düzen (masaüstü):** sol sütun (x=60, ~285px) başlık 12px + fiyat 12px + kalıp notu 10px ("Fits true to size. Order your normal size…") + 3 accordion (Product Details / Sizing / Delivery and Returns, her biri 285x45px, alt çizgi 1px #181818). Orta: 478x598px (4:5) görseller alt alta. Sağ: "Select Size" açılır kutusu (285x40px, 1px #E5E5E5) ve "ADD TO BAG" (285x60px, #181818 zemin, beyaz DIN 10px uppercase 1px aralık, radius 0).
- **Beden listesi:** US 4–13 görünür; stokta olmayanlar listeden kaldırılmıyor, satırın sağında **"Notify Me"** yazıyor (7.5–13). Satır yüksekliği 40px, hover #EFEFEF.
- **Mobil:** galeri üstte; alt kısımda yapışkan çubuk: ad + fiyat satırı, yan yana renk ("NAVY") ve "Select Size" kutuları, altında tam genişlik "ADD TO BAG" (342x40px).
- Teslimat: "All orders are shipped via UPS. This item ships in 1-3 business days."

![[ald-pdp-mobile.jpg]]
*Mobil PDP: yapışkan alt çubukta renk + beden + sepete ekle.*

## Sepet ve satın alma kolaylığı
incelenemedi: beden seçimi ve "ADD TO BAG" tıklaması otomasyonda zaman aşımına uğradı; bütçe kısıtı nedeniyle tekrar denenmedi.

## Mobil deneyim
Header 61px sabit; logo kaydırınca ambleme dönüşüyor; PLP 2 sütun; PDP'de yapışkan satın alma çubuğu (KPT'de eksik olan desen).

## Güven ve ikna unsurları
| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| Canlı yer/saat satırı | Hero | Otantiklik, "gerçek bir yer" | Evet: "İstanbul atölyesi" |
| Stoksuz bedende "Notify Me" | PDP beden listesi | Kayıp kaçınma, talep sinyali | Evet, doğrudan |
| İşbirliği adı ürün adında | PLP/PDP | Otorite / sosyal kanıt | Kısmen ("New Balance Made in USA" alt başlığı) |
| Kalıp notu başlığın altında | PDP | Belirsizlik azaltma | Evet |

## Performans ve teknik gözlem
Shopify. Ana sayfa: 211 istek, 1,9 MB, DOMContentLoaded 2,4 sn; PDP 3,1 MB. Hero video 1080p MP4 (~20 MB tam dosya), poster görsel yok: video yüklenene kadar ekran **beyaz** kalıyor (headless yakalamada tamamen beyaz).

## Güçlü yanlar / Zayıf yanlar
- **Güçlü:** Tek font/tek ağırlık sistemi; fotoğraf tutarlılığı; logo dönüşümü gibi küçük marka anları; stoksuz bedenlerin görünür kalması.
- **Zayıf:** 10px gövde metni okunabilirlik sınırında; ana sayfada hiçbir ürün yok (keşif tamamen menüye bağlı); posterli olmayan video beyaz ekran riski; güven bilgisi (iade, kargo eşiği) PDP'de accordion içinde gizli.

## KPT için çıkarımlar
- **Uygula:** Tüm ürün fotoğraflarını tek zemin rengine (#F3F4F1 veya #F6F6F6) ve tek orana (4:5) sabitle; kartta yalnızca ad (solda) + fiyat (sağda) tek satır. PDP'de stoksuz bedenleri gri + "Haber ver" etiketiyle göster. PLP sonunda "SONRAKİ: TERLİK" gibi tam genişlik kategori geçiş butonu.
- **Uyarla:** Tek fontla hiyerarşi: Manrope 400'ü 11–13px'te, uppercase etiketleri 1.2–1.4px aralıkla kullan; Cormorant'ı yalnızca film/editoryal başlıkta. Hero'da ürün kartlarını kaldırıp tek bir atölye filmi + tek satır canlı yer/saat.
- **Kaçın:** 10px gövde metni (KPT için minimum 12px); posterli olmayan video; ana sayfayı tamamen ürünsüz bırakmak (KPT'nin trafik kazanması gerekiyor, ALD'nin marka bilinirliği yok).

İlgili: [[Hero ve Banner Desenleri]], [[Renk ve Tipografi]], [[Ürün Sayfası]], [[Beden ve Kalıp]], [[Mobil Deneyim]], [[Görsel Tasarım ve Trendler 2026]], [[KPT Store Denetimi]]

## Ekran görüntüleri
Yukarıda gömülü: `ald-hero-desktop.jpg`, `ald-plp-desktop.jpg`, `ald-pdp-desktop.jpg`, `ald-pdp-mobile.jpg`.

## Kaynaklar
- https://www.aimeleondore.com/ (2026-10-04 gözlem)
- https://www.aimeleondore.com/collections/footwear (2026-10-04 gözlem)
- https://www.aimeleondore.com/products/ald-new-balance-1300 (2026-10-04 gözlem)
