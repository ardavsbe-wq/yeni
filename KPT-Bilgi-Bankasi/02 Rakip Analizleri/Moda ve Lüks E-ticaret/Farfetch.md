---
tür: rakip-analizi
site: Farfetch
url: https://www.farfetch.com/
ülke: UK
segment: lüks moda pazar yeri (butik + marka marketplace)
erişim: kısmi
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.farfetch.com/]
etiketler: [rakip, luks-pazar-yeri, moda]
---

# Farfetch

> [!summary] Özet
> Farfetch, 2007'de Londra'da kurulmuş, 1.400'ü aşkın marka, butik ve mağazanın ürününü 190'dan fazla ülkeye satan bir lüks moda pazar yeri. Ocak 2024'ten beri Coupang'ın (Wikipedia, 2026). Ana sayfada gözlenen en güçlü 3 yanı: (1) tek font ailesi ("Farfetch Basis"), iki renk (#222222 / #FFFFFF) ve sıfır köşe yuvarlaklığından oluşan sade bir görsel sistem, (2) karar yükünü azaltan "Choose a department" giriş ekranı (3 büyük departman kutusu ve her departman için 4 kategori kutusu), (3) 4 sütunlu, iyi gruplanmış bir footer ("Customer Service / About / Discounts and membership / Content and services"). KPT için en değerli ders: **Erkek / Kadın / Çocuk ayrımını ilk ekranda görsel kutularla vermek** ve bütün arayüzü tek font, tek koyu renk ve 24px'lik bir ızgara üzerine kurmak.

> [!warning] Erişim notu
> Ana sayfa açıldı (HTTP 200). **Erkek sneaker PLP'si (`/shopping/men/sneakers-2/items.aspx`) Akamai "Access Denied" (HTTP 403) döndürdü.** Ana sayfadaki menü linkine tıklayarak yapılan ikinci deneme (`/shopping/men/items.aspx`) de 403 aldı. Kurallar gereği aşılmaya çalışılmadı. **PLP, PDP ve sepet incelenemedi.** Ayrıca proxy yavaş olduğu için TTFB ~10 sn ölçüldü ve alt bölümlerdeki lazy-load görseller headless tarayıcıda yüklenmedi. Bunlar test ortamından kaynaklanıyor, gerçek kullanıcı deneyimini yansıtmıyor olabilir.

## Kimlik ve konumlandırma
- **Model:** Pazar yeri. Ürünler partner butik ve markalardan gönderiliyor. İade sayfasında "returned to our brand or partner boutique" ifadesi bunu doğruluyor (Farfetch UK Returns, 2026).
- **Ölçek:** 1.400'ü aşkın marka/butik/mağaza, 190'dan fazla ülkeye teslimat, yaklaşık 2.220 çalışan (Wikipedia, 2026).
- **Sahiplik:** Coupang'ın satın alması 31 Ocak 2024'te tamamlandı. Mayıs 2026'da "Farfetch First" adıyla, Avrupa'da bir sonraki güne ücretsiz teslimat yükseltmesi sunan premium hizmet başlatıldı (Wikipedia, 2026).
- **Sayfa başlığı:** "FARFETCH | The Global Destination For Modern Luxury".

## Görsel dil
| Rol | Hex | Kullanım yeri |
|---|---|---|
| Ana metin / birincil buton | `#222222` | Tüm metinler (67 öğe), "Sign Up" butonu dolgusu |
| Zemin | `#FFFFFF` | Sayfa, header |
| Açık gri yüzey | `#F5F5F5` | En üstteki 30px şerit, hesap ikonu zemini |
| Footer zemini | `#E6E6E6` | Footer bloğu |
| İkon (pasif) | `#B6B6B6` | Arama büyüteci |
| Ters metin | `#FFFFFF` | Departman kutularındaki büyük etiketler |

- **Tipografi:** Tek aile **"Farfetch Basis"** (grotesk, kuruma özel). Gövde ve link: 15px / 20px, 400. Bölüm başlıkları (H2 "Choose a department", "Womenswear"): 22px / 28px, 400, ortalı, normal harf. Kategori etiketleri ("NEW IN", "SHOES"): 15px, 400, `text-transform: uppercase`. Bülten başlığı (H3 "Never miss a thing"): 30px / 38px, 400. Footer sütun başlıkları: 15px, 700. Sayfada yalnızca 400 ve 700 ağırlıkları kullanılıyor. Harf aralığı normal.
- **Köşe:** Hiçbir öğede border-radius yok (0px). Butonlar ve inputlar keskin köşeli.
- **Izgara:** 1440px genişlikte kenar boşluğu 24px, sütun aralığı 24px. 4 sütun için sütun genişliği 330px (x = 24 / 378 / 732 / 1086).
- **Fotoğraf:** Departman kutuları 16:9 (447×251, dosya adında `16x9_three`). Kategori kutuları 3:4 (329×439, `3x4_fou`). Yaşam tarzı ve dış mekân çekimleri (beton duvar, şehir, çimen), düz ışık, bol negatif alan.
- **İkonlar:** 24px ince çizgili (kalp, çanta, büyüteç) ve 44×44 dokunma alanı.

## Header ve navigasyon
- **Üst şerit:** 30px yüksekliğinde, `#F5F5F5` zeminli bir şerit. İnceleme sırasında içeriği boş göründü (tahmin: duyuru içeriği geç yükleniyor).
- **Header:** `position: sticky`, masaüstünde 124px, mobilde 100px, beyaz zemin, alt çizgi yok.
  - Solda 3 link: "Womenswear", "Menswear", "Kidswear" (15px, 44px yükseklik).
  - Ortada logo (SVG, 201×25).
  - Sağda 4 ikon butonu (44×44): dil/bölge (bayrak), hesap, "Wishlist 0 items.", "Bag 0 items.". Ekran okuyucu etiketleri sayaç içeriyor.
  - İkinci satır sağda arama kutusu: 226px genişlik, yalnızca alt çizgili, büyüteç ikonlu, placeholder **"What are you looking for?"**.
- **Gizli mega menü linkleri (Womenswear):** "25% off", "New in", "Brands", "Clothing", "Shoes", "Bags", "Accessories". Yani indirim, yeni gelenler ve markalar kategori linklerinden önce geliyor.

## Ana sayfa ve banner/hero örnekleri
Kök URL, kişiselleştirilmemiş bir **departman seçim sayfası** gösteriyor. Bölüm sırası:
1. H2 "Choose a department" (22px, ortalı).
2. **3 departman kutusu:** her biri 16:9 fotoğraf, ortasında beyaz 30px büyük harf etiket ("WOMENSWEAR", "MENSWEAR", "KIDSWEAR"). Okunurluk için hafif koyulaştırma var gibi görünüyor (tahmin). Buton yok, kutunun tamamı link.
3. "Womenswear" başlığı ve 4 kutu (3:4 fotoğraf, altında 15px büyük harf etiket): NEW IN / CLOTHING / BAGS / SHOES.
4. "Menswear" başlığı ve 4 kutu: NEW IN / CLOTHING / ACCESSORIES / SHOES.
5. "Kidswear" başlığı ve 4 kutu: BOYS / GIRLS / BABY BOYS / BABY GIRLS.
6. Bülten: H3 "Never miss a thing", "Sign up for promotions, tailored new arrivals, stock updates and more – straight to your inbox", 300×42 e-posta inputu, `#222222` "Sign Up" butonu (91×44, 15px 700, radius 0) ve KVKK benzeri onay metni.
7. Footer.

## Kategori sayfası (PLP)
incelenemedi: Akamai 403, iki deneme (doğrudan URL ve menü tıklaması).

## Ürün sayfası (PDP)
incelenemedi: PLP'ye erişilemediği için PDP linki alınamadı.

## Sepet ve satın alma kolaylığı
Sepet ekranı incelenemedi. Herkese açık yardım sayfasından (Farfetch UK Returns, 2026):
- İade süresi: **"We accept returns within 30 days, starting from the day your order was delivered."**
- İki ücretsiz yöntem var: **"Book a free returns collection"** (adresten alım) ve **"Return for free at a drop-off point near you"**.
- İade işlenmesi en fazla 6 takvim günü, bankaya yansıması en fazla 14 gün sürüyor. Para Farfetch hesabına kredi (5 yıl geçerli) olarak da alınabiliyor.
- Ayakkabıda şart: giyilmemiş, etiketli ve orijinal kutusunda olmalı.
- Footer'da "Cryptocurrency payments" linki var (kripto ödeme).

## Mobil deneyim
- Header 100px ve sticky. Bayrak, hesap, kalp ve çanta ikonları sağda, arama alt satırda (16px, 226px). Mobilde 16px font, iOS'un input'a odaklanınca yaptığı otomatik zoom'u önler.
- Departman kutuları tek sütun. Kategori kutuları ortalanmış küçük görsel ve altında büyük harf etiketle diziliyor.
- **Gözlenen hata:** 390px genişlikte "Choose a department" butonu logoyla üst üste bindi. Bu, yükleme sırasındaki geçici bir durum olabilir (tahmin).

![[farfetch-ana-sayfa-mobil.jpg]]
*Mobil 390px: sticky header, buton ve logo çakışması, departman listesi.*

## Güven ve ikna unsurları
| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| "FARFETCH Customer Promise" linki | Footer, Customer Service | Risk azaltma / güvence | Evet: "KPT Güvencesi" sayfası (orijinal ürün, 14 gün iade, hızlı kargo) |
| İndirim programları listesi (öğrenci, sağlık çalışanı, emekli, "Refer a friend") | Footer | Karşılıklılık, aidiyet | Kısmen: öğrenci ve arkadaşını getir indirimi |
| "Second Life: sell your designer bags", "Refresh: clear out your wardrobe" | Footer | Sürdürülebilirlik, değer geri kazanımı | İleride: ikinci el sneaker takası |
| Ücretsiz iade alımı ve bırakma noktası | Yardım sayfası | Kayıptan kaçınma | Evet: "Ücretsiz iade" ifadesi PDP'de |
| Bültende "stock updates" vaadi | Ana sayfa | FOMO / kıtlık | Evet: "Bedenin gelince haber ver" |

## Performans ve teknik gözlem
- Masaüstünde 68 istek / 1.711 KB, mobilde 86 istek / 1.873 KB. TTFB 9,8 sn ve DOMContentLoaded 19,9 sn ölçüldü (proxy kaynaklı olabilir, gerçek değer değildir).
- 15 görselin 11'i `loading="lazy"`. Görseller CMS CDN'inden oran bazlı varyantla geliyor (`16x9_three`, `3x4_fou`). Oran adıyla görsel varyantı adlandırma, KPT için iyi bir pratik.
- Çerez penceresi çıkmadı (bölge bayrağı masaüstünde ABD, mobilde UK gösterdi).

## Güçlü yanlar / Zayıf yanlar
- **Güçlü:** Tek font, tek koyu renk ve 0 radius ile tutarlı sistem. 44px dokunma alanları. Ekran okuyucu için sayaçlı etiketler ("Bag 0 items."). Departman öncelikli bilgi mimarisi. Footer gruplaması.
- **Zayıf:** Kök sayfada hiçbir ürün, fiyat veya değer önerisi (kargo, iade) görünmüyor. Üst şerit boş kaldı. Mobilde header çakışması gözlendi. Yoğun bot koruması meşru otomasyonları bile engelliyor.

## KPT için çıkarımlar
- **Uygula:**
  - Ana sayfada hero'nun hemen altına **3 departman kutusu** koy: "ERKEK", "KADIN", "ÇOCUK". 16:9 fotoğraf, ortada beyaz 28–30px büyük harf etiket, alt yarıda `linear-gradient(transparent, rgba(0,0,0,.35))`, kutunun tamamı tıklanabilir, aralık 24px. KPT'nin eksik Erkek/Kadın/Çocuk menüsü sorununu doğrudan çözer.
  - Her departman altında 4 kategori kutusu (3:4): "YENİ GELENLER / SNEAKER / GİYİM / TERLİK-MONT". Etiket 15px Manrope 600, büyük harf.
  - Header ikonlarını 44×44 dokunma alanı ve 24px çizgi ikonla yap, `aria-label="Sepet, 2 ürün"` gibi sayaçlı etiket kullan.
  - Masaüstünde 24px kenar ve 24px sütun aralıklı 12 sütunluk ızgara kur.
- **Uyarla:**
  - Farfetch'in sıfır radius ve tek renk sertliği lüks segmente uygun. KPT'de bordo `#741E32` vurgusunu yalnızca birincil CTA'da kullan, butonlarda 0–4px radius ile premium hissi koru.
  - Bülten başlığını "Hiçbir drop'u kaçırma" gibi yaz, "stok bildirimleri" vaadini ekle.
  - Footer'ı 4 gruba ayır: Müşteri Hizmetleri / KPT Hakkında / İndirimler ve Üyelik / İçerik.
- **Kaçın:**
  - Ana sayfanın ilk ekranında kargo, iade ve taksit bilgisini hiç göstermemek. KPT üst şeridinde mutlaka "500 TL üzeri ücretsiz kargo · 14 gün ücretsiz iade · 9 taksit" gibi metin olsun (rakamlar KPT politikasına göre).
  - Boş bırakılan duyuru şeridi.
  - Mobilde header öğelerinin çakışması: 390px'te logo ve buton için sabit genişlik ayır.

İlgili desenler: [[Header ve Navigasyon]], [[Hero ve Banner Desenleri]], [[Footer]], [[Renk ve Tipografi]], [[Güven Sinyalleri]], [[Mobil Deneyim]], [[KPT Store Denetimi]].

## Ekran görüntüleri
![[farfetch-ana-sayfa-masaustu.jpg]]
*Masaüstü 1440px: 30px gri şerit, sticky header (sol 3 departman linki, ortada logo, sağda 4 ikon ve alt çizgili arama), "Choose a department" ve 3 adet 16:9 departman kutusu.*

![[farfetch-bulten-footer.jpg]]
*Bülten bloğu (`#222222` "Sign Up", 0 radius) ve 4 sütunlu `#E6E6E6` footer.*

## Kaynaklar
- Gözlem: https://www.farfetch.com/ (2026-10-04, masaüstü 1440×900 ve mobil 390×844)
- Farfetch UK Returns and refunds: https://www.farfetch.com/uk/returns-and-refunds
- Wikipedia, "Farfetch" (erişim 2026-10-04): https://en.wikipedia.org/wiki/Farfetch
