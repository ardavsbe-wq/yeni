---
tür: uygulama
konu: geliştirici-brief
öncelik: önce-bunu-oku
etiketler: [uygulama, brief, kabul-kriterleri]
---

# AI Geliştirici Brief'i

> [!important] Görev
> KPT Store'un (OpenCart 4 + özel `extension/kpt` eklentisi) ön yüzünü, aşağıdaki kurallara ve kabul kriterlerine göre yeniden tasarla ve geliştir. Mevcut sitenin marka sesini, beden öncelikli keşif fikrini ve erişilebilirlik temelini koru; [[KPT Store Denetimi]]'nde listelenen hataları düzelt; [[Tasarım Token Önerisi]]'ndeki tek token sistemini uygula.

## 1. Bağlam

- **Ne satıyoruz:** sneaker ağırlıklı ayakkabı (yetişkin ve çocuk), az miktarda mont/giyim, terlik. Markalar: New Balance, Nike, adidas, Skechers, Puma, Vans, Columbia. ~321 ayakkabı.
- **Kime:** Türkiye'deki online alışverişçi; çekirdek kitle Gen Z ve Millennial sneaker alıcısı + konfor odaklı günlük kullanıcı (Skechers). Bkz. [[Sneaker Kültürü ve Alıcı Profili]], [[Türkiye E-ticaret Pazarı]].
- **Konumlandırma:** sakin, seçkin, "atölye" hissi veren çok markalı butik; bağıran indirim pazarı değil.
- **Marka sesi:** samimi "sen" dili, kısa, noktayla biten başlıklar ("Numaranla başla.", "Bir sonraki adımın."). Korunur. Örnekler: [[KPT Store Denetimi#5. Mikro metin ve marka sesi (korunmalı)]].

## 2. Değişmez kurallar

1. **Fiyat dürüstlüğü:** ekranda görülen fiyat = sepetteki fiyat. Beden bazlı fiyat varsa beden seçimiyle anında güncellenir.
2. **Karanlık desen yok:** sahte stok/sayaç, önceden işaretli onay kutuları, gizli maliyet, utandırıcı ret metni yok. Bkz. [[Satın Alma Psikolojisi]].
3. **Gerçek ürün görseli:** markalı ürünler AI ile yeniden çizilmez. Kampanya atmosferi için AI kullanılırsa "Yapay zekâ ile oluşturulmuştur" etiketi (Türk rakiplerde gözlenen uygulama, bkz. [[Türkiye Sneaker Mağazaları]]).
4. **Tek vurgu rengi** (bordo `#741E32`) yalnızca birincil satın alma eylemlerinde ve seçili durumlarda.
5. **Erişilebilirlik:** WCAG 2.2 AA. Türkiye'de 2025/10 sayılı Genelge e-ticaret siteleri için WCAG 2.2 uyumuna 21.06.2027'ye kadar süre tanıyor (bkz. [[E-ticaret UX Verileri]]). Klavye ile tüm akış tamamlanabilir; odak görünür; dokunma hedefi ≥44 px.
6. **Performans bütçesi:** mobil LCP < 2,5 sn, INP < 200 ms, CLS < 0,1; ana sayfa ilk yük ≤ 1,2 MB; render'ı engelleyen CSS tek dosya + kritik CSS satır içi.
7. **Yasal zorunluluklar** yayın öncesi tamam: [[Türkiye E-ticaret Pazarı]] içindeki yasal kontrol listesi.
8. Rakip notlarındaki desenler **uyarlanır, kopyalanmaz**; başka markaların görsel ve metinleri kullanılmaz.

## 3. Veri modeli değişiklikleri (önce bunlar, çünkü UI bunlara dayanıyor)

| Alan | Tür | Not |
|---|---|---|
| `urun_adi_gorunen` | metin | **Marka + Model + Renk adı**: "New Balance 9060 Sea Salt". Tedarikçi adı ayrı alanda saklanır |
| `model` | metin | "9060", "Samba OG" (arama ve gruplama için) |
| `renk_adi` | metin | Tedarikçinin renk adı, temizlenmiş ("Sea Salt", "Beyaz/Siyah") |
| `renk_ailesi` | enum | Siyah, Beyaz, Gri, Bej/Krem, Kahverengi, Lacivert, Mavi, Yeşil, Kırmızı, Bordo, Pembe, Mor, Sarı/Turuncu, Çok renkli |
| `kitle` | enum | Erkek, Kadın, Unisex, Çocuk (Bebek/Küçük/Büyük çocuk alt kırılımı opsiyonel) |
| `kategori` | enum | Sneaker, Koşu, Basketbol, Yürüyüş, Outdoor, Halı saha, Terlik & Sandalet, Bot, Mont... |
| `beden_sistemi` | enum | EU, EU-adidas (1/3), US, UK |
| `beden_eu_norm` | ondalık | Ondalık EU değeri (36 2/3 → 36.67) |
| `beden_filtre_grubu` | tam sayı | EU'nun tam kısmı: 41, 41⅓, 41.5 → 41 (markalar arası karşılaştırma için) |
| `beden_cm` | ondalık | Marka tablosundan |
| `kalip` | enum + metin | dar / normal / geniş + not ("Yarım numara büyük al") |
| `stil_kodu` | metin | Üretici kodu (ör. U9060EEE) |
| `malzeme_ust`, `malzeme_taban`, `kapanis` | metin | Künye |
| `varyant_fiyat` | para | Beden bazlı fiyat (mevcut `data-variant-price`) |
| `onceki_fiyat_ref` | para | İndirim gösterimi için yasal referans: indirimden önceki son 10 günün en düşük fiyatı (1 Ağustos 2026 kuralı; [[Türkiye E-ticaret Pazarı]]) |

- Ürün adındaki notlar (ör. "(2 numara büyük alınması tavsiye edilir.)") `kalip` alanına taşınır.
- Renk ve kategori temizliği için bir eşleme tablosu yazılır; küçük harf dönüşümü yerel ayardan bağımsız (`mb_strtolower($s, 'UTF-8')`), mevcut "whıte" hatası giderilir.
- Ayrıntı: [[Ayakkabı Beden ve Kalıp]].

## 4. Sayfa bazlı gereksinimler ve kabul kriterleri

### Global (header, footer, çerez)
- Spesifikasyon: [[Header ve Navigasyon]], [[Footer]], [[Güven Sinyalleri]].
- **Kabul:** masaüstü menüde `Yeni gelenler · Erkek · Kadın · Çocuk · Markalar` var; mobil menü 20/20 denemede tek dokunuşla açılıp kapanıyor (iOS Safari + Android Chrome); duyuru şeridi değer önerisi gösteriyor; çerez seçimi sayfayı yenilemiyor; footer'da yasal linkler ve iletişim bilgisi var.

### Ana sayfa
- Bölüm sırası: duyuru şeridi → hero (≤1 ekran, tek mesaj, tek birincil buton) → kitle/kategori karoları (Erkek, Kadın, Çocuk, Yeni gelenler) → "Numaranla başla." (kompakt, seçilen beden hatırlanır) → öne çıkan modeller (3–4 kart) → yeni gelenler ürün ızgarası (8) → marka karoları (logo) → kampanya bandı (varsa) → hizmet şeridi → footer. Spesifikasyon: [[Hero ve Banner Desenleri]].
- **Kabul:** otomatik dönen öğe yok; ilk ekranda en az bir kategori girişi görünüyor (390×844 ve 1440×900'de); hero görseli `<img>` + `fetchpriority="high"`, ≤250 KB; mobil LCP < 2,5 sn (Lighthouse mobil).

### Kategori sayfası (PLP)
- Spesifikasyon: [[Kategori Sayfası ve Filtreler]].
- **Kabul:** beden, renk, marka, kategori filtreleri çoklu seçimli; masaüstünde seçim ≤400 ms içinde sonuçları güncelliyor (sayfa yenilemeden, URL güncelleniyor); sıralama seçimle uygulanıyor (buton yok); uygulanan filtreler çip olarak görünüyor; renk filtresinde ≤15 aile; "Ayakkabı" grubunda giyim/oyun kartı kategorileri çıkmıyor; geri tuşu filtre ve kaydırma konumunu koruyor.

### Ürün sayfası (PDP)
- Spesifikasyon: [[Ürün Sayfası]], [[Beden ve Kalıp]].
- **Kabul:** beden seçilince fiyat anında güncelleniyor ve `aria-live` ile duyuruluyor; seçimden önce fiyat aralığı görünüyor; tüm beden aralığı görünüyor, tükenenler soluk + "Gelince haber ver"; kalıp notu beden ızgarasının yanında; butonun altında teslim/iade/taksit/orijinallik satırları; adet seçici yok; mobilde sticky alt çubuk; açıklama + künye dolu; en az 6 görsel, 4:5; `Product` JSON-LD ve OG etiketleri mevcut.

### Arama
- Spesifikasyon: [[Arama]].
- **Kabul:** "sambá", "SAMBA", "samba og" aynı sonuçları veriyor; "nıke" → Nike; sıfır sonuçta öneriler var; panel açılmadan arama görselleri yüklenmiyor.

### Sepet ve ödeme
- Spesifikasyon: [[Sepet ve Ödeme]].
- **Kabul:** sepete eklenince mini sepet çekmecesi açılıyor; adet değişikliği otomatik; toplam KDV dahil ve kargo açık; misafir ödeme var; ödeme formu `autocomplete` ve doğru klavye türleriyle; yasal onaylar ve sipariş butonu metni mevzuata uygun ([[Türkiye E-ticaret Pazarı]]).

## 5. Teknik notlar

- URL: `/erkek/sneaker`, `/new-balance-9060-sea-salt-u9060eee` gibi slug yapısı; eski `index.php?route=...` adreslerinden 301 yönlendirme.
- CSS: 8 dosya → 1 dosya + kritik CSS; token'lar CSS değişkeni ([[Tasarım Token Önerisi]]).
- JS: tek bir header/menü modülü (mevcut `store.js` ve `atelier-commerce.js` çakışmasını kaldır); filtreler için fetch + `history.replaceState`.
- Görseller: AVIF/WebP + JPEG fallback, `srcset` (400/800/1200/1600), `loading="lazy"` (ilk ekran hariç), `width`/`height` öznitelikleri.
- Fontlar: Manrope değişken woff2, preload, `font-display: swap`.
- Analitik olayları: `view_item_list`, `select_item`, `view_item`, `select_size`, `add_to_cart`, `view_cart`, `begin_checkout`, `purchase`, `filter_apply`, `search`, `notify_me` (çerez onayına bağlı).

## 6. Test kontrol listesi

- [ ] Lighthouse mobil: Performans ≥ 90, Erişilebilirlik ≥ 95, SEO ≥ 95 (yayında)
- [ ] axe-core: 0 ciddi/kritik ihlal (ana sayfa, PLP, PDP, sepet, ödeme)
- [ ] Klavye ile: menü → PLP filtre → PDP beden seç → sepete ekle → ödemeye geç
- [ ] Gerçek cihaz: iOS Safari, Android Chrome (menü, filtre çekmecesi, sticky çubuk, galeri)
- [ ] Beden bazlı fiyat: PDP fiyatı = mini sepet = sepet = ödeme özeti
- [ ] Türkçe karakter: başlıklarda büyük harf "İ" doğru, aramada eşdeğerlik
- [ ] 390, 768, 1024, 1440 px genişliklerde yatay kaydırma yok

## 7. Referans haritası

| Soru | Not |
|---|---|
| Şu an ne var, ne bozuk? | [[KPT Store Denetimi]] |
| Hangi renk/font/boşluk? | [[Tasarım Token Önerisi]], [[Renk ve Tipografi]] |
| Bileşen nasıl olmalı? | `03 Desen Kütüphanesi` |
| Neden böyle? (kanıt) | [[Satın Alma Psikolojisi]], [[E-ticaret UX Verileri]], [[Dönüşüm Vaka Çalışmaları]] |
| Türkiye'ye özgü ne var? | [[Türkiye E-ticaret Pazarı]], [[Trendyol]], [[Türkiye Sneaker Mağazaları]] |
| Beden nasıl modellenir? | [[Ayakkabı Beden ve Kalıp]] |
| Rakipler nasıl yapıyor? | [[Rakip Karşılaştırma Matrisi]] |
| Sırayla ne yapılacak? | [[Yapılacaklar Listesi]] |
