---
tür: rakip-analizi
site: Nike Türkiye
url: https://www.nike.com/tr/
ülke: TR
segment: marka DTC (global platform, TR yerelleştirmesi)
erişim: kısmi
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.nike.com/tr/, https://www.nike.com/tr/w/erkek-ayakkabilar-nik1zy7ok, https://www.nike.com/tr/t/air-force-1-07-lv8-erkek-ayakkabisi-K3OuKghd/IW3476-001, https://www.nike.com/tr/cart]
etiketler: [rakip, marka-dtc, sneaker, nike]
---

# Nike Türkiye

> [!summary] Özet
> Nike'ın global "nike.com" platformunun Türkçe yerelleştirmesi; her yaştan sporcuya ve sneaker tüketicisine doğrudan satış yapıyor. En güçlü 3 yanı: (1) 5 sütunlu, tamamen metin tabanlı ve çok net bir mega menü (Öne Çıkanlar / Ayakkabılar / Giysiler / Spor / Markalar), (2) PLP'de solda sabit, 3'lü beden ızgarası + renk daireleri olan çoklu seçimli filtre paneli ve kartta renk varyant küçük resimleri, (3) PDP'de stoktaki/stokta olmayan tüm EU bedenlerini 3 sütunlu kutu ızgarada gösteren beden seçici ve mobilde ekranın altına sabitlenmiş tam genişlik "Sepete Ekle" çubuğu. KPT için en değerli ders: **ürün adı + alt satırda "hedef kitle + ürün türü" (örn. "Nike Air Force 1 '07 LV8" / "Erkek Ayakkabısı")** formatı ve kısa açıklama + 3 maddelik künye (Gösterilen Renk / Stil kodu / Menşe) yapısı, KPT'nin boş açıklama sorununa doğrudan uygulanabilir bir standart.

> [!warning] Erişim notu
> Sayfalar açıldı (HTTP 200) ancak: (1) test ortamının çıkış IP'si ABD'de olduğundan her sayfada "We think you are in United States. Update your location?" konum penceresi çıktı; (2) hero videoları headless Chromium'da codec eksikliğinden oynamadı ("Sorry, your browser doesn't support embedded videos."), bu gerçek kullanıcı deneyimi değildir; (3) **Sepete ekleme isteği `api.nike.com/buy/carts/v2/TR/...` adresinden HTTP 403 döndü** (bot koruması); ekranda "Hata / Talebinle ilgili bir sorun yaşadık..." modalı göründü. Kurallar gereği aşılmaya çalışılmadı; sepet doluyken deneyim **incelenemedi**, yalnızca boş sepet ekranı görüldü.

## Kimlik ve konumlandırma

- **Kim:** Nike Inc.'in resmi Türkiye mağazası (`/tr/` alt yolu, `lang="tr-TR"`). Sayfa başlığı: "Nike. Just Do It. Nike TR". Meta açıklama: "Nike, sporculara ilham vermek için yenilikçi ürünler, deneyimler ve hizmetler sunar."
- **Kime:** Erkek, Kadın, Çocuk; spor dalına göre (Koşu, Futbol, Basketbol, Antrenman, Tenis, Kaykay, Golf) ve "sokak giyimi" kullanıcısına. Alt markalar: Jordan, ACG, NOCTA, Kobe, NikeSKIMS.
- **Türkiye bağlamı:** Nike, Ağustos 2024'te gümrük düzenlemesi (yurt dışı ekspres kargo limitinin 30 €'ya düşürülmesi) gerekçesiyle Türkiye'den online siparişi durdurmuştu (Medyascope, 2024; Just Style, 2024). İnceleme tarihinde sitenin üst şeridinde "En sevdiğin Nike ürünlerini Nike.com ve Nike App'ten sipariş edebilirsin." yazıyor, yani satış yeniden açık. Yardım sayfasına göre siparişler **uluslararası gönderiliyor ve gümrükten geçiyor; vergiler ödeme tutarına dahil** (nike.com/tr Kargo yardım sayfası, 2026). Bu, yerel stokla satan KPT için bir **avantaj alanı**: hızlı yerel teslimat ve taksit vurgusu Nike'ın kendi sitesinde yok.
- **Ton:** Sen diliyle, kısa ve motivasyonel ("BU YARIŞ SENİN YARIŞIN", "Kabına Sığmaz"). Ürün dili teknik değil, fayda odaklı.

## Görsel dil

### Renk paleti (hesaplanmış stillerden)

| Rol | Hex | Kullanım yeri |
|---|---|---|
| Ana metin / birincil buton | `#111111` | Başlıklar, fiyat, "Sepete Ekle" dolgusu, nav linkleri |
| İkincil metin | `#707072` | Ürün alt başlığı ("Erkek Ayakkabısı"), footer linkleri, mega menü alt linkleri |
| Zemin | `#FFFFFF` | Sayfa zemini |
| Açık gri yüzey | `#F5F5F5` | Üst yardımcı şerit, duyuru şeridi, arama kutusu, ürün görseli zemini |
| Ayraç | `#E5E5E5` | Akordeon ve bölüm çizgileri |
| Vurgu (rozet) | `#D33918` | PLP kart rozeti: "Yeni Satışa Sunuldu", "En Çok Satan", "Yakında Satışa Sunuluyor", "Tükendi" |
| Ters metin | `#FFFFFF` | Hero başlıkları, siyah buton metni |

Tek renkli (siyah-beyaz-gri) sistem; tek renkli vurgu yalnızca turuncu-kırmızı rozet metninde. Renk tamamen ürün fotoğrafından geliyor.

### Tipografi

- **Aileler:** "Helvetica Now Text Medium" (gövde, butonlar, linkler; ağırlık 500 baskın), "Helvetica Now Text" (400; açıklama metni), "Helvetica Now Display Medium" (PDP başlıkları), **"Nike Futura ND"** (hero başlıkları; sıkışık, ağır, büyük harf).
- **Boyutlar:** Hero başlığı masaüstünde **76px**, mobilde **40px** (Futura ND, büyük harf). Bölüm başlığı "İKONLARIMIZI İNCELE" aynı ailede ~76px. Kart başlığı/fiyat **16px/500**. Alt başlık 16px/400 `#707072`. Mega menü ana başlıkları ~14px/500 `#111111`, alt linkler 12px/500 `#707072`. Üst duyuru şeridi **12px/400**. Footer linkleri 12–14px/500.
- Harf aralığı normal; büyük harf yalnızca hero ve bölüm başlıklarında (metin zaten büyük harfle yazılmış, `text-transform` yok).

### Şekil, boşluk, hareket

- **Radius:** butonlar ve arama kutusu **30px** (tam hap şekli); PLP/PDP ürün görselleri ~**20px** (PDP ana görselde belirgin yuvarlak köşe); filtre beden kutuları 3–4px; renk örnekleri daire (%50).
- **Butonlar:** Hero CTA beyaz dolgu, `#111111` metin, **76×36px**, 16px/500, radius 30px ("İncele"). PDP "Sepete Ekle" **376×60px**, siyah dolgu, beyaz metin, radius 30px; altında "Favori" aynı ölçüde, beyaz zemin + 1px gri çerçeve + kalp ikonu.
- **İkonlar:** ince çizgili (1.5px) monokrom: büyüteç, kalp, çanta; mobilde kişi ve hamburger.
- **Hareket:** hero otomatik dönen 2 slaytlı carousel, "Döngüyü duraklat" butonu ve 5px nokta göstergeleri var; mega menü hover ile açılıyor.

## Header ve navigasyon

- **Yardımcı şerit (36px, `#F5F5F5`):** solda Jordan logosu; sağda "Mağaza Bul | Yardım | Bize Katıl | Oturum Aç" (12px/500, dikey çizgi ayraçlı).
- **Ana header (60px, beyaz):** solda Nike swoosh; ortada **"Yeni · Erkek · Kadın · Çocuk · Spor · NikeSKIMS"** (16px/500); sağda gri dolgu hap arama kutusu "Ara" (~168×36px, `#F5F5F5`, radius 30px), favori kalp ve sepet çantası ikonları (36×36 dokunma alanı).
- **Duyuru şeridi (58px, `#F5F5F5`):** ortalanmış tek satır: "En sevdiğin Nike ürünlerini Nike.com ve Nike App'ten sipariş edebilirsin." (12px). Kampanya/kargo mesajı yok.
- **Sticky:** aşağı kaydırıldığında yardımcı şerit ve duyuru şeridi kayboluyor, yalnızca 60px ana header üstte kalıyor.
- **Mega menü ("Erkek" hover):** tam genişlik beyaz panel, 5 sütun, görsel yok, yalnızca metin:
  - **Öne Çıkanlar:** Yeni Ürünler, En Çok Satan Ürünler, Sokak Giyimi, Futbol: Yeni Kulüp Formaları 26/27, Temel Giyim Ürünleri
  - **Ayakkabılar:** Tüm Ayakkabılar, Günlük Giyim, Jordan, Koşu, Futbol, Basketbol, Antrenman ve Spor Salonu, Kaykay, Kişiye Özel Ayakkabılar
  - **Giysiler:** Tüm Giyim, Kapüşonlu Üstler ve Sweatshirt'ler, Üstler ve Tişörtler, Takımlar ve Formalar, Şortlar, Eşofman Altları ve Taytlar, Eşofmanlar, Ceketler, Aksesuarlar
  - **Spor:** Koşu, Futbol, Basketbol, Antrenman ve Spor Salonu, Tenis, Kaykay, Golf
  - **Markalar:** Nike Sportswear, ACG: All Conditions Gear, Jordan, Kobe, NOCTA
  - Aktif menü öğesinin altında 2px siyah alt çizgi. Panel açıkken sayfa içeriği karartılmıyor.
- **Hedef kitle kurgusu:** Erkek / Kadın / Çocuk birinci seviye; her birinin içinde **aynı 5 sütunlu şablon** tekrar ediyor (kategori → ürün türü → spor → marka). Kullanıcı önce kimin için aldığını, sonra ne aldığını seçiyor.
- **Mobil menü:** sağdan kayan tam yükseklik çekmece (sol ~70px'te sayfa görünür kalıyor). Büyük (~22px) satırlar: "Yeni / Erkek / Kadın / Çocuk / Spor / NikeSKIMS", her birinde sağda `>` ok (alt seviye ekrana kayarak açılıyor). Altında Jordan logolu link, üyelik çağrısı: "Nike'ın en iyi ürünlerine, ilham verici içeriklere ve spor hakkında hikayelere erişmek için Nike Üyesi ol. Daha fazla bilgi edin" + "Bize Katıl" (siyah) ve "Oturum Aç" (çerçeveli) hap butonlar; en altta Yardım, Sepet, Siparişler, Mağaza Bul ikonlu linkler.

## Ana sayfa ve banner/hero örnekleri

Bölüm sırası (yukarıdan aşağı, masaüstü sayfa yüksekliği 4.396px):

1. **Hero carousel (tam genişlik, 1440×700px, mobil 390×585px), 2 slayt, video:**
   - Slayt A: üst etiket "After Dark Tour Koleksiyonu" (16px), başlık **"BU YARIŞ SENİN YARIŞIN"** (Futura ND, iki satır, beyaz, ortalı), CTA beyaz hap **"İncele"**.
   - Slayt B: başlık **"EVERY. DAY. SPEED."**, alt metin "O Pazar günü hızlı olmak istiyorsan Salı antrenmanlarını hızlandır. Pegasus Plus 2 şimdi satışta.", CTA **"İncele"**.
   - Metin bloğu dikeyde alt-orta (başlık ~y590, CTA ~y740). Sol/sağ ok yok; 5px beyaz noktalar + duraklat butonu.
2. **2'li bölünmüş banner ızgarası (2 × ~666×600px, 12px aralık, kenar boşluğu 48px):** sol alt köşede küçük üst etiket (16px/500 beyaz) + başlık (~24px beyaz) + 1–2 beyaz hap CTA.
   - "Renkli Stiller" / **"Renk Paletini Değiştir"** / CTA'lar: **"Erkek Ürünlerini İncele"** + **"Kadın Ürünlerini İncele"** (cinsiyete göre ikili CTA deseni).
   - "Nike Basketball" / **"Caitlin 1 Özel Koleksiyonu"** / **"İncele"** + **"Daha Fazla Bilgi"**.
3. **İkinci 2'li ızgara (~666×400px):** "ACG Lava Flow Ultralight" / **"Dondurucu Soğuğa Karşı Lav Sıcaklığı"** / "İncele"; "Erling Haaland Phantom 6" / **"Kabına Sığmaz"** / "İncele".
4. **Tam genişlik bölünmüş editoryal banner (2 fotoğraf yan yana, kenar boşluksuz):** üst etiket "Nike Zoom Skylon 11", dev başlık **"MESAFELER GERİDE, GÜNLÜK HAYATIN İÇİNDE"** (Futura ND), CTA **"Keşfet"**.
5. **"İKONLARIMIZI İNCELE"** (Futura ND ~76px ortalı): 8 sütunlu ızgarada 16 ikon model, her biri şeffaf zeminli ~80px ürün kesiti + 12px etiket: Air Jordan 1, Air Max, Grafik Baskılı Tişört, Dunk, Air Force 1, 24.7 Koleksiyonu, ACG, Pegasus, Vomero Plus, Metcon, Taraftar Ekipmanları, Jordan Retro, Sabrina 4, Tatum 4, Mercurial Superfly, P6000. Mobilde yatay kaydırma + "Tümünü Gör".
6. **SEO link bloğu (4 sütun):** "Ayakkabılar / Giysiler / Çocuk / Öne Çıkanlar" başlıkları (20px/500) altında 4'er uzun kuyruk link ("Siyah Koşu Ayakkabıları", "Erkek Çocuk Okul Ayakkabıları" vb.), uzun metin "…" ile kesiliyor.
7. **Footer:** 3 sütun "Kaynaklar / Yardım / Şirket" + sağda dünya ikonu "Türkiye". Yardım sütunu: Yardım Al, Sipariş Durumu, Kargo ve Teslimat, İadeler, Ödeme Seçenekleri, Bize Ulaş, İncelemeler. Alt satır: "© 2026 Nike, Inc. Tüm Hakları Saklıdır." + Kullanım Şartları, Satış Şartları, Bilgi Toplumu Hizmetleri, Gizlilik ve Tanımlama Bilgisi Politikası, Gizlilik ve çerez ayarları. **Ödeme logosu, güven rozeti, e-bülten formu yok.**

Ana sayfada **ürün kartı ızgarası yok**; tamamen editoryal banner + ikon model navigasyonu.

## Kategori sayfası (PLP)

İncelenen: "Erkek Ayakkabıları (636)".

- **Başlık satırı:** solda H1 "Erkek Ayakkabıları" + gri olmayan "(636)" sonuç sayısı (~24px/500); sağda **"Filtreleri Gizle"** + ayar ikonu (filtre panelini açıp kapatıyor, ızgara 3'ten 4 sütuna genişliyor) ve **"Sıralama Ölçütü ⌄"** açılır menü.
- **Sol panel (240px, kendi içinde kaydırılan, sticky):**
  1. Alt kategori linkleri (16px/500): Sandaletler ve Terlikler, Günlük Giyim, Jordan, Koşu, Basketbol, Futbol, Antrenman ve Spor Salonu, Kaykay, Golf, Tenis, Yürüyüş, Nike By You.
  2. Akordeon filtreler (her biri 48px yükseklik, 1px `#E5E5E5` üst çizgi, sağda chevron): **Cinsiyet (1)** (seçili sayısı parantezde), Fiyata Göre İncele, İndirimler ve Fırsatlar, **Numara/Beden**, **Renk**, Custom, Ayakkabı Yüksekliği, Koleksiyonlar, Spor, Marka.
  - **Numara/Beden ızgarası:** 3 sütun, her kutu ~57×36px, 1px açık gri çerçeve, 4px radius, ortalı 16px rakam. Değerler: 35.5, 36, 36.5, 37.5, 38, 38.5, 39, 40, 40.5, 41, 42, 42.5, 43, 44, 44.5, 45, 45.5, 46, 47, 47.5, 48, 48.5, 49.5, 50.5, 51.5, 52.5 (yarım numaralar dahil, "EU" öneki yok). Son satırda 2 kutu genişleyerek satırı dolduruyor.
  - **Renk:** 3 sütun, ~28px dolu renk dairesi + altında 12px etiket: Siyah, Mavi, Kahverengi, Yeşil, Gri, Multi-Color (desenli daire), Turuncu, Pembe, Mor, Kırmızı, Beyaz (ince gri çerçeveli), Sarı. Tedarikçi renk adları değil, **12 normalize ana renk** kullanılıyor.
  - Filtreler anında uygulanıyor (buton yok), çoklu seçim.
- **Mobil filtre:** başlık altında yatay kaydırmalı alt kategori sekmeleri; altında yatay kaydırmalı **hap çipler** (36px yükseklik, 1px gri çerçeve, radius 30px): "⚙ (1)" (tüm filtreler), "Cinsiyet (1) ⌄", "Fiyata Göre İncele ⌄", "İndirimler ve Fırsatlar", "Numara/Beden", "Renk". Çip satırı kaydırmada başlıkla birlikte üstte sabit kalıyor.
- **Ürün kartı anatomisi (masaüstü 3 sütun, kart 348px, 16px aralık):**
  1. Kare (1:1) görsel, `#F5F5F5` zemin üzerinde stüdyo çekimi yan profil, köşe radius yok/çok az.
  2. **Renk varyant şeridi:** görselin hemen altında 48×48px küçük resimler (6'ya kadar), hover ile ana görsel değişiyor. Masaüstünde görünür; mobilde 2 sütunda yatay kaydırılabilir şerit.
  3. Rozet satırı: **"Yeni Satışa Sunuldu" / "En Çok Satan" / "Yakında Satışa Sunuluyor" / "Tükendi" / "Geri Dönüştürülmüş Malzemeler"** — 16px/500, `#D33918`, arka plansız düz metin.
  4. Ürün adı 16px/500 `#111111` ("Nike Metcon 10").
  5. Hedef kitle + tür 16px/400 `#707072` ("Erkek Antrenman Ayakkabısı").
  6. Fiyat 16px/500: **"8.699₺"** (binlik ayırıcı nokta, kuruşsuz, ₺ boşluksuz sonda). İndirimde yeni fiyat + üstü çizili eski fiyat (sepette "current price 5.099,00₺, original price 7.199,00₺" erişilebilirlik etiketiyle görüldü).
  - Kartta "sepete ekle" veya favori ikonu yok.
- **Mobil ızgara:** 2 sütun, ~192px kart, ~6px aralık, metin 14px.
- **Sayfalama:** sonsuz kaydırma (masaüstü sayfa yüksekliği 15.000px+, 169 görsel, 157'si lazy).
- **SEO:** sayfa sonunda "İlgili Kategoriler" link bulutu ("En İyi Erkek Ayakkabıları", "Erkek Siyah Koşu Ayakkabıları", "Halı Saha Kramponları"…).
- Sıralama menüsü test sırasında açılmadı; seçenekler **incelenemedi**.

## Ürün sayfası (PDP)

İncelenen: Nike Air Force 1 '07 LV8 Erkek Ayakkabısı, Stil IW3476-001, 7.799₺.

- **Düzen (masaüstü):** ortalanmış ~1016px blok: solda dikey küçük resim şeridi (9 × 60×60px, 8px radius, 8px aralık), ortada ana görsel ~532×665px (4:5 dikey, `#F5F5F5` zemin, ~20px radius, sağ altta beyaz daire ok butonları ‹ ›), sağda 376px bilgi sütunu. Bilgi sütunu sabit (sticky) değil.
- **Galeri:** **9 görsel** ("görsel 1 / 9"): yan profil, taban, iç yan, üstten çift, 3/4, arkadan çift, 3 detay yakın çekim (dikiş, topuk, burun). Hover ile küçük resim değişimi. Video/360 yok.
- **Başlık yapısı (KPT için şablon):**
  - H1: **"Nike Air Force 1 '07 LV8"** (~24px/500, `#111111`)
  - H2: **"Erkek Ayakkabısı"** (16px/400, `#707072`)
  - Fiyat: **"7.799₺"** (16px/500)
  - Sayfa `<title>`: "Nike Air Force 1 '07 LV8 Erkek Ayakkabısı. Nike TR"
  - URL: `/tr/t/air-force-1-07-lv8-erkek-ayakkabisi-<id>/IW3476-001` (slug + stil kodu)
- **Renk seçimi:** bu üründe tek renk; çok renkli ürünlerde başlık altında renk varyant küçük resimleri gösteriliyor (PLP'deki şeritle aynı mantık).
- **Beden seçici:**
  - Üst satır: solda **"Numara/Beden Seç"** (16px/500), sağda cetvel ikonu + **"Beden/Numara Rehberi"** (14px/500, modal açıyor).
  - **3 sütunlu ızgara, her kutu 118×46px**, 1px açık gri çerçeve, 4px radius, 16px/400 metin, değerler **"EU 36" … "EU 49.5"** (21 beden, yarım numaralar dahil).
  - Seçili beden: 1px **siyah** çerçeve (dolgu yok).
  - Stok dışı: bu üründe 21 bedenin tamamı aktifti; Nike'ın tükenen bedenleri ızgaradan çıkarmayıp gri zemin + soluk metinle pasif gösterdiği **gözlenemedi** (bu üründe yok). Kalıp bilgisi ("dar kalıp, yarım numara büyük al" vb.) PDP'de **yok**.
- **CTA:** "Sepete Ekle" (376×60px, `#111111`, beyaz 16px/500, radius 30px); tıklanınca yükleme sırasında `#707072` griye dönüyor. Altında "Favori ♡" (376×60px, beyaz, gri çerçeve). Beden seçmeden tıklanırsa uyarı davranışı test edilmedi.
- **Promosyon notu:** CTA'nın altında ortalı gri metin: **"Bu ürün site promosyonları ve indirimleri kapsamında değildir."**
- **Açıklama yapısı (KPT için şablon):**
  1. 1 paragraf, 2 cümle, fayda + hikâye: "Rahat, dayanıklı, zamana meydan okuyan bu stilin bir numara olması boşuna değil. Klasik 1980'ler yapısı, deri ve tekstili göz alıcı ayrıntılarla bir araya getirerek hem sahadayken hem de yoğun günlerde giyebileceğin bir stil oluşturur."
  2. Madde listesi (künye): **"Gösterilen Renk: Siyah/Cool Grey/Cool Grey"**, **"Stil: IW3476-001"**, **"Menşe Ülke/Bölge: Vietnam"**.
  3. Altı çizili link "Ürün Ayrıntılarını Görüntüle" (modal; içerik bu oturumda okunamadı).
  4. Akordeonlar (1px çizgi ayraçlı, 22px başlık): **"Kargo ve İadeler"** → "Minimum sipariş toplamına ulaşan siparişlerde ücretsiz kargo. Daha Fazla Bilgi Edin." / "30 gün içinde ücretsiz iade, bazı istisnalar uygulanabilir."; **"Yorumlar (0)"** + 5 boş yıldız; **"Daha Fazla Bilgi"** → "Dana derisi içerir" (malzeme uyarısı).
- **Teslimat/iade/taksit:** CTA yakınında **taksit bilgisi yok**, teslimat tarihi yok; kargo/iade bilgisi akordeonun içinde gizli.
- **Çapraz satış:** sepet sayfasında "Şunları da Beğenebilirsin" carousel'i (10 ürün, ok butonlu); PDP'de alt bölüm bu oturumda görüntülenmedi.

## Sepet ve satın alma kolaylığı

- **Sepete ekleme geri bildirimi:** incelenemedi (cart API 403). Hata durumunda ortalı modal: başlık **"Hata"**, metin **"Talebinle ilgili bir sorun yaşadık. Sorun yaşamaya devam edersen sayfayı yenilemeyi dene."**, siyah hap buton **"Sepeti Görüntüle"**, sağ üstte gri daire kapat. Arka plan %40 karartılıyor. (Hata mesajının bile sen diliyle ve çözüm önerisiyle yazılması örnek alınabilir.)
- **Boş sepet ekranı:** 2 sütun: solda "Sepet" + "Sepetinde ürün yok."; sağda **"Özet"** kutusu: "Ara Toplam ⓘ — / Tahmini Kargo ve İşlem Ücreti — / Toplam —", altında iki hap buton (~335×60px, boşken pasif gri): **"Misafir Kullanıcı Olarak Ödeme"** ve **"Üye Girişi Yaparak Ödeme"**. Misafir ödeme destekleniyor.
- **Fiyat formatı sepette:** "7.499,00₺" (kuruşlu), PLP/PDP'de kuruşsuz.
- **Ödeme yöntemleri (ikincil kaynak):** Visa, MasterCard, TROY; tek siparişte tek yöntem; "Uluslararası işlemler için kartın bankadan etkinleştirilmesi gerekebilir." (nike.com/tr Ödeme Seçenekleri yardım sayfası, 2026). Taksit: ayrı yardım sayfası var ("Nike.com Siparişimi Taksitle Ödeyebilir miyim?"); arama özetine göre taksit seçenekleri **kart bilgisi girildikten sonra ödeme adımında** görünüyor (nike.com/tr yardım, 2026). Sitede hiçbir yerde ödeme logosu gösterilmiyor.
- **Ücretsiz kargo eşiği (ikincil kaynak):** "13.000 ₺ ve üzeri siparişlerde ücretsiz; 13.000 ₺ altındaki siparişlerde 475 ₺"; hızlandırılmış kargo yok; vergiler ve gümrük ödemeye dahil (nike.com/tr Kargo yardım sayfası, 2026). Eşik göstergesi (progress bar) sepet ekranında boşken yok.
- **İade (ikincil kaynak):** 30 gün, iade kargo ücretini Nike karşılıyor, ürün "giyilmemiş, yıkanmamış ve etiketi çıkarılmamış" olmalı (nike.com/tr İade Politikası, 2026).

## Mobil deneyim

- Header 60px: swoosh solda; sağda arama, kişi (Oturum Aç), çanta, hamburger (her biri 36×36). Duyuru şeridi 2 satıra kırılıyor.
- Hero 390×585px (dikey), başlık 40px Futura ND.
- PLP: yatay kaydırmalı alt kategori sekmesi + hap filtre çipleri, 2 sütun.
- **PDP mobil sırası:** başlık + alt başlık + fiyat **görselin üstünde** (kullanıcı ürünü ve fiyatı ilk bakışta görüyor) → tam genişlik kaydırmalı galeri (4:5'e yakın, altta nokta göstergeli) → beden seçici → açıklama → akordeonlar.
- **Sticky ATC:** ekranın altına sabit, **tam genişlik 390×62px siyah çubuk, beyaz "Sepete Ekle"** (radius yok); sayfa boyunca görünür. KPT'nin bilinen eksikliği için doğrudan referans.

## Güven ve ikna unsurları

| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| "En Çok Satan" rozeti | PLP kartı, `#D33918` metin | Sosyal kanıt | Evet: satış verisiyle ilk 10 modele |
| "Yeni Satışa Sunuldu" / "Yakında Satışa Sunuluyor" | PLP kartı | Yenilik, beklenti | Evet: yeni sezon modellerde |
| "Tükendi" rozeti kartta görünür kalıyor | PLP | Kıtlık | Kısmen: tükenen ürünü listede tutmak KPT'de hayal kırıklığı yaratabilir; sona at |
| Cinsiyete göre ikili CTA ("Erkek Ürünlerini İncele" / "Kadın Ürünlerini İncele") | Ana sayfa banner | Seçim mimarisi, yol kısaltma | Evet |
| Üyelik çağrısı ("Nike Üyesi ol") + "Bize Katıl" | Header, mobil menü, footer | Aidiyet, ayrıcalık | Kısmen: KPT'de basit "favori/hesap" ile |
| "30 gün içinde ücretsiz iade" | PDP akordeonu | Risk azaltma | Evet ama **CTA'nın altında görünür** yaz |
| "Sorun yaşamaya devam edersen sayfayı yenilemeyi dene" | Hata modalı | Kontrol hissi, empati | Evet |
| Yorumlar (0) + boş yıldız | PDP | Sosyal kanıt (burada ters etki) | **Kaçın:** yorum yokken "(0)" göstermek güveni düşürür |

## Performans ve teknik gözlem

- Ana sayfa (masaüstü): TTFB 1.113 ms, DOMContentLoaded 2.418 ms, load 4.404 ms, 250+ istek, **4,2 MB** aktarım; 32 görselin 27'si lazy.
- PLP: TTFB 870 ms, load 5.007 ms, **5,8 MB**, 169 görsel (157 lazy).
- Görseller Cloudinary benzeri dönüşüm URL'leriyle (`t_PDP_144_v1/f_auto,q_auto:eco`) otomatik format/kalite; küçük resimler 144px.
- Konum algılama penceresi (IP tabanlı) her sayfada tekrar çıkıyor; kullanıcı "Türkiye" seçince kayboluyor.
- Cart API (`api.nike.com/buy/carts/v2/TR/NIKE/NIKECOM`) otomasyon tarayıcısına 403 dönüyor.

## Güçlü yanlar / Zayıf yanlar

**Güçlü:**
- Kristal netlikte bilgi mimarisi: hedef kitle → ürün türü → spor → alt marka; mega menü tamamen metin, hızlı taranıyor.
- PLP'de 3'lü beden ızgarası + 12 normalize renk dairesi; mobilde hap çipler.
- Kartta renk varyant küçük resimleri; tek bakışta renk seçeneği.
- PDP'de tüm bedenler kutu ızgarada, "EU" önekiyle; mobil sticky ATC.
- Tutarlı ürün adlandırma: "Model adı" + "Kitle + Tür".

**Zayıf:**
- PDP'de taksit, teslimat süresi, ücretsiz kargo eşiği görünmüyor; "Minimum sipariş toplamı" muğlak (gerçek eşik 13.000 ₺ ve yalnızca yardım sayfasında).
- Footer ve sepette ödeme logosu, güven rozeti yok; Türkiye kullanıcısının alıştığı "peşin fiyatına taksit" dili yok.
- Kalıp bilgisi yok; yorumlar boş.
- Sayfalar ağır (4–6 MB).
- Uluslararası gönderim/gümrük nedeniyle teslimat 3–11 iş günü aralığında (ikincil kaynak, eski sürüm sayfası).

## KPT için çıkarımlar

- **Uygula:**
  - Ürün başlığı şablonu: `H1 = Marka + Model + Varyant` ("Nike Air Force 1 '07 LV8"), altında `16px #707072` satır: `Hedef kitle + Ürün türü` ("Erkek Ayakkabısı", "Genç Çocuk Ayakkabısı", "Kadın Koşu Ayakkabısı"). Aynı ikili satırı PLP kartında da kullan.
  - Açıklama şablonu: 2 cümlelik fayda paragrafı + 3 maddelik künye: "Gösterilen Renk: …", "Stil: <tedarikçi stil kodu>", "Menşe Ülke/Bölge: …". KPT'nin boş açıklama sorunu için minimum içerik standardı.
  - PDP beden ızgarası: 3 sütun, 46px yükseklik kutular, "EU 42.5" formatı, seçili = 1px siyah çerçeve; üst satırda sağda "Beden/Numara Rehberi" linki. Stokta olmayanları **gizlemek yerine** pasif göster (KPT'nin mevcut sorunu).
  - PLP filtre: akordeon sırası Cinsiyet → Fiyat → İndirim → Numara → Renk; numara 3'lü ızgara, renk 12 normalize daire + etiket. Seçili sayıyı başlıkta "(1)" ile göster.
  - Mobil PDP'de başlık + fiyatı görselin üstüne koy; alta tam genişlik sabit "Sepete Ekle" çubuğu (62px).
  - Ana sayfa banner'larında cinsiyet ikili CTA: "Erkek Ürünlerini İncele" / "Kadın Ürünlerini İncele".
  - "İkonlarımızı İncele" deseni: şeffaf zeminli ürün kesitleriyle model bazlı navigasyon (KPT: "Samba", "530", "Old Skool", "Air Force 1"…).
- **Uyarla:**
  - Mega menüyü 5 sütun metin olarak kur, ama KPT çok markalı olduğu için "Markalar" sütununu en başa al (New Balance, Nike, adidas, Skechers, Puma, Vans, Columbia).
  - Rozet rengi olarak Nike'ın `#D33918`'i yerine KPT bordo `#741E32` ile düz metin rozet ("Yeni", "Çok Satan").
  - Kargo/iade akordeonu yerine CTA'nın hemen altında 3 satırlık görünür güven bloğu: teslimat süresi, ücretsiz kargo eşiği (somut TL), taksit ("Peşin fiyatına 3 taksit" vb.). Nike'ın bunu yapmaması KPT için farklılaşma fırsatı.
- **Kaçın:**
  - "Yorumlar (0)" ve boş yıldız göstermek.
  - "Minimum sipariş toplamına ulaşan siparişlerde ücretsiz kargo" gibi tutar vermeyen muğlak metin.
  - Hero'da otomatik oynayan ağır video (4 MB+ sayfa); KPT'nin zaten ağır hero sorunu var.

## Ekran görüntüleri

![[nike-mega-menu-hero.jpg]]
Masaüstü: "Erkek" hover mega menüsü (5 metin sütunu) ve altında "BU YARIŞ SENİN YARIŞIN" hero slaytı.

![[nike-plp-filtre.jpg]]
PLP: solda 3'lü numara ızgarası ve renk daireleri, kartta renk varyant şeridi ve `#D33918` rozet metni (sağ altta test ortamının konum penceresi).

![[nike-pdp.jpg]]
PDP: 9 küçük resimli dikey şerit, 4:5 ana görsel, "Numara/Beden Seç" 3 sütunlu EU ızgarası ve 60px siyah "Sepete Ekle".

![[nike-mobil-pdp.jpg]]
Mobil PDP: başlık/fiyat görselin üstünde, altta sabit tam genişlik "Sepete Ekle" çubuğu.

İlgili desen notları: [[Header ve Navigasyon]], [[Hero ve Banner Desenleri]], [[Kategori Sayfası ve Filtreler]], [[Ürün Sayfası]], [[Beden ve Kalıp]], [[Sepet ve Ödeme]], [[Güven Sinyalleri]], [[Mobil Deneyim]], [[Footer]], [[Renk ve Tipografi]], [[Türkiye E-ticaret Pazarı]], [[KPT Store Denetimi]].

## Kaynaklar

- https://www.nike.com/tr/ (gözlem, 2026-10-04)
- https://www.nike.com/tr/w/erkek-ayakkabilar-nik1zy7ok (gözlem)
- https://www.nike.com/tr/t/air-force-1-07-lv8-erkek-ayakkabisi-K3OuKghd/IW3476-001 (gözlem)
- https://www.nike.com/tr/cart (gözlem)
- https://www.nike.com/tr/help/a/kargo-teslimat (ikincil: kargo ücreti ve eşik, 2026)
- https://www.nike.com/tr/help/a/odeme-secenekleri (ikincil: ödeme yöntemleri, 2026)
- https://www.nike.com/tr/help/a/taksitli-odeme (ikincil: taksit, 2026)
- https://www.nike.com/tr/help/a/iade-politikasi-gs (ikincil: iade politikası, 2026)
- https://medyascope.tv/2024/08/10/nike-turkiyedeki-internet-alisverislerini-durdurdu/ (Nike'ın TR online satışı durdurması, 2024)
- https://www.just-style.com/newsletters/nike-halts-turkiye-online-orders-after-customs-crackdown (2024)
