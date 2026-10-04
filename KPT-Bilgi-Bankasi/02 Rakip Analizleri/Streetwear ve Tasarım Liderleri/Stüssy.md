---
tür: rakip-analizi
site: Stüssy
url: https://www.stussy.com/
ülke: US
segment: streetwear marka DTC (kült marka)
erişim: tam
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.stussy.com/, https://www.stussy.com/collections/new-arrivals, https://www.stussy.com/products/115855-midweight-puffer-black, https://www.stussy.com/blogs/chapters]
etiketler: [rakip, streetwear, tasarim-lideri, minimalizm]
---

# Stüssy

> [!summary] Özet
> 1980'den beri "California sportswear" satan kült streetwear markası (meta açıklama: "California sportswear, worldwide since 1980"). En güçlü 3 yanı: (1) ana sayfada **beyaz zeminde ortalanmış tek bir siyah-beyaz portre**; başlık yok, CTA yok, kaydırma yok; (2) tüm sitede **tek font, tek boyut (10px), tek ağırlık (500), tamamen büyük harf** ile "katalog / arşiv" hissi; (3) el yazısı logonun tek grafik öğe olduğu, ikon yerine kelime kullanan ("SEARCH", "BAG", "MENU") arayüz. KPT için ders: marka karakteri olan **tek bir imza öğe** (Stüssy'de el yazısı logo) + son derece disiplinli tipografi, renk kullanmadan premium ve ayırt edici bir görünüm üretiyor.

## Kimlik ve konumlandırma
- Meta: "Authentic Stüssy goods. Made tough for the world. Quality guaranteed. Built for the long haul."
- Marka anlatımı ürün dışı içerikte: "ARCHIVE", "NEWS", "STORES", "CHAPTERS" (dünyadaki Chapter mağazalarının fotoğraflı dizini).

## Görsel dil

### Renk paleti
| Rol | Hex | Kullanım yeri |
|---|---|---|
| Metin, CTA zemini | #000000 | Tüm metin, "ADD TO BAG" butonu |
| Zemin | #FFFFFF | Tüm sayfalar |
| İkincil / pasif | #757575 | Renk adı ("BLACK"), stokta olmayan bedenler (PLP'de 93 öğe) |
| Renk küçük görseli zemini | #FBFAF8 | PDP renk seçici kutuları |
| Seçili küçük görsel çerçevesi | #C6C6C6 (1px) | PDP renk seçici |
| Ürün fotoğraf zemini | ~#FAF9F6 (fotoğraftan ölçüldü, #F9F8F4–#FBFAF8 aralığı) | PLP stüdyo ürün fotoğrafları |
| Ayırıcı | #E5E5E5 | Minimal kullanım |

**Az renkle premium:** Arayüzde siyah ve beyaz dışında renk yok; ürün fotoğraf zemini saf beyaz değil **sıcak kırık beyaz** olduğu için ürünler kâğıt üstünde katalog gibi duruyor. Bu ton KPT'nin mevcut #F3F4F1 zeminine çok yakın.

### Tipografi
- **Aile:** HelveticaNeue (sitedeki 576 metin öğesinin tamamı).
- **Boyut:** Masaüstünde **yalnızca 10px**, satır yüksekliği 14px (1.4). Mobilde her şey **12px**, satır 16.8px. Hiyerarşi boyutla değil **konum, boşluk ve gri (#757575)** ile kuruluyor; H1 (ürün adı) bile 10px.
- **Ağırlık:** 500 (tek istisna "Skip to content" 400).
- **Büyük harf:** Her şey uppercase (navigasyon, ürün adı, fiyat, buton, yasal metin).
- **Harf aralığı:** normal (0).
- Logo: el yazısı "Stüssy" imzası, sol üstte ~120x85px; sitedeki tek grafik/ifade öğesi.

### Fotoğraf stili
- Ana sayfa: siyah-beyaz, yakın plan portre (yaşlı bir adam, güneş gözlüğü, leopar desenli gömlek), doğal ışık, belgesel tadında.
- PLP: düz yatırılmış (flat lay) ürün, sıcak kırık beyaz zemin, 4:5 oran, ürün kadrajın ~%85'i.
- PDP ilk kare: açık gri duvar + beton zemin önünde ayakta tam boy model (stüdyo), sonra arkadan model ve ürün kareleri.
- Izgaraya serpiştirilmiş editoryal kare: PLP'de 2 sütun genişliğinde yaşam tarzı fotoğrafı (beton zeminde model).

### Boşluk ritmi ve hareket
- Sol navigasyon sütunu 180px; içerik x=180'den başlar. Menü satırları 20px aralıklı.
- PLP kart sütun aralığı 5px; satırlar arası ~55px (ad+fiyat bloğunun altında geniş nefes).
- Geçiş: `all 0.25s cubic-bezier(0.215, 0.61, 0.355, 1)` (easeOutCubic), `opacity 0.25s`. Hareket neredeyse yok; sitenin "sakin" algısının bir parçası.

## Header ve navigasyon
- Masaüstü: header 54px, sabit, şeffaf. **Kalıcı sol dikey menü** (sayfa kaydıkça yerinde kalır): NEW ARRIVALS, TEES, OUTERWEAR, HEADWEAR, KNITS, SWIMWEAR, TOPS & SHIRTS, BOTTOMS, DENIM, SWEATS, SUNGLASSES, ACCESSORIES, "—" ayırıcı, ARCHIVE, CHAPTERS, SUPPORT, ACCOUNT, NEWSLETTER, LEGAL, US / $. Sol altta "© 2026 STÜSSY". Aktif sayfa altı çizili.
- Alt menüler (DOM'da): TEES > Graphics, Basics; HEADWEAR > Caps, Beanies, Buckets, New Era; DENIM > Big Ol', Classics, Slim, Jackets; SWEATS > Hoodies, Zip-ups, Crews, Sweatpants, Basics.
- Üst orta duyuru: **"FREE STANDARD SHIPPING IN US ON ORDERS OVER $200 USD - HIDE"** ("HIDE" ile kapatılabilir; PDP'de kaydırınca gizleniyor).
- Sağ üst: ikon yok, kelime: **"SEARCH"**, **"BAG"**. Mobil: "SEARCH  BAG  MENU" (12px).

## Ana sayfa ve banner/hero örnekleri

![[stussy-home-desktop.jpg]]
*Masaüstü ana sayfa: beyaz alanda ortalanmış tek siyah-beyaz portre, solda dikey menü.*

**Hero (sayfanın tamamı):**
- **Görsel türü:** Tek fotoğraf (`<picture>`), siyah-beyaz portre, statik (slayt yok; 6 ekran görüntüsünde değişmedi).
- **Kırpma/oran:** **3:4 dikey**, masaüstünde 426x568px, yatayda tam ortada (x=507), üstten 166px. Görselin etrafında her yönde ~170–500px beyaz boşluk; viewport'un yalnızca ~%19'unu kaplıyor. Mobilde 259x345px, y=249.
- **Başlık / alt metin / CTA:** **Yok.** Görselin üstünde veya altında hiçbir metin yok.
- **Metin-görsel ilişkisi:** Metin (menü) solda, görsel ortada; birbirine hiç değmiyor. "Galeri duvarına asılı tek fotoğraf" kurgusu.
- Sayfa yüksekliği 900px: kaydırılacak başka bölüm yok.

![[stussy-home-mobile.jpg]]
*Mobil ana sayfa: logo, üç kelimelik header ve ortada tek portre.*

> [!example] KPT için çeviri
> "Sakin, atölye" estetiği için: ana sayfa ilk ekranında #F3F4F1 zeminde ortalanmış tek bir 3:4 ürün/atölye fotoğrafı (ör. eldeki tek bir New Balance 990, siyah-beyaz), başlık yok; ürünler bir sonraki ekranda başlar. Stüssy'nin aksine KPT'de altına küçük tek satır (12px uppercase) "YENİ GELENLER →" eklenmeli, çünkü KPT'nin marka bilinirliği yok.

**Editoryal sayfa – Chapters (`/blogs/chapters`):** başlık yerine altı çizili "CHAPTER DIRECTORY" linki; mağaza fotoğrafları 840x560px (**3:2**) alt alta, her birinin altında tek satır 10px uppercase: **"STÜSSY TORONTO     241 SPADINA AVENUE #100A TORONTO, ON M5T 3A8, CANADA"**. Ardından ~30 mağazalık metin dizini ("INDEX"). Ticaret yok; tamamen marka dünyası.

## Kategori sayfası (PLP)

![[stussy-plp-desktop.jpg]]
*New Arrivals: 4 sütun, kırık beyaz zeminli 4:5 ürün fotoğrafları ve 2 sütun genişliğinde editoryal kare.*

- Izgara: 4 sütun x 297px, aralık 5px, içerik x=180–1383. Görsel 297x371 (4:5). Mobil 2 sütun.
- Kart anatomisi: görsel → ~17px boşluk → **ad** (10px/500 uppercase) → varsa **"3 COLORS"** → **fiyat**. Swatch, rozet, kaydet ikonu yok. Her kartın DOM'unda beden linkleri var (XS–XXL; stokta olmayanlar #757575); görünür değil, hover'da gösterildiği tahmin ediliyor (tahmin).
- Izgarada editoryal kare: ~559px genişliğinde (2 sütun) yaşam tarzı fotoğrafı ürünlerin arasına yerleştirilmiş.
- Kontroller: içerik başında "VIEW ALL" ve "FILTER" (yalnızca kelime). Sayfa uzun (16.282px), 362 görsel, 341'i lazy.

## Ürün sayfası (PDP)

![[stussy-pdp-desktop.jpg]]
*PDP: 648x810 görseller alt alta, sağda 325px yapışkan bilgi sütunu.*

- Galeri: 648x810px (**4:5**) 6 görsel alt alta (x=180), her biri tıklanınca zoom ("Zoom into image 1 of 6").
- Bilgi sütunu (x=878, 325px, kaydırınca yapışkan): "MIDWEIGHT PUFFER" / "$225" / "BLACK" (#757575) / beden harfleri düz metin olarak yan yana "XS S M L XL XXL" / 4 renk küçük görseli (45x55, #FBFAF8 zemin) / **"ADD TO BAG"** (325x35px, #000000, beyaz 10px/500 uppercase, radius 0) / "PRODUCT DETAILS >", "SIZE GUIDE >", "SHIPPING & RETURNS >", "CHAT" / "FREE STANDARD SHIPPING IN US FOR ORDERS OVER $200 USD. EXCLUSIONS APPLY."
- **Doğrulama geri bildirimi:** beden seçmeden butona basınca buton metni **"SELECT A SIZE"** oluyor (ayrı hata mesajı yok). Stoksuz beden için "NOTIFY ME WHEN AVAILABLE" mevcut.
- Mobil: görsel tam genişlik, altında aynı blok; **yapışkan sepet çubuğu yok**.

## Sepet ve satın alma kolaylığı
incelenemedi: beden etiketine otomasyonla tıklanamadı, sepete ekleme tamamlanmadı; bütçe kısıtı nedeniyle tekrar denenmedi.

## Mobil deneyim
Tüm metin 12px'e çıkıyor (masaüstünden büyük); header "SEARCH / BAG / MENU" kelimeleri; PLP 2 sütun; PDP'de sabit CTA yok; footer'da "NEWSLETTER *" satırı ve ok.

## Güven ve ikna unsurları
| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| Kargo eşiği duyurusu (kapatılabilir) | Üst orta | Hedef gradyanı | Evet, "Gizle" seçeneğiyle |
| "Authentic Stüssy goods… Quality guaranteed" | Meta/marka dili | Orijinallik güvencesi | Evet: "%100 orijinal" |
| Chapter mağaza dizini | Editoryal | Fiziksel varlık = güven | KPT mağazası/atölyesi varsa |
| Buton metninin "SELECT A SIZE"e dönmesi | PDP | Hata önleme | Evet |

## Performans ve teknik gözlem
Shopify. Ana sayfa 236 istek / 2,5 MB, DOMContentLoaded 2,1 sn; PLP 5,7 MB. `--header-height: 81px` CSS değişkeni.

## Güçlü yanlar / Zayıf yanlar
- **Güçlü:** Kopyalanamaz derecede tutarlı tipografi; tek görselli ana sayfa; kelime tabanlı ikon dili; sıcak kırık beyaz fotoğraf zemini; ızgara içi editoryal kare.
- **Zayıf:** 10px metin ve tamamen büyük harf okunabilirliği düşürüyor; PDP'de güven/iade bilgisi linklerin arkasında; mobilde yapışkan CTA yok; ana sayfa ürün keşfi sunmuyor.

## KPT için çıkarımlar
- **Uygula:** Ürün fotoğraf zeminini sıcak kırık beyaz (~#FAF9F6 / KPT'de #F3F4F1) olarak sabitle; PLP ızgarasına her 8–12 üründe bir 2 sütunluk atölye/yaşam tarzı karesi ekle; beden seçilmeden CTA'ya basılınca buton metnini "BEDEN SEÇİN" yap.
- **Uyarla:** Tek imza öğe fikri: KPT'nin Archivo Black logosu yerine (veya yanına) el işi / damga hissi veren tek bir grafik öğe; header ikonlarını kelimeyle değiştir ("ARA", "SEPET (2)") ve uppercase etiketlerde 11–12px Manrope 500 kullan.
- **Kaçın:** 10px metin; tamamen başlıksız ana sayfa (KPT için ürün keşfi şart); mobilde sabit sepete ekle çubuğunun olmaması.

İlgili: [[Hero ve Banner Desenleri]], [[Renk ve Tipografi]], [[Header ve Navigasyon]], [[Kategori Sayfası ve Filtreler]], [[Ürün Sayfası]], [[Görsel Tasarım ve Trendler 2026]], [[KPT Store Denetimi]]

## Ekran görüntüleri
Gömülü: `stussy-home-desktop.jpg`, `stussy-home-mobile.jpg`, `stussy-plp-desktop.jpg`, `stussy-pdp-desktop.jpg`.

## Kaynaklar
- https://www.stussy.com/ (2026-10-04 gözlem)
- https://www.stussy.com/collections/new-arrivals (2026-10-04 gözlem)
- https://www.stussy.com/products/115855-midweight-puffer-black (2026-10-04 gözlem)
- https://www.stussy.com/blogs/chapters (2026-10-04 gözlem)
