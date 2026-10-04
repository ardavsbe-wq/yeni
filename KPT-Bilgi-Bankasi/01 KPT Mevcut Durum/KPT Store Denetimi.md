---
tür: mevcut-durum
site: KPT Store
url: https://sensitivity-strips-icq-athletic.trycloudflare.com (geçici önizleme tüneli)
platform: OpenCart 4 + özel "kpt" eklentisi (PHP 8.3)
incelenme: 2026-10-04
incelenen-sayfalar: [ana sayfa, kategori (category_group=footwear), ürün (id=50142), arama, sepet, beden rehberi, markalar, teslimat, favoriler, hesap]
ekranlar: [masaüstü 1440×900, mobil 390×844]
etiketler: [kpt, denetim, mevcut-durum]
---

# KPT Store Denetimi

> [!summary] Özet
> KPT Store sakin, okunaklı ve erişilebilir bir iskelete sahip: kontrastlar sağlam, dokunma hedefleri 44 px, JavaScript hafif (TBT 0 ms, CLS 0,003). Satışı en çok zayıflatan şeyler: (1) hero'daki AI üretimi dönen ayakkabının çift pozlanmış görünmesi ve 900 KB'lık PNG olması, (2) kategori filtrelerinin tek seçimli açılır menüler olması ve ham tedarikçi verisiyle dolu olması, (3) ürün sayfasında karar bilgisinin eksikliği ve **bedene göre değişen fiyatın beden seçilince güncellenmemesi** (kullanıcı gerçek fiyatı ancak sepette görüyor). Bu not, siteyi yeniden yapacak ajanlar için mevcut durumun tam dökümüdür: neyi koruyacağını ve neyi düzelteceğini buradan çıkar.

İlgili notlar: [[AI Geliştirici Brief'i]] · [[Yapılacaklar Listesi]] · [[Tasarım Token Önerisi]] · [[Rakip Karşılaştırma Matrisi]]

---

## 1. Teknik altyapı

| Konu | Mevcut durum |
|---|---|
| Platform | OpenCart 4, özel `extension/kpt` eklentisi. Tüm sayfalar tek bir route üzerinden: `index.php?route=extension/kpt/common/store&page=<sayfa>` |
| Sunucu | PHP 8.3.35, Cloudflare tüneli üzerinden yayın (önizleme) |
| Güvenlik başlıkları | `content-security-policy: frame-ancestors 'self'; object-src 'none'; base-uri 'self'`, `x-frame-options: SAMEORIGIN`, `x-content-type-options: nosniff`, `referrer-policy: strict-origin-when-cross-origin`. Lighthouse en iyi uygulamalar: **100** |
| İndeksleme | `<meta name="robots" content="noindex,nofollow">` ve `x-robots-tag: noindex, nofollow`. Önizlemede doğru, yayında **kaldırılmalı** |
| Çerezler | `KPT_ATELIER` (oturum, HttpOnly, Secure, SameSite=Lax, 30 gün), `currency=TRY` |
| CSS | 8 ayrı render'ı engelleyen dosya: `fonts.css`, `store.css`, `atelier-hero.css`, `atelier-stage.css`, `atelier-commerce.css`, `atelier-navbar.css`, `footwear-preview.css`, `footwear-shell.css`, `footwear-showcase.css` |
| JS | `atelier-stage.js`, `store.js`, `analytics.js`, `atelier-commerce.js`, `footwear-showcase.js` (5 dosya, hafif) |
| Fontlar | Kendi sunucusunda woff2: Manrope 400–800 (5 dosya), Cormorant Garamond 400/500, Anton (tanımlı), Archivo Black (logo). Türkçe karakterlerin tamamı mevcut (fontTools ile doğrulandı) |
| Yapılandırılmış veri | Ürün sayfasında **canonical yok, JSON-LD yok, Open Graph yok** |
| URL yapısı | Anlamsız: `...&page=product&id=50142`. Slug tabanlı URL gerekli (`/new-balance-9060-beyaz-u9060eee`) |

## 2. Ölçümler

### Lighthouse 13.5 (ana sayfa)

| Kategori | Mobil | Masaüstü |
|---|---|---|
| Performans | 73 | 83 |
| Erişilebilirlik | 96 | 96 |
| En iyi uygulamalar | 100 | 100 |
| SEO | 66 (noindex nedeniyle) | 66 |

| Metrik | Mobil | Masaüstü | Hedef |
|---|---|---|---|
| FCP | 2,4 sn | 1,1 sn | < 1,8 sn |
| LCP | **5,8 sn** | 2,3 sn | < 2,5 sn |
| TBT | 0 ms | 0 ms | < 200 ms |
| CLS | 0,003 | 0,003 | < 0,1 |
| Speed Index | 4,4 sn | 1,9 sn | < 3,4 sn |
| Sayfa ağırlığı | 2.253 KiB | 2.314 KiB | < 1.500 KiB |
| TTFB | 810 ms | 990 ms | < 200 ms (önbellekli) |

- **LCP öğesi:** hero'daki `span.kpt-showcase__turntable-layer` (CSS arka plan görseli). LCP dökümü: TTFB 948 ms + **kaynak yükleme gecikmesi 1.848 ms** + yükleme 521 ms + render 80 ms. Gecikmenin sebebi görselin CSS `background-image` olduğu için tarayıcının onu geç keşfetmesi.
- **En ağır görseller:** `image/catalog/kpt/campaign/turntable-ai/nb-9060-turntable.png` (905 KB) ve `adidas-samba-turntable.png` (908 KB). Görsel teslimiyle ~1,3 MB tasarruf mümkün.
- **Render'ı engelleyen CSS:** mobilde ~1 sn tahmini kazanç.
- TTFB ölçümü Cloudflare tüneli üzerinden yapıldı; gerçek sunucuda yeniden ölçülmeli.
- Ana sayfada 361 `<img>` var; **343'ü** arama paneli için önceden DOM'a basılmış gizli sonuç görseli (`data-search-src`). Gereksiz DOM yükü.

### Erişilebilirlik (axe-core 4.13, WCAG 2.2 AA)

| Kural | Etki | Yer |
|---|---|---|
| `list` | Ciddi | `ol.atelier-stage-slides` içinde `<li>` olmayan doğrudan çocuk |
| `label-content-name-mismatch` (Lighthouse) | Orta | Hero "Ürünü incele" linki ve model sekmeleri (01 9060 / 02 Samba / 03 JA 3): `aria-label` görünen metinle başlamıyor; sesle kontrol eden kullanıcılar butonu bulamaz |

Ürün ve kategori sayfasında axe ihlali bulunmadı.

### Kontrast (WCAG oranları, hesaplandı)

| Çift | Oran | Durum |
|---|---|---|
| Ink `#171B1C` / Paper `#F3F4F1` | 15,72 | AAA |
| Sage gri `#56605E` / Paper | 5,89 | AA |
| Model adı `#626F65` / Sage `#E5E8E3` | 4,27 | AA (yalnızca büyük metin; 96 px kullanılıyor, geçer) |
| Taupe `#6A5D54` / Paper | 5,75 | AA |
| Taupe `#6A5D54` / Kum `#D8CFC3` | **4,12** | Küçük metinde **AA'yı geçmiyor** |
| Beyaz / Bordo `#741E32` | 10,64 | AAA |
| Paper `#F3EFE7` / Kahve `#2B211D` | 13,69 | AAA |
| Bordo / Paper | 9,63 | AAA |
| `#485249` / Sage | 6,59 | AA |

## 3. Görsel dil

### Renk paleti (hesaplanmış stillerden)

| Rol | Hex | Kullanım |
|---|---|---|
| Ink (metin) | `#171B1C` | Ana metin, header ikonları, footer zemini |
| Paper (zemin) | `#F3F4F1` | Sayfa zemini, footer metni |
| Sage (yüzey) | `#E5E8E3` | Hero zemini, ürün görsel zemini |
| Sage gri | `#56605E` | Yardımcı metin (alt başlık, meta) |
| Model gri-yeşil | `#626F65` | Hero'daki dev model adı ("9060") |
| Bordo (vurgu) | `#741E32` | Birincil CTA (mobil hero, Sepete ekle, Ara, Sırala), sepet ikonu, aktif sekme |
| Kahve | `#2B211D` | Atölye bölümü metni ve "Ürünü incele" butonu |
| Taupe | `#6A5D54` | Atölye bölümü yardımcı metni |
| Kum | `#D8CFC3` | Atölye çizgileri/yüzey |
| Krem | `#F3EFE7` | Atölye bölümü zemini, `theme-color` |
| Kiremit (eski) | `#BD3525` | `:root` içinde tanımlı eski vurgu token'ı |

> [!warning] Üç token katmanı iç içe
> CSS'te üç ayrı tema sistemi var:
> 1. `:root`: `--paper:#f6f5f0; --ink:#141513; --muted:#61635e; --line:#d9d9d1; --accent:#bd3525; --surface:#eeeee9; --display:'Anton'`
> 2. `.theme-atelier`: `--paper:#f3efe7; --ink:#2b211d; --muted:#6a5d54; --line:#d8cfc3; --accent:#741e32; --surface:#e9e2d7; --display:'Cormorant Garamond'`
> 3. footwear katmanı (sabit değerler): `#171B1C`, `#F3F4F1`, `#E5E8E3`, `#56605E`
>
> Sonuç: sayfa soğuk adaçayı tonları ile sıcak krem/kum tonları arasında gidip geliyor, birincil butonlar üç farklı renkte (bordo, kahve, neredeyse siyah). Tek token setine inilmeli → [[Tasarım Token Önerisi]].

### Tipografi

| Rol | Font | Boyut | Not |
|---|---|---|---|
| Logo | Archivo Black | ~28 px | "KPT STORE", büyük harf |
| Hero marka | Manrope 700 | 29 px | "New Balance" |
| Hero model adı | Manrope 800 | 96 px | "9060", `#626F65` |
| Hero slogan | Manrope 700 | 42 px | "Karakteri tabanında." |
| Bölüm başlıkları | Manrope 800 | 42 px | "Bir sonraki adımın.", harf aralığı -0,035/-0,055em |
| Atölye başlıkları | Cormorant Garamond 500 | ~40 px | "Bir modelden başla.", "9060", arama "Aradığın ürünü bul." |
| Gövde/meta | Manrope 400–600 | **12–14 px** | En sık boyutlar: 13 px (58 öğe), 12 px (39), 14 px (24); 10–11 px de var |
| Menü | Manrope 700 | 13 px | Büyük harf, harf aralığı ~0,04em |

> [!warning] Yazı boyutu tabanı düşük
> Meta ve gövde metninde 12–13 px baskın. Mobilde meta en az 14 px, gövde ve form alanları 16 px olmalı (iOS 16 px altındaki input'larda sayfayı yakınlaştırır). Detay: [[Renk ve Tipografi]].

### Diğer

- Köşe yuvarlaklığı: butonlar ve kutular **0 px** (keskin köşe); favori butonu tam daire; arama kutusu hap (pill).
- İkonlar: ince çizgi (outline) ikonlar; sepet ikonu dolgulu bordo alışveriş çantası içinde "K".
- Ürün görselleri: `#E5E8E3` zeminde paketçekim (packshot); bazı tedarikçi görselleri farklı zeminde (ör. turuncu zeminli Nike Mind 001 Slide).
- Hareket: hero'da otomatik dönen 12 karelik sprite ve otomatik model geçişi; atölye bölümünde otomatik ilerleyen slayt (Durdur butonu var).

## 4. Sayfa sayfa döküm

### 4.1 Header ve navigasyon

- **Masaüstü:** Logo (sol) · menü (orta): `AYAKKABI` · `KOŞU` · `TERLİK` · `MODELLER ▾` · `MARKALAR ▾` · arama kutusu "Model veya marka ara" (hap şekilli, `#E5E8E3` zemin) · ikonlar: favoriler, sepet (bordo), hesap.
- **Mobil:** Logo · arama ikonu · sepet ikonu · hamburger. Hamburger menü içeriği: `Ayakkabı`, `Koşu`, `Terlik`, `Modeller`, `Markalar`, `Kadın`, `Erkek`, `Favorilerim`, `Hesabım`. Dikkat: **Kadın/Erkek yalnızca mobil menüde var, masaüstünde yok; Çocuk hiçbir yerde yok** (oysa katalogda çok sayıda çocuk ürünü var).
- **Üst şerit:** "İstanbul · 4 Ekim Pazar · Ekim modelleri" (tarih/şehir; karar vermeye yardımcı bilgi taşımıyor).

> [!bug] Mobil menü tutarsız açılıyor
> Otomatik testlerde aynı tıklama bazen menüyü açtı, bazen açmadı (`aria-expanded` false kaldı, `#main-nav` `display:none`). Sebep adayı: aynı butona iki ayrı script tıklama dinleyicisi bağlıyor (`store.js` genel `[data-toggle]` dinleyicisi menüyü açıp ilk linke odaklanıyor; `atelier-commerce.js` ayrıca `navToggle` click dinleyicisi ve header üzerinde menüyü kapatan bir `focusout` dinleyicisi ekliyor). Gerçek iOS ve Android cihazlarda test edilmeli; menü açma/kapatma mantığı tek bir yerde toplanmalı.

![[kpt-mobil-menu.jpg]]
*Mobil menü açıkken (dokunma ile açıldığı bir deneme).*

### 4.2 Ana sayfa (yukarıdan aşağı)

1. **Hero vitrin (showcase):** 3 model, ekrana sabitlenmiş (pinned) kartlar, kaydırdıkça değişiyor ve kendiliğinden birkaç saniyede bir sonraki modele geçiyor.
   - 01 New Balance **9060**: slogan "Karakteri tabanında.", ürün "9060 UNISEX LIFESTYLE SNEAKER", "14.025,00 TL'den", CTA "Ürünü incele →"
   - 02 adidas **Samba**: slogan "Her adımda klasik.", ürün "Samba OG Unisex Beyaz Sneaker", "5.650,00 TL"
   - 03 Nike **JA 3**
   - Alt kontrol çubuğu: "↓ Kaydır, farklı açıları keşfet" · sekmeler `01 9060` `02 Samba` `03 JA 3` · "diğer açıyı göster" ikonu · Oynat/Durdur.
   - Etiket: "AI ile oluşturulmuş görselleştirme".
   - Masaüstünde kataloğa ulaşmak için ~2.200 px, mobilde ~2.000 px kaydırma gerekiyor (≈2,5 ekran).
2. **Marka satırı:** New Balance · Nike · adidas · Skechers · Puma · Vans (metin, logo değil).
3. **"Numaranla başla."**: 22'den 49.5'e kadar 50 beden butonu (masaüstünde 3 satır, mobilde 8 satır).
4. **"Bir sonraki adımın."** / "Günlük rotan için farklı silüetler." · "Tüm ayakkabılar →" · 8 ürün kartı (masaüstü 4 sütun, mobil 2 sütun).
5. **"Bir modelden başla."** (atölye bölümü, krem zemin, Cormorant başlık): eğik kesilmiş ürün kartı, "NEW BALANCE / 9060 / Beyaz · Unisex / 14.025,00 TL'den / Ürünü incele", altında 6 ürünlük ilerleme çubuğu ve "Durdur".
6. **Hizmet linkleri:** "Doğru numarayı bul. — Ölçü ve beden rehberi" · "Favorilerine dön. — Aklında kalan modeller" · "Alışverişini planla. — Teslimat ve iade bilgileri".
7. **Footer** (siyah).

![[kpt-hero-cift-pozlama.jpg]]
*0,7 sn arayla alınan 4 kare: 2. ve 3. karede iki açı üst üste biniyor (opaklıklar 0,48/0,52), 4. karede hero kendiliğinden Samba'ya geçmiş.*

> [!bug] Hero görseli çift pozlanmış
> Dönen ayakkabı 12 karelik bir sprite (4×3, `background-size: 400% 300%`). İki `.kpt-showcase__turntable-layer` katmanı yaklaşık %50 opaklıkla üst üste binerek geçiş yapıyor; 30° açı farkı olan iki kare karıştığı için ürün çoğu an yarı saydam ve bulanık görünüyor. Çözüm: çapraz geçişi kaldırıp kareler arasında doğrudan geçiş, 24–36 kare veya 2–3 sn'lik döngü video (WebM/MP4 + poster). Daha iyisi: gerçek fotoğraf. → [[Hero ve Banner Desenleri]]

![[kpt-mobil-hero.jpg]]
*Mobil hero: bordo "Ürünü incele" butonu tek doygun renk olduğu için iyi ayrışıyor (Von Restorff).*

![[kpt-masaustu-ilk-ekran.jpg]]
*Masaüstü ilk açılış: çerez penceresi hero'daki ürün adını ve butonu kapatıyor.*

![[kpt-numaranla-basla-ve-urunler.jpg]]
*Marka satırı, "Numaranla başla" beden ızgarası ve ürün kartları.*

![[kpt-atolye-bolumu.jpg]]
*Atölye bölümü: krem zemin, Cormorant Garamond başlık, kahve buton. Sayfanın geri kalanıyla farklı bir renk sıcaklığı.*

### 4.3 Çerez penceresi

- Başlık "Seçimin sana özel olsun.", metin "İzinle gezdiğin ürünleri hatırlar, ilgin doğrultusunda öneriler sunarız. İzin vermeden de alışveriş yapabilirsin."
- Butonlar: "Yalnızca gerekli" (çerçeveli) · "İzin ver" (siyah dolgulu) · "Tercihleri özelleştir +".
- Masaüstünde sağ altta 390×220 px kutu; mobilde ekranın ~%25'i.
- **Seçim yapınca sayfa baştan yükleniyor** (tam sayfa navigasyonu). Seçim sayfayı yenilemeden uygulanmalı.
- Olumlu: "Yalnızca gerekli" ile "İzin ver" eşit ağırlıkta; karanlık desen yok (KVKK çerez rehberiyle uyumlu yaklaşım). → [[Türkiye E-ticaret Pazarı]]

### 4.4 Kategori sayfası (PLP)

URL: `...&page=catalog&category_group=footwear` · Başlık "Ayakkabını bul" · alt metin "Markanı, numaranı ve rengini seç; sana uyan modeli keşfet." · "321 ürün" · 14 sayfa.

- **Filtreler (masaüstü sol kolon, mobilde "Filtreler 1 aktif" ile açılır):** "Ürün ara" metin kutusu · Marka (açılır menü) · Kategori (açılır menü) · Kullanıcı (Tümü/Unisex/Kadın/Erkek/Çocuk, açılır menü) · Numara (açılır menü, 50+ değer) · Renk (açılır menü, 50+ değer) · "En yüksek fiyat (TL)" · "Yalnızca stoktakiler" · **"Filtreleri uygula"** butonu · "Tüm filtreleri temizle". Hepsi **tek seçimli**.
- **Sıralama:** açılır menü (Yeni eklenenler / Fiyat: düşükten yükseğe / Fiyat: yüksekten düşüğe / Ürün adı) + ayrı bordo **"Sırala"** butonu.
- **Uygulanan filtre çipi:** "Kategori grubu: Ayakkabı ✕" + "Tümünü temizle" (iyi).
- **Ürün kartı:** görsel (kare, `#E5E8E3` zemin) · sağ üstte daire favori butonu (44×44) · marka (kalın) · ürün adı · "Kitle · Kategori" (ör. "Kadın · Casual Ayakkabı") · fiyat (sağa hizalı, "TL'den" ekli olabilir). Masaüstü 3 sütun, mobil 2 sütun.

> [!bug] Renk filtresi verisi kirli
> Gerçek değerlerden örnekler: `Alpine snow-puma white`, `Belirtilmemiş`, `Beyaz/pembe/altın`, `Beyaz gümüş`, `Buz Mavisi / Siyah`, `Cwhıte/cgreen/magbeı`, `Grey three`, `Görseldeki renk`, `Gül kurusu- natürel`, `Lavender mınt`, `Lıght grey`, `Panda`, `Purple mınt`, `Siyah / pembe altin`, `Siyah / Pembe Altın`, `Siyah / pembe altın`, `Sugared almond-puma white`, `Weiß`, `Whıte/whıte/vıvıd green`.
> "whıte", "Lıght", "mınt" yazımları, İngilizce kelimelerin **Türkçe yerel ayarla küçük harfe çevrildiğini** (I → ı) gösteriyor: kod hatası. Çözüm: renkleri ~14 aileye eşleyen bir tablo (`renk_ailesi`: Siyah, Beyaz, Gri, Bej/Krem, Kahverengi, Lacivert, Mavi, Yeşil, Kırmızı, Bordo, Pembe, Mor, Sarı/Turuncu, Çok renkli), orijinal renk adı ürün sayfasında "renk adı" olarak kalsın; küçük harf dönüşümü `mb_strtolower($s, 'UTF-8')` ile yerelden bağımsız yapılsın (Türkçe metinler için ayrı kural).

> [!bug] Beden ve kategori verisi
> - Numara listesi: `22 … 49.5` buçuklu EU bedenler ile adidas'ın kesirli bedenleri (`36 2/3`, `37 1/3`, `38 2/3`, `39 1/3`, `40 2/3`, `41 1/3`, `42 2/3`, `43 1/3`, `43 2/3`, `44 2/3`, `45 1/3`, `48 2/3`) aynı listede, çocuk ve yetişkin karışık. → [[Ayakkabı Beden ve Kalıp]]
> - "Ayakkabı" grubundayken kategori listesinde `Mont`, `Spor Mont`, `Oyun Kartları` da çıkıyor; marka listesinde `Panini` (çıkartma albümü) ve `Columbia` var.

> [!bug] Ürün adları tutarsız
> Gerçek örnekler: "9060 UNISEX LIFESTYLE SNEAKER" · "Mind 001" · "Palermo Moda Wns PUMA White-PUMA Black" · "Mind 001 Slide Summit White (W)" · "GARAGE Büyük Erkek Çocuk Siyah Spor Ayakkabı BKNV" · "Mind Slide Flyknit Slide Bronze Eclipse Total Orange (2 numara büyük alınması tavsiye edilir.) TERLİK" · "Ja 3 Jurassic Park "Explorer" Erkek Basketbol Ayakkabısı". Standart: **Marka + Model + Renk adı** (ör. "New Balance 9060 Sea Salt"); kitle ve kategori ayrı alanlarda; kalıp notu PDP'de "Kalıp" alanında; tedarikçi kodları "Ürün detayları"nda.

![[kpt-plp-masaustu.jpg]]
*Masaüstü PLP: beş tek seçimli açılır filtre, ayrı "Sırala" butonu, farklı zeminli ürün görselleri.*

![[kpt-plp-mobil.jpg]]
*Mobil PLP: filtreler katlanmış, sıralama kutusu ve butonu ürünlerden önce büyük yer kaplıyor.*

### 4.5 Ürün sayfası (PDP)

Örnek: `...&page=product&id=50142` (New Balance 9060).

- Breadcrumb: "Ana sayfa / Sneaker / New Balance".
- **Galeri:** masaüstünde 2×2 ızgara (5 görsel), her karede büyüteç ikonu; dikey fotoğraflar geniş karelere sığdırıldığı için yanlarda gri boşluk. Mobilde kaydırılabilir galeri, "1 / 5" sayacı ve ok butonları, "Fotoğrafları büyütmek için seç." ipucu.
- **Bilgi kolonu:** "New Balance" · H1 "9060 UNISEX LIFESTYLE SNEAKER" · "Unisex · Beyaz" · fiyat "14.025,00 TL'den" · "Beden seç" + "Beden rehberi →" · beden kutuları (yalnızca stokta olanlar: 38.5, 39.5, 40) · "Sepete eklemek için bedenini seç." · "Adet" (− 1 +) · bordo "Sepete ekle" (tam genişlik, 64 px yükseklik) · "Fiyat seçtiğin bedene göre değişir. Bu mağaza inceleme aşamasındadır. Gerçek ödeme ve sevkiyat yapılmaz." · akordeonlar: "Ürün açıklaması" (açık), "Ürün detayları", "Teslimat & iade".
- **Ürün açıklaması:** yalnızca "NEW BALANCE 9060 UNISEX LIFESTYLE SNEAKER" (ürün adının tekrarı).
- **Alt bölüm:** "Keşfe devam." / "İncelediğin modele yakın ürünleri keşfet." / "Son baktıkların" (3 ürün; mobilde 2 sütunlu ızgarada tek kalan kart).

> [!bug] Beden seçilince fiyat güncellenmiyor (kritik)
> Beden kutuları `data-variant-price` taşıyor: **38.5 → 14.674 TL**, **39.5 → 14.480 TL**, **40 → 14.025 TL**. 39.5 seçildiğinde sayfadaki fiyat "14.025,00 TL'den" olarak kalıyor; sepette ise **14.480,00 TL** çıkıyor. Kullanıcı sepette beklemediği bir fiyat artışıyla karşılaşıyor: Baymard'a göre beklenmedik maliyetler sepet terkinin en büyük nedeni ve bu durum fiyat gösterimi açısından yasal risk de taşır. Çözüm: beden seçilince fiyat anında güncellensin; beden kutularında fark gösterilsin (ör. küçük "+649 TL"); seçimden önce aralık yazılsın ("14.025–14.674 TL"). → [[Ürün Sayfası]], [[Türkiye E-ticaret Pazarı]]

> [!bug] Diğer PDP eksikleri
> - Stokta olmayan bedenler hiç görünmüyor; kullanıcı kendi bedeninin tükendiğini mi yoksa hiç gelmediğini mi anlayamıyor. Tüm aralık gösterilmeli; tükenenler üstü çizili + "Gelince haber ver".
> - Butonun yanında teslim tarihi, iade süresi, taksit, orijinallik bilgisi yok (akordeonda saklı).
> - Sneaker için gereksiz adet seçici.
> - Mobilde sabit (sticky) "Sepete ekle" çubuğu yok; kaydırınca buton kayboluyor.
> - Yorum/puan yok; kalıp bilgisi yok; malzeme, renk adı, stil kodu yok.

![[kpt-pdp-masaustu.jpg]]
*Masaüstü PDP: yalnızca 3 beden, adet seçici, ürün adını tekrar eden açıklama.*

![[kpt-pdp-mobil.jpg]]

### 4.6 Sepete ekleme geri bildirimi (iyi çalışıyor)

- Beden seçmeden "Sepete ekle"ye basınca: "Lütfen mevcut bedenlerden birini seç." uyarısı.
- Beden seçilince kutu bordo dolguya dönüyor.
- Ekleme sonrası: butonun altında çerçeveli satır içi mesaj "Sepetine eklendi. Alışverişe devam edebilirsin." + altta koyu toast "Seçtiğin beden sepete eklendi. **Sepeti gör**" + header'daki sepet ikonunda "1" rozeti. Kullanıcı sayfada kalıyor.

![[kpt-pdp-sepete-eklendi-mobil.jpg]]

### 4.7 Sepet

- Başlık "Alışveriş sepetin" · "1 ürün" · satır: "9060 UNISEX LIFESTYLE SNEAKER · 39.5", "Beyaz · Beden 39.5", Adet + **"Güncelle"** butonu (otomatik güncellenmiyor), "Kaldır", "14.480,00 TL" · "Alışverişe devam et".
- "Sipariş özeti": Ara toplam · Teslimat "Test siparişi · 0,00 TL" · Toplam · bordo "Ödemeye geç" · "Yerel test ödemesi. Kart bilgisi istenmez."
- Alt bölüm "Son baktıkların": sneaker sepetinin altında **Panini çıkartma albümü** öneriliyor (alakasız çapraz satış).
- Boş sepet: "Sepetin yeni keşiflere açık. Bir ürün ve beden seçerek başlayabilirsin. — Ürünleri keşfet" (iyi bir boş durum metni).
- Eksik: ücretsiz kargo eşiği/ilerleme çubuğu, tahmini teslim tarihi, ödeme yöntemi logoları, taksit bilgisi, kupon alanı.

![[kpt-sepet-mobil.jpg]]

### 4.8 Arama

- Header'daki arama tam ekran panel açıyor: Cormorant başlık "Aradığın ürünü bul.", bordo çerçeveli giriş kutusu, bordo "Ara →" butonu, "Bir modelden başla" öneri linkleri (New Balance 9060, Nike Mind 001, ...).
- Yazarken canlı sonuç: "9 ürün bulundu. İlk 4 eşleşme gösteriliyor." + küçük görselli 4 sonuç + "Tüm sonuçları gör →". İyi bir desen; küçük görseller dikey kırpılmış ve gri bantlı.
- Sorun: tüm ürünlerin arama görselleri sayfa yüklenirken DOM'a basılıyor (343 gizli `<img>`).

![[kpt-arama-mobil.jpg]]

### 4.9 Bilgi sayfaları

- **Beden rehberi** ("Doğru beden, iyi bir başlangıç."): 3 adımlı ölçüm yöntemi metni, "kesin beden tablosu yerine geçmez" uyarısı, "Beden hakkında soru sor". **Beden tablosu yok, görsel yok, marka bazlı dönüşüm yok.** → [[Ayakkabı Beden ve Kalıp]]
- **Markalar** ("İyi markalar, kendi seçkin."): 8 marka, hepsinde aynı tek cümle "Koleksiyondaki ürünleri beden, numara ve rengine göre keşfet." Marka hikâyesi, logo, öne çıkan model yok.
- **Teslimat ve iade:** yer tutucu metin: "Satıcı unvanı, adresi, iletişim bilgileri, ödeme sağlayıcısı, kargo ücretleri, teslimat süreleri, mesafeli satış sözleşmesi ve iade prosedürü gerçek işletme bilgileriyle tamamlanacaktır." Yayın öncesi zorunlu yasal içerik → [[Türkiye E-ticaret Pazarı]].
- **Favoriler (boş):** "İlk favorin hangisi olacak? Ürünlerdeki kalbe dokun, kendi seçkini oluştur."
- **Hesap:** "Yeniden hoş geldin." e-posta + şifre ("en az 10 karakter"), "Şifremi unuttum", "Hesap oluştur".

![[kpt-beden-rehberi.jpg]]

### 4.10 Footer

Siyah zemin. Sol: logo, "Bir sonraki favorin burada.", "Ayakkabı · Mont · Koleksiyon". Kolonlar: **Keşfet** (Tüm ürünler, Markalar, Favoriler, Son baktıkların) · **Yanındayız** (KPT hakkında, İletişim, Sık sorulan sorular, Beden rehberi, Teslimat ve iade) · **Tercihler senin** (Gizlilik, Kullanım koşulları, İzin tercihlerini düzenle, Hesabım). Alt satır: "© 2026 KPT Store · Ön izleme" · "Gerçek ürün kataloğu · Gerçek ödeme ve sevkiyat yapılmaz".
Eksik: iletişim bilgisi (telefon/e-posta/adres), ödeme logoları, sosyal medya, e-bülten, ETBİS kaydı, KVKK aydınlatma metni, mesafeli satış sözleşmesi, ön bilgilendirme formu, iade formu bağlantıları.

![[kpt-footer.jpg]]

## 5. Mikro metin ve marka sesi (korunmalı)

Ton: samimi "sen" dili, kısa, nokta ile biten başlıklar. Örnekler: "Kendi adımını keşfet." · "Karakteri tabanında." · "Her adımda klasik." · "Numaranla başla." · "Bir sonraki adımın." · "Günlük rotan için farklı silüetler." · "Bir modelden başla." · "Doğru numarayı bul." · "Favorilerine dön." · "Alışverişini planla." · "Sepetin yeni keşiflere açık." · "İlk favorin hangisi olacak?" · "Seçimin sana özel olsun." · "Bir sonraki favorin burada."
Bu ses tutarlı ve ayırt edici; yeni tasarımda korunmalı. Yalnızca bilgi taşıması gereken yerlerde (üst şerit, PDP güven bloğu) somut bilgiyle desteklenmeli.

## 6. Güçlü yanlar (korunacaklar)

1. **"Numaranla başla"**: beden öncelikli keşif; incelenen rakiplerin hiçbirinin ana sayfasında yok. Kompaktlaştırılarak korunmalı (ör. kullanıcının seçtiği beden hatırlanıp PLP'de varsayılan filtre olsun).
2. Kontrast ve dokunma hedefleri (44×44 px ikon butonları, 52–64 px birincil butonlar).
3. Anlamlı `aria-label`'lar ("Favorilere ekle: 9060 UNISEX…"), otomatik hareket için Durdur/Oynat düğmesi.
4. Hafif JavaScript (TBT 0 ms), düşük CLS.
5. Sepete ekleme geri bildirimi (satır içi mesaj + toast + rozet).
6. Canlı arama paneli ve sonuç sayısı.
7. Çerez penceresinde eşit ağırlıklı seçenekler.
8. İyi boş durum metinleri (sepet, favoriler).
9. Tutarlı marka sesi.
10. Bordonun tek doygun renk olması (doğru kullanılırsa güçlü bir eylem rengi).

## 7. Öncelikli sorun listesi

| # | Sorun | Önem | Desen notu |
|---|---|---|---|
| 1 | Beden seçilince fiyat güncellenmiyor, sepette farklı fiyat | Kritik | [[Ürün Sayfası]] |
| 2 | Hero ürünü çift pozlanmış, AI görsel, 900 KB PNG, LCP 5,8 sn | Kritik | [[Hero ve Banner Desenleri]] |
| 3 | Renk filtresi kirli veri + I→ı hatası | Kritik | [[Kategori Sayfası ve Filtreler]] |
| 4 | PDP'de yalnızca stoktaki bedenler | Kritik | [[Beden ve Kalıp]] |
| 5 | Mobil menü tutarsız açılıyor | Yüksek (doğrulanmalı) | [[Header ve Navigasyon]] |
| 6 | Tek seçimli açılır filtreler + "Uygula" ve "Sırala" butonları | Yüksek | [[Kategori Sayfası ve Filtreler]] |
| 7 | Erkek/Kadın/Çocuk masaüstü menüsünde yok | Yüksek | [[Header ve Navigasyon]] |
| 8 | PDP'de güven bloğu yok (teslimat, iade, taksit, orijinallik) | Yüksek | [[Güven Sinyalleri]] |
| 9 | Ürün adı standardı yok, açıklamalar boş | Yüksek | [[Ürün Sayfası]] |
| 10 | Kataloğa ulaşmak 2,5 ekran kaydırma; otomatik dönen hero | Yüksek | [[Hero ve Banner Desenleri]] |
| 11 | Üç token katmanı, üç birincil buton rengi, 3 font ailesi | Orta | [[Renk ve Tipografi]] |
| 12 | 12–13 px baskın yazı boyutu | Orta | [[Renk ve Tipografi]] |
| 13 | Mobilde sticky sepete ekle yok | Orta | [[Mobil Deneyim]] |
| 14 | 8 render-blocking CSS, 343 gizli arama görseli | Orta | [[E-ticaret UX Verileri]] |
| 15 | Çerez seçimi sayfayı yeniliyor | Orta | [[Güven Sinyalleri]] |
| 16 | Anlamsız URL, canonical/JSON-LD/OG yok | Orta | [[AI Geliştirici Brief'i]] |
| 17 | Sepette alakasız çapraz satış (Panini), ücretsiz kargo eşiği yok | Orta | [[Sepet ve Ödeme]] |
| 18 | Beden rehberinde tablo yok | Orta | [[Ayakkabı Beden ve Kalıp]] |
| 19 | Footer'da yasal ve iletişim bilgileri eksik | Yayın öncesi zorunlu | [[Footer]] |
| 20 | `ol` içinde `li` dışı öğe, aria-label uyuşmazlığı | Düşük | [[E-ticaret UX Verileri]] |

## Kaynaklar

- Ölçümler: Lighthouse 13.5.0, axe-core 4.13.0, Playwright 1.56 + Chromium, fontTools; 4 Ekim 2026'da önizleme tüneli üzerinden.
- Kod incelemesi: `store.js`, `atelier-commerce.js`, `fonts.css`, sayfa HTML'i (herkese açık kaynaklar).
