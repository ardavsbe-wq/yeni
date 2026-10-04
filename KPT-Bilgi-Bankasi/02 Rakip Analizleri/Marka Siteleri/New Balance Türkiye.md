---
tür: rakip-analizi
site: New Balance Türkiye
url: https://www.newbalance.com.tr/
ülke: TR
segment: marka DTC (yerel distribütör işletmesi)
erişim: kısmi
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.newbalance.com.tr/, https://www.newbalance.com.tr/erkek-spor-ayakkabi, https://www.newbalance.com.tr/urun/new-balance-9060-4485]
etiketler: [rakip, marka-dtc, sneaker, new-balance]
---

# New Balance Türkiye

> [!summary] Özet
> New Balance'ın Türkiye resmi sitesi; KPT ile **aynı ürün adlandırma mantığını** (Marka + Model + Renk + Cinsiyet + Tür + SKU) kullanan, Türkiye pazarına göre kurgulanmış bir DTC. En güçlü 3 yanı: (1) PDP'de **stokta olmayan bedenleri gizlemeden gri dolgulu gösteren** 7 sütunlu beden ızgarası, (2) "Sepete Ekle"nin hemen altında "3 aya kadar taksit seçenekleri" ve "Fiyatı düşünce haber ver", (3) PLP'de sayaçlı checkbox/kutu/renk çipi filtreleri. KPT için en değerli ders: KPT'nin "yalnızca stoktaki bedenler" sorununa birebir çözüm olan beden ızgarası ve CTA altındaki Türkiye'ye özgü güven satırları.

> [!note] Erişim notu
> Ana sayfa, PLP ve PDP açıldı (HTTP 200). "Sepete Ekle" tıklandı ancak görünür geri bildirim çıkmadı ve sepet sayacı 0'da kaldı (sayfada reCAPTCHA rozeti var, tahmin: otomasyon nedeniyle). Sepet sayfası adresi bulunamadı (`/sepet` → 404). Sepet/ödeme **incelenemedi**. Koordinatörün bütçe talimatıyla inceleme bu noktada durduruldu.

## Kimlik ve konumlandırma

- Sayfa başlığı "New Balance Resmi Web Sitesi". Footer manifestosu: "Spor ayakkabıdan daha büyük bir şey için mücadele ediyoruz… Şimdi ya da asla: Anı yaşa."
- Retro/lifestyle (1906, 9060, 2002R, 530, 740, 725) ağırlıklı; koşu ikinci planda. Ürünlerin çoğu "Unisex" etiketli (Erkek Ayakkabı PLP'sinde 159 ürünün 117'si Unisex).
- İletişim footer'da açık: "0212 400 05 85 · Pazartesi - Cuma / 09:00 - 16:30 · iletisim@newbalance.com.tr".

## Görsel dil

| Rol | Hex | Kullanım yeri |
|---|---|---|
| Marka kırmızısı | `#CF0A2C` | "Sepete Ekle", "Satın Al", "Üye Ol" dolgusu; "İndirim" menü linki; seçili renk alt çizgisi |
| Ana metin | `#000000` | Başlık, fiyat, ürün adı |
| Nav metni | `#2D3141` | Menü linkleri, stoktaki beden metni |
| "Yeni" rozeti | `#D97706` | Kart üstü "Yeni" metni (amber) |
| Duyuru şeridi | `#151415` | Üst şerit zemini (50px) |
| Ürün görsel zemini | `#F2F2F3` / `#F5F5F5` civarı | PLP/PDP görsel arka planı |
| Stok dışı beden | zemin `#F8F8F8`, metin `#727272` | PDP beden kutusu |
| Beden çerçevesi | `#E5E5E7` (2px) | Stoktaki beden kutusu |

- **Tipografi:** "ProximaNova" (gövde, 14–16px/500) ve "ProximaNovaSemibold" (başlık, buton, nav 14px). **Hero başlığı serif: "EBGaramondMedium" 48px** ("2000", "1890A"), KPT'nin Cormorant Garamond kullanımına yakın bir sneaker örneği.
- **Şekil:** butonlar **köşesiz (0px radius)** dikdörtgen, 56px yükseklik; filtre çipleri 4px; header kategori sekmeleri 4px.

## Header ve navigasyon

- **Üst şerit (50px, `#151415`, beyaz 14px):** solda Türk bayrağı + "Türkçe ▾" | "TRY ▾"; ortada 3 mesajlı dönen şerit (nokta göstergeli): **"Koşu ve Antrenman Keşfet"**, **"%40'a Varan İndirim Satın Al"**, **"Siparişleriniz 1-3 iş günü içerisinde kargoya teslim edilecektir."** (CTA'lar 700 ağırlık, altı çizili); sağda "İade | Yardım".
- **Ana header (81px, sticky `top-0`):** solda NB logosu; "Yeniler · Erkek · Kadın · Çocuk · **İndirim** (kırmızı) · Blog"; sağda gri dolgulu dikdörtgen arama "Ara" (~176×36px), kişi ikonu + "Giriş | Üyelik", sepet ikonu + kırmızı daire sayaç "0".
- **Mega menü ("Erkek" hover, tam genişlik, görselsiz):** 5 sütun, ilk sütundan sonra dikey ayraç çizgisi:
  - Sol (vurgu listesi): En Yeniler, Koşu ve Antrenman, Outdoor ve Trail Ayakkabı, Unisex, Made in USA, MADE in UK, İkonik 574, WRPD Runner, Klasik 1906, Spor Giyim, FuelCell Rebel, Retro Ayakkabılar, Matching Sets
  - **AYAKKABI:** Günlük Giyim, Koşu, Terlik · **GİYİM:** Sweatshirt, Tişört, Eşofman Altı, Şort, Deniz Şortu, Mont & Yelek · **AKSESUAR:** Çanta, Çorap
  - **KOLEKSİYONLAR (model numarasıyla):** 1906, 9060, 2002R, 204L, 2010, 2000, 530, 740, 1000, 725, 327, 878, 408
  - Aktif menü öğesinin altında kırmızı 2px çizgi.
- **Mobil:** üst şerit + header (hamburger, kişi ikonu kırmızı nokta bildirimli, ortada logo, arama, sepet); altında **yatay kaydırmalı gri hap sekmeler** "Yeniler · Erkek · Kadın · Çocuk · İndirim" (her zaman görünür, hamburger'a gerek kalmadan hedef kitle seçimi).

## Ana sayfa ve banner/hero örnekleri

1. **Hero carousel** (tam genişlik ~1440×655px, sol/sağ ok): görselin **altında** beyaz alanda ortalı serif başlık **"2000"** / alt metin **"Modern mimariden ilham alan tasarım."** / siyah buton **"Keşfet"** (160×56px). Diğer slayt: **"1890A" / "Köklerden geleceğe." / "Keşfet"**. Mobilde buton tam genişlik kırmızı.
2. **"Öne Çıkanlar"** + segment kontrolü **Erkek | Kadın | Çocuk** (gri zemin içinde beyaz seçili sekme, 157×34px) + yatay ürün carousel'i (4 kart görünür, alt ilerleme çubuğu).
3. **2'li yaşam tarzı/ürün banner'ı:** **"204L" / "Gösterişsiz şıklık." / "Satın Al"** ve **"FuelCell Rebel" / "Hız için tasarlandı." / "Satın Al"** (kırmızı 176×56px).
4. **Bölünmüş banner:** **"725" / "2000'lerin koşu mirası." / "Keşfet"** (beyaz zemin, 2px kırmızı çerçeve, kırmızı metin).
5. **"Alışveriş Kategorileri":** 3 dikey fotoğraf kartı "Retro Ayakkabılar · Koşu ve Antrenman · Spor Giyim".
6. **"En Yeniler"** ürün carousel'i.
7. **Üyelik bandı** (siyah, 96px): "Üye ol, yeni sezonu ve koleksiyonlarımızı sen keşfet!" + kırmızı **"Üye Ol"** (172×56px).
8. **Footer:** Müşteri Hizmetleri (Kargo Takip, Sıkça Sorulan Sorular, Ürün İnceleme, İşlem Rehberi, Sözleşmeler, Mağazalar) · Kurumsal (Hakkımızda, KVKK, Veri Politikası, Ticari Ünvan, Gizlilik ve Çerez, Çerez Ayarları) · Koleksiyonlar · İletişim. Ödeme logosu görülmedi.

## Kategori sayfası (PLP)

- Breadcrumb "Anasayfa / Erkek / **Ayakkabı**"; H1 "Ayakkabı" + **"159 ürün listeleniyor"**.
- Solda "Filtreleri Gizle" (çerçeveli, ayar ikonlu); sağda "⇅ Sırala": **Yeni Gelenler · Fiyat: Düşükten Yükseğe · Fiyat: Yüksekten Düşüğe · İndirim Oranına Göre**.
- **Filtre paneli (360px, akordeon, +/− ikon):**
  1. **Kategori:** checkbox + sayaç: "Ayakkabı (159)", "Günlük Giyim (138)", "Koşu Ayakkabı (17)", "Terlik (4)".
  2. **Beden:** 5 sütunlu kare kutu ızgarası (~56×56px, 1px gri çerçeve): 35 … 46.5 (18 değer).
  3. **Renk:** hap çipler, renk noktası + ad + sayaç: "Gri (48)", "Siyah (36)", "Beyaz (19)", "Kahverengi (19)", Yeşil (10), Bej (8), Lacivert (7), Antrasit (4), Mavi, Mor, Bordo, Krem, Pembe, Turuncu.
  4. **Cinsiyet:** Unisex (117), Erkek (40), Kadın (2).
- **Kart (masaüstü 4 sütun, 252px):** kare görsel `#F5F5F5` zemin; altında **renk varyant küçük resimleri** (~36px, seçili 1px siyah çerçeve); "Yeni" (`#D97706` 14px); ürün adı H3 14px/500 iki satır; tür satırı ("Ayakkabı"/"Günlük Giyim"); fiyat 16px "10.990,00₺". Hover'da "Hızlı İncele" butonu ve kalp ikonu.
- **Sayfalama:** "12 / 159 sonuç" + **"Daha fazla"** butonu.
- Sayfa sonunda SEO metni: "New Balance Erkek Ayakkabı" ve "ENCAP Teknolojisi ile Daha Konforlu Adımlar".

## Ürün sayfası (PDP)

İncelenen: **New Balance 9060 Gri Unisex Ayakkabı U9060GRY**, 11.990,00₺.

- **Galeri:** masaüstünde **2 sütunlu dikey ızgara** (her kare ~460×460px, 8px aralık), **8 görsel** (yan, arka, taban, model üzerinde); mobilde kaydırmalı + 8 nokta.
- **Başlık bloğu:** üst satır gri küçük "Unisex Günlük Giyim U9060GRY" → H1 **"New Balance 9060 Gri Unisex Ayakkabı U9060GRY"** (16px/500) → fiyat "11.990,00₺" → **"Renk: Gri"** + renk varyant küçük resimleri (seçili kırmızı 3px alt çizgi).
- **Beden seçici:** "Beden Seçiniz:" + sağda altı çizili **"Beden Ölçüm Tablosu"**. 7 sütun, **56×44px** butonlar:
  - Stokta: şeffaf zemin, 2px `#E5E5E7` çerçeve, `#2D3141` metin.
  - **Stok dışı: `#F8F8F8` dolgu, `#727272` metin, görünür kalıyor** (36, 37, 41.5, 42, 45, 47.5).
  - Seçili: **siyah dolgu, beyaz metin**.
  - Beden seçmeden "Sepete Ekle": sağ üstte beyaz toast **"Lütfen beden seçimi yapınız"** (320×42px).
- **CTA bloğu:** kırmızı **"Sepete Ekle"** (432×56px, `#CF0A2C`, 0 radius) → gri **"3 aya kadar taksit seçenekleri"** → ikonlu linkler **"Fiyatı düşünce haber ver"**, **"Favorilerine Ekle"**, **"Paylaş"**.
- **Sticky:** masaüstünde kaydırınca sağ üstte mini kart (küçük resim + ad + "Sepete Ekle"); **mobilde sabit ATC yok**.
- **Açıklama (akordeon):** **"Ürün Açıklaması"** (1 paragraf hikâye) + **"Ürün Detayları"** (madde listesi: "ABZORB orta taban…", "Topukta yarı saydam CR cihazı" + "Ürün kodu #: U9060GRY" + "Materyal: 68% Domuz Derisi 17% Polüretan 15% Polyester").
- Yorum bölümü, teslimat tarihi yok.

## Sepet ve satın alma kolaylığı

- incelenemedi: ATC görünür geri bildirim vermedi, sayaç 0 kaldı.
- Sitede gözlenen Türkiye'ye özgü metinler: "3 aya kadar taksit seçenekleri", "Siparişleriniz 1-3 iş günü içerisinde kargoya teslim edilecektir.", header'da "İade" kısayolu. Ücretsiz kargo eşiği görülmedi.

## Mobil deneyim

- Yatay hap kategori sekmeleri; hero altı tam genişlik kırmızı "Keşfet".
- PDP: breadcrumb → galeri → başlık → renk → 5 sütunlu beden ızgarası → tam genişlik ATC (342×56px). Sticky ATC yok.

## Güven ve ikna unsurları

| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| Stok dışı bedeni gri göstermek | PDP | Kıtlık, şeffaflık | Evet, doğrudan |
| "3 aya kadar taksit seçenekleri" | CTA altı | Ödeme acısını azaltma | Evet |
| "Fiyatı düşünce haber ver" | CTA altı | Kayıp kaçınma | Evet |
| "1-3 iş günü içerisinde kargoya" | Üst şerit | Belirsizliği azaltma | Evet |
| "%40'a Varan İndirim" | Üst şerit | Çapalama | Kısmen |
| Filtre sayaçları "(48)" | PLP | Bilgi kokusu | Evet |

## Performans ve teknik gözlem

- Ana sayfa: TTFB 235 ms, load 1.106 ms, 63 istek, **225 KB**; JPG, CDN `newbalance.sm.mncdn.com`. Tailwind sınıfları. reCAPTCHA rozeti. `/sepet` 404.

## Güçlü yanlar / Zayıf yanlar

- **Güçlü:** stok dışı beden gösterimi; CTA altı taksit/fiyat alarmı; sayaçlı filtreler; mobil kategori sekmeleri; çok hafif sayfa.
- **Zayıf:** SKU'lu ürün adı uzun; tür etiketi tutarsız ("Ayakkabı"/"Günlük Giyim"); H1 16px küçük; mobil sticky ATC yok; görünür ATC geri bildirimi gözlenemedi.

## KPT için çıkarımlar

- **Uygula:**
  - PDP beden ızgarası: tüm bedenler, stok dışı `#F8F8F8` + `#727272`, seçili siyah dolgu; "Beden Ölçüm Tablosu" sağda.
  - CTA altı: "3 aya kadar taksit seçenekleri" + "Fiyatı düşünce haber ver" + "Favorilerine Ekle".
  - "Lütfen beden seçimi yapınız" toast'ı.
  - Filtre: Kategori checkbox + sayaç → Beden 5'li ızgara → Renk noktalı hap + sayaç → Cinsiyet.
  - Açıklama: "Ürün Açıklaması" + "Ürün Detayları" (özellik maddeleri + "Ürün kodu #:" + "Materyal:").
- **Uyarla:**
  - Ürün adı: H1'de SKU'yu çıkar, üst gri satırda göster; H1 ≥24px.
  - Mobil hap sekmeleri "Erkek · Kadın · Çocuk · Markalar".
  - Hero altı serif başlık + alt metin + düz buton deseni, KPT bordo `#741E32` ile.
- **Kaçın:** tutarsız tür etiketi; görünür onay vermeyen ATC; mobilde sticky ATC eksikliği.

## Ekran görüntüleri

![[nb-mega-menu.jpg]]
"Erkek" mega menüsü: vurgu listesi + AYAKKABI/GİYİM/AKSESUAR + model numaralı KOLEKSİYONLAR.

![[nb-plp-filtre.jpg]]
PLP: sayaçlı Kategori checkbox'ları, 5'li Beden ızgarası, noktalı Renk çipleri; kartta renk varyantları.

![[nb-pdp-beden.jpg]]
PDP: stok dışı gri bedenler, seçili "43" siyah; kırmızı "Sepete Ekle", taksit ve fiyat alarmı.

![[nb-mobil-pdp.jpg]]
Mobil PDP: tam genişlik ATC, taksit satırı, akordeonlar.

İlgili: [[Beden ve Kalıp]], [[Ürün Sayfası]], [[Kategori Sayfası ve Filtreler]], [[Header ve Navigasyon]], [[Güven Sinyalleri]], [[Mobil Deneyim]], [[KPT Store Denetimi]], [[Nike Türkiye]].

## Kaynaklar

- https://www.newbalance.com.tr/ (gözlem, 2026-10-04)
- https://www.newbalance.com.tr/erkek-spor-ayakkabi (gözlem)
- https://www.newbalance.com.tr/urun/new-balance-9060-4485 (gözlem)
