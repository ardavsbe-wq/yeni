---
tür: rakip-analizi
site: END. Clothing
url: https://www.endclothing.com/
ülke: UK
segment: premium sneaker ve menswear butiği (çok markalı)
erişim: kısmi
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.endclothing.com/us, https://www.endclothing.com/us/footwear/sneakers, https://www.endclothing.com/us/new-balance-983-sneaker-u9835du.html, https://www.endclothing.com/us/launches/all-launches]
etiketler: [rakip, premium-sneaker-butigi, global-butik]
---

# END. Clothing

> [!summary] Özet
> Newcastle merkezli END., premium menswear ve sneaker satan, editoryal içerikle ticareti birleştiren çok markalı bir butik. Siteye girince otomatik olarak `/us` sürümüne (USD) yönlendirildik. En güçlü 3 yanı: (1) Proxima Nova + #1A1A1A tek renkli, sıkı ve premium bir görsel dil, (2) 4 sütunlu beden ızgarası, beden seçmeden sepete basınca kırmızı doğrulama ve beden ızgarasının hemen altında net teslim tarihi, (3) her yerde tekrarlanan "vergiler dahil" güven mesajı. KPT için en değerli ders: Ürün sayfasında beden ızgarası + teslim tarihi + "ek ücret yok" satırı + mobilde sabit sepete ekle çubuğu. Bunlar KPT'nin bilinen eksiklerini birebir kapatıyor.

> [!warning] Erişim notu
> Her sayfa yüklemesinde sitenin kendi API'si (`api2.endclothing.com/.../countries/` ve `paymentMethodsByCountryCode`) 416 hatası verdi. Ekranın ortasında "ERROR / Request failed with status code 416 / OK" modalı açıldı. Modalı kapatıp inceledik. Ancak **sepete ekleme bu yüzden tamamlanmadı**: sepet çekmecesi ve ödeme adımı incelenemedi. Bu hata muhtemelen bizim proxy ortamımızdan kaynaklanıyor (tahmin). Bot engeli değil.

## Kimlik ve konumlandırma
- Sayfa başlığı: "Style. Sneakers. Culture. Community. | END. (US)". Meta açıklaması: "The leading retailer of style, sneakers, culture, community."
- Üstte MEN / WOMEN ayrımı var (iki ayrı mağaza gibi). Sneaker kataloğu sneakers PLP'sinde **560 ürün**.
- Ticaret ile editoryali bir arada kuruyor: ana sayfada tarihli "FEATURES" makaleleri, "THE EDITS" ve marka blokları var.

## Görsel dil
| Rol | Hex | Kullanım yeri |
|---|---|---|
| Birincil metin / buton | #1A1A1A | Metin, "SHOP NOW", "ADD TO CART", üst şerit zemini |
| İkincil metin | #999999 | Ürün kartında renk adı, pasif "WOMEN" |
| Görsel zemini | #EEEEEE | Ürün fotoğrafı arka planı, filtre chip çerçevesi |
| Yüzey | #FAFAFA / #F8F8F8 / #F5F5F5 | Karusel okları, arama kutusu, "ADD TO WISHLIST" |
| İndirim vurgusu | #AE0000 | Menüdeki "Sale" |
| Zemin | #FFFFFF | Sayfa |

- **Tipografi:** Yalnızca Proxima Nova kullanılıyor (400/600). Neredeyse tüm başlıklar BÜYÜK HARF ve geniş harf aralıklı (harf aralığı ≈ font boyutu × 0.1):
  - Hero H2: 32px 600, ls 3.2px
  - Bölüm H2: 22px 600, ls 2.2px
  - PLP H1: 18px 600, ls 1.8px
  - Filtre başlığı: 14px 600, ls 1.4px
  - Gövde metni: 14px 400, ls 0.28px
  - Etiket ("■ LATEST"): 10px
- Köşeler neredeyse sıfır: hero CTA 2px, arama kutusu 4px, sepete ekle 0px. Dairesel olan tek öğeler 40px karusel okları ve 64px canlı destek balonu.
- Fotoğraf dili: ürünler açık gri (#EEEEEE) zemin üzerinde, yandan profil, gölgesiz stüdyo çekimi. Kampanyalar ise açık zeminli editoryal portreler.

## Header ve navigasyon
- **Üst şerit** (#1A1A1A, 40px yükseklik, kayan marquee, 10px büyük harf). Metinler birebir: "ALL IMPORT DUTIES INCLUDED • LATEST SNEAKERS: ADIDAS, NEW BALANCE, VANS • NEW IN: BIG ROCK CANDY MOUNTAINEERING, DRAKES, GANDER • SHOP FALL AT END. • MID-SEASON SALE, UP TO 60% OFF".
- **1. satır (57px):** Solda MEN (koyu) / WOMEN (gri) sekmeleri, ortada "END." logosu. Sağda "Search menswear" arama kutusu (197×34, #F8F8F8 zemin, 4px köşe) ve hesap, favori, sepet ikonları.
- **2. satır (56px):** New In · Brands · Footwear · Clothing · Accessories · Lifestyle · Active · Launches · **Sale** (kırmızı). Header toplam 153px. `headroom` sınıfı taşıyor: aşağı kaydırınca gizlenip yukarı kaydırınca geri gelen davranış (tahmin).
- **Footwear mega menüsü** (tam genişlik, 4 sütun):
  - VIEW ALL FOOTWEAR: Latest Sneakers, Footwear Bestsellers, Sneakers, Boots, Running, Shoes, Sandals & Slides, Slippers
  - FOOTWEAR BRANDS: adidas, Air Jordan, Asics, New Balance, Nike, Puma, Salomon, Saucony, Vans…
  - TRENDING STYLES: adidas BW Army, adidas Samba, New Balance 992, Salomon XT-6…
  - FEATURED: 2 görsel kart ("Sneakers", "Birkenstock")
- **Launches mega menüsü:** VIEW ALL LAUNCHES, Sneaker Launches, Apparel Launches + LAUNCHES BRANDS (Nike, Adidas, New Balance, Asics, Puma) + 4 görsel kart.
- **Mobil:** hamburger · logo · arama · sepet. Altında MEN / WOMEN sekmeleri tam genişlikte.

## Ana sayfa ve banner/hero örnekleri
**Hero:** Tam genişlikte, yaklaşık 1408×750 boyutunda 5 slaytlık karusel. Metin sol altta (x=32), fotoğrafın alt kısmında koyu degrade var. Altta 47×2px çizgi şeklinde sayfalama göstergeleri.

| Slayt | Başlık (birebir) | Alt metin | CTA |
|---|---|---|---|
| 1 | (kırmızı "sale" tipografi görseli) | – | SHOP SALE |
| 2 | FALL '26 AT END. | The brands, jackets, knits, and footwear to know this season | SHOP NOW |
| 3 | NEW-SEASON JACKETS | Explore our outerwear picks from workwear to down, waxed, technical, and more | SHOP NOW |
| 4 | NEW-IN FOOTWEAR | Picks from Diemme, Birkenstock, Fracap, and more | SHOP NOW |

CTA ölçüleri: 168×46, #1A1A1A zemin, beyaz yazı, 16px 600 büyük harf, ls 1.6px, 2px köşe.

**Bölüm sırası (yukarıdan aşağı):**
1. Hero karusel
2. NEW IN: 10 ürünlü karusel, "VIEW ALL" ve 40px yuvarlak oklar
3. DANIEL SIMMONS marka bloğu: solda 680px yaşam tarzı fotoğrafı ve "SHOP NOW", sağda ürün karuseli
4. NEW IN SNEAKERS: 5'li görünür karusel
5. THE EDITS: KNITWEAR / CHECKS / TROUSERS / HATS, büyük dikey kartlar
6. MELLOW CLO marka bloğu
7. LIFESTYLE: tam genişlik banner, "The latest in lifestyle" + SHOP NOW
8. FEATURES: tarihli 3 editoryal kart, örn. "01/10/2026 — ALINA AKBAR LEARNED TO SEE THROUGH HER CAMERA", 21px büyük harf, VIEW ALL
9. Bülten: "SIGN UP TO THE END. MENSWEAR MAILING LIST — Sign up to hear about exclusive early sale access, and new collections."
10. Footer

Editoryal içerik ve ticaret şöyle bağlanıyor: marka bloğu = editoryal fotoğraf + o markanın satın alınabilir ürünleri yan yana.

## Launch / çekiliş mekaniği
- Menüdeki "Launches" ve `launches.endclothing.com` artık normal bir PLP'ye gidiyor: "MEN'S ALL LAUNCHES", **145 ürün**, standart filtrelerle. Açıklama metni: "Discover the best new sneaker drops available today and preview what's coming next across upcoming launches before they go live."
- Web'de **çekiliş/kayıt arayüzü görmedik.** Ürünler "■ LATEST" rozetiyle normal satılıyor. END.'in çekilişleri uygulama üzerinden yürüttüğü bilgisi doğrulanmadı (tahmin).

## Kategori sayfası (PLP)
- Breadcrumb: "Mens > Footwear > Sneakers".
- Üst blok: solda gölgeli beyaz kutu. İçinde H1 "MEN'S SNEAKERS", 4 satırlık SEO metni + "read more" ve "SHOP MEN / SHOP WOMEN" sekmeleri. Sağda yaşam tarzı fotoğrafı.
- Trend chip'leri: Adidas, Nike, Puma, Diemme, Y-3, Eytys. 28px yükseklik, 1px #EEEEEE çerçeve, 4px köşe, 12px yazı.
- Sonuç satırı: "560 products". Uygulanan filtre chip'i ("Sneakers ×") ve "Clear all".
- Sol kenar çubuğu (310px), akordeon filtreler, her seçenekte ürün sayısı:
  - BRAND (kendi içinde arama kutusu var)
  - DEPARTMENT
  - FOOTWEAR STYLE (model bazlı, örn. "New Balance 1890 7")
  - COLOUR
  - CLOTHING SIZE
  - FOOTWEAR SIZE (UK ve EU ayrı listeleniyor, örn. "EU 42 454")
  - PRICE (min/max $ kutuları)
- Sağ üst: "View: Product / Outfit" anahtarı ve sıralama (Featured / Latest / Price (Low) / Price (High)).
- Izgara masaüstünde 4 sütun. Kart anatomisi:
  - #EEEEEE zeminde kare görsel
  - "■ LATEST" 10px büyük harf
  - Ad 14px #1A1A1A
  - Renk adı 14px #999999
  - Fiyat 14px
- Sayfalama: incelenemedi.

## Ürün sayfası (PDP)
- **Galeri:** Solda 74px küçük görsel sütunu (6 görsel). Ana görseller 566×566, #EEEEEE zeminde alt alta diziliyor. Sağdaki bilgi kolonu kaydırırken **sabit (sticky)** kalıyor.
- **Başlık yapısı (ortalı):**
  - "■ LATEST"
  - "NEW BALANCE 983 SNEAKER" (18px 600, ls 1.8px)
  - "Shadow Blue & Zinc Blue" (14px #999999)
  - "$209" (16–18px 600)
- **Beden seçici:**
  - "Select a size" etiketi ve sağda ikonlu "Size guide" linki.
  - Izgara 4 sütun × 3 satır, hücre 97×43, 1px çizgi, 12px yazı, ls 1.2px. Gösterilen bedenler UK 6–11.5.
  - Seçilen bedende 2px #1A1A1A çerçeve ve 600 kalınlık var. Etiket "Select a size" yerine seçilen bedene ("UK 8") dönüşüyor.
  - Stokta olmayan beden gösterimi görülmedi. Ya hepsi stoktaydı ya da tükenen bedenler hiç gösterilmiyor (tahmin).
- **Doğrulama:** Beden seçmeden "ADD TO CART"a basınca "Select a size" yazısı ve ızgara çerçevesi kırmızıya dönüyor, buton griye geçiyor. Butonu baştan pasif yapmak yerine hatayı gösteriyorlar.
- **Butonun üstünde güven satırları (birebir):** "Order now to receive **Wed 07 Oct - Fri 09 Oct.**" (tarih yeşil) ve "We cover Import Duties - no hidden fees at checkout."
- **CTA'lar:** "ADD TO CART" 300×44, #1A1A1A zemin, 16px 600, 0px köşe. "ADD TO WISHLIST" 300×44, #F5F5F5 zemin, koyu yazı.
- **Sekmeler:** DESCRIPTION / SHIPPING / RETURNS (aktif sekmenin altı çizgili). Açıklama: 1 paragraf hikâye metni, 4 maddelik özellik listesi ve "Style Code: U9835DU".
- Yorum bölümü yok.

## Sepet ve satın alma kolaylığı
- Sepete ekleme geri bildirimi: incelenemedi. Butona basınca gri yüklenme durumuna geçti, ardından 416 hata modalı çıktı.
- Mobil PDP'deki kargo bölümü (birebir):
  - "FREE FedEx IC Plus Service on orders over $200.00"
  - "$14.99 via FedEx IC Plus Service"
  - "$19.99 via FedEx International Priority"
  - Her seçeneğin altında yeşil renkli teslim tarih aralığı
  - "All shipments to United States are Delivery Duty Paid"
- İade metni: "you can return it to us within 30 days for an exchange or refund."

## Mobil deneyim
- PDP'de görseller kaydırmalı galeri, altında 6 nokta gösterge. Bilgiler ortalı, beden ızgarası 4 sütun.
- **Ekranın altında sabit, tam genişlik siyah "ADD TO CART" çubuğu** var (≈370×44).
- Favori, ikonlu metin linki olarak gösteriliyor ("Add to Wishlist").
- Açıklama, kargo ve iade sekme yerine alt alta bölümler halinde.
- Sağ altta 64px #1A1A1A sohbet balonu her sayfada duruyor ve içeriğin üstüne biniyor.

## Güven ve ikna unsurları
| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| "ALL IMPORT DUTIES INCLUDED" / "no hidden fees" | Üst şerit + PDP | Sürpriz maliyetten kaçınma (Baymard: beklenmedik ek ücret, sepeti terk sebeplerinin başında) | Evet: "Tüm vergiler dahil, ödemede ek ücret yok" |
| Somut teslim tarih aralığı | PDP, buton üstü | Somutluk, belirsizliği azaltma | Evet: "Sipariş ver, 7–9 Ekim arası kapında" |
| "■ LATEST" rozeti | Kart + PDP | Yenilik etkisi | Evet: "YENİ" |
| Ücretsiz kargo eşiği ($200) | Kargo bölümü | Hedefe yaklaşma (goal gradient) | Evet, sepette ilerleme çubuğu ile |
| 30 gün iade | Returns sekmesi | Risk azaltma | Evet |
| Tarihli editoryal makaleler | Ana sayfa | Otorite ve hikâye anlatımı | Uyarla: haftalık kısa yazı |

## Performans ve teknik gözlem
- Ana sayfa masaüstü: TTFB 845ms, DOMContentLoaded 3.0sn, load 5.8sn, 293 istek, **5.1 MB**. 120 görselin 37'si lazy, çoğu JPG.
- PLP: 226 istek, 1.45 MB, load 2.2sn.
- Arama Algolia ile çalışıyor (`search1web.endclothing.com/.../queries`).
- Teknik hata (API 416) kullanıcıya ham metinle, ekranı kilitleyen bir modal olarak gösteriliyor. Logo ile SPA geçişinde de "SOMETHING WENT WRONG / THERE IS A PROBLEM WITH END. / We are experiencing a problem and will be back soon" sayfası çıktı.

## Güçlü yanlar / Zayıf yanlar
- **Güçlü:** Tutarlı tipografik sistem (tek font, büyük harf, harf aralığı). Doğrulamalı beden ızgarası. Butonun hemen üstünde teslim tarihi ve vergi mesajı. Sayılı ve model bazlı filtreler. Sticky bilgi kolonu. Mobilde sabit sepete ekle çubuğu.
- **Zayıf:** Ham teknik hata modalı. 5 MB ana sayfa. Gri "WOMEN" sekmesi pasif görünüyor. Hero alt metni 14px beyaz ve fotoğraf üzerinde, kontrastı zayıf. Ürün yorumu yok.

## KPT için çıkarımlar
- **Uygula:**
  - PDP'de 4 sütunlu beden ızgarası: hücre ≈97×43, 1px #171B1C20 çizgi. Seçili hücre 2px #171B1C çerçeveli olsun ve etiket seçilen bedeni ("42") göstersin.
  - Beden seçmeden "Sepete Ekle"ye basılınca etiket ve ızgara çerçevesi bordo (#741E32) olsun, butonu baştan pasif yapma.
  - Butonun hemen üstüne 2 satır ekle: "Bugün sipariş ver, **8–10 Ekim** arası kapında" (tarih vurgulu) ve "Tüm vergiler dahil — ödemede ek ücret yok".
  - Mobilde ekranın altında sabit, tam genişlik "Sepete Ekle" çubuğu.
  - PLP filtrelerini akordeon ve sayılı yap ("Beden 42 (54)"). Sıralama: Önerilen / En yeni / Fiyat artan / Fiyat azalan.
- **Uyarla:**
  - 40px koyu üst şerit, 3–5 mesaj dönüşümlü: "Tüm vergiler dahil • 30 gün ücretsiz iade • 9 taksit".
  - Marka bloğu: sol yarıda yaşam tarzı fotoğrafı, sağda o markanın ürün karuseli (örn. New Balance 1906R).
  - PLP üstünde trend chip'leri: "New Balance 530", "Samba", "Air Force 1".
- **Kaçın:**
  - Ham API hatasını modal ile gösterme.
  - 5 MB'lık ana sayfa.
  - Pasif görünen gri sekmeler.
  - Fotoğraf üstünde 14px ince açık renk metin.
  - İçeriği kapatan sohbet balonu.

İlgili desen notları: [[Ürün Sayfası]] · [[Beden ve Kalıp]] · [[Header ve Navigasyon]] · [[Hero ve Banner Desenleri]] · [[Kategori Sayfası ve Filtreler]] · [[Güven Sinyalleri]] · [[Mobil Deneyim]] · [[Renk ve Tipografi]] · [[KPT Store Denetimi]]

## Ekran görüntüleri
![[endclothing-masaustu-hero.jpg]]
Masaüstü: koyu üst şerit, iki satırlı header ve 5 slaytlık hero ("NEW-SEASON JACKETS" slaytı).

![[endclothing-mega-menu.jpg]]
Footwear mega menüsü: 4 sütun, en sağda 2 görsel kart.

![[endclothing-pdp-beden.jpg]]
PDP: beden seçmeden sepete basınca kırmızı doğrulama (etiket + ızgara çerçevesi), butonun üstünde teslim tarihi ve vergi satırları.

![[endclothing-mobil-pdp.jpg]]
Mobil PDP: kaydırmalı galeri, 4 sütun beden ızgarası, sabit "ADD TO CART" çubuğu, kargo seçenekleri.

## Kaynaklar
- https://www.endclothing.com/us (doğrudan gözlem, 2026-10-04)
- https://www.endclothing.com/us/footwear/sneakers
- https://www.endclothing.com/us/new-balance-983-sneaker-u9835du.html
- https://www.endclothing.com/us/launches/all-launches
- https://baymard.com/lists/cart-abandonment-rate (ek ücretlerin sepet terkindeki rolü; bütçe nedeniyle bu oturumda yeniden açılmadı)
