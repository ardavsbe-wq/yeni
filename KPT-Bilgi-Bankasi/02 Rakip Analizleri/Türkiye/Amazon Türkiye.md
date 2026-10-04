---
tür: rakip-analizi
site: Amazon Türkiye
url: https://www.amazon.com.tr/
ülke: TR
segment: global pazar yeri (genel)
erişim: kısmi
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.amazon.com.tr/ (mobil 390px: tam içerik; masaüstü: ara sayfa), https://www.amazon.com.tr/s?k=erkek+sneaker (503), Google Play tanıtım görselleri]
etiketler: [rakip, pazar-yeri, türkiye, jakob-yasası]
---

# Amazon Türkiye

> [!summary] Özet
> Amazon'un Türkiye pazar yeri; Prime ve ertesi gün teslimatla konumlanıyor. Gözlenen en güçlü 3 yanı: fiyat iddiasını dönemle veren rozet ("30 günün en düşük fiyatı"), kuruşu üst simge yapan net fiyat tipografisi, yorumlarda yıldız dağılımı histogramı + "Doğrulanmış Alışveriş" + varyant bilgisi. KPT için en değerli ders: indirim gösteriminde **yüzde rozeti + eski fiyat üstü çizili + dönemli fiyat iddiası** üçlüsü Türk alıcının artık aradığı şeffaflık seviyesi.

> [!warning] Erişim: kısmi
> Mobil (390×844) ana sayfa bir kez tam yüklendi (HTTP 200) ve **[G]** gözlemlerin tamamı bu yakalamadan. Masaüstünde "Alışverişe devam etmek için aşağıdaki düğmeye tıklayın / Alışverişe Devam Et" ara sayfası çıktı (HTTP 202; butona basılmadı); ikinci normal denemede masaüstü ve mobil arama sayfası **"Üzgünüz / İsteğinizi işlemeye çalıştığımızda bir hata oluştu."** (HTTP 503) döndü; WebFetch de 503 aldı. Kural gereği bırakıldı: **PLP ve PDP doğrudan incelenemedi.** **[İ]** = Amazon.com.tr Google Play görselleri (tarihi belirsiz, eski tasarım).

## Kimlik ve konumlandırma
- Ana sayfa başlığı: "Amazon.com.tr: Elektronik, bilgisayar, akıllı telefon, kitap, oyuncak, yapı market, ev, mutfak, oyun konsolları ürünleri ve daha fazlası için internet alışveriş sitesi" [G].
- Google Play açıklaması: "Binlerce üründe geçerli **ertesi gün teslimat** fırsatı", "'Şimdi Al' özelliği ile tek tıkla sipariş" [İ].
- İnceleme günü kampanya bağlamı: "Prime Alışveriş Festivali 5-12 Ekim" [G].

## Görsel dil [G] (mobil ana sayfa, hesaplanmış stiller)
| Rol | Hex | Kullanım yeri |
|---|---|---|
| Ana metin | #0F1111 | Gövde metni (670 düğüm) |
| İkincil metin | #565959 | Açıklama, üstü çizili eski fiyat |
| Link | #2162A1 | "Tüm fırsatları gör", linkler |
| Fırsat kırmızısı | #CC0C39 | "%14 İndirim" rozet zemini, "30 günün en düşük fiyatı" metni |
| Header | #131921 / #232F3E | Üst çubuk / navigasyon şeridi |
| Birincil CTA sarısı | #FFD814 | Çerez "Kabul Et" vb. |
| Açık turuncu | #FEBD69 | Tek öğe; arama "Git" butonu olması muhtemel (tahmin) |
| Açık zemin | #F0F2F2 | Bölüm zeminleri |

- Font: Arial (metin düğümlerinin büyük çoğunluğu), başlıklarda "Amazon Ember Modern Display". Boyutlar: 12px ve 10px (kart metni), 14px, 15px, 18px (raf başlıkları), 24px; ağırlık 400 ve 700.
- Köşe yuvarlaklığı: 8px (en sık), 4px (rozetler), 12–16px (hero kartları).

## Header ve navigasyon [G]
- Üst çubuk: logo ".com.tr" + **"Teslimat konumu: Istanbul 34912 / Konumu güncelle"** (konuma göre teslim tarihi).
- Navigasyon şeridi: Tümü · Günün Fırsatları · Kitap · Çok Satanlar · Günlük İhtiyaçlar · Prime Video · Yeni Çıkanlar · Moda · Prime · Müşteri Hizmetleri · Elektronik …
- Hesap: "Merhaba, Giriş yapın / Hesap ve Listeler", "İadeler ve Siparişler", "0 Alışveriş Sepeti".

## Ana sayfa ve banner/hero örnekleri [G]
- Hero: yatay kaydırmalı, 16px radius kart, sonraki kart sağdan ~90px görünüyor (kaydırma ipucu). Kart 1: **"Fırsatlar yarın başlıyor! Sepetin hazır mı?"** + mavi hap "Prime Alışveriş Festivali 5-12 Ekim" + sarı etiket **"Peşin fiyatına 9 taksit*"** + dipnot "İndirim seçili ürünlerdedir. *Detaylar: amazon.com.tr/taksitler".
- Kart 2: **"Günlük ihtiyaçlara sepette %15 indirim"** / "Prime ol, %20 indirim kazan!" / "1.000 TL üzeri seçili ürünlerde, maksimum 500 TL indirimle sınırlıdır."
- Bölüm sırası (başlıklar birebir): Öne çıkan fırsat ve mağazalar → Sana özel avantajları keşfet → 300 TL'ye sepette 60 TL indirim! → ⭐Haftanın Seçimleri⭐ → İlk siparişinde kargo bedava → peşin fiyatına 9 aya varan taksit fırsatı → Bütçe dostu ürünler → 500 TL bonus fırsatı → Outlet Reyonu → 1000 TL altı fırsatlar → 👕 Moda fırsatları → Amazon'da alışveriş çok kolay → Kişiye özel önerileri görün.
- Fırsat kartı anatomisi: görsel (8px radius) → ad tek satır kesik → **"%14 İndirim"** (beyaz metin, #CC0C39 zemin, 4px radius) → kırmızı kalın **"30 günün en düşük fiyatı"** (varyantlar: "90 günün…", "365 günün en düşük fiyatı") → fiyat **"10.999⁰⁰ TL"** (kuruş üst simge) → gri üstü çizili **"12.800,00 TL"**.
- Raf altı: **"✨İlk siparişinde kargo bedava✨"**.

## Kategori sayfası (PLP)
incelenemedi: 503. Eski Google Play görselinde fırsat listesi: "Filtrele ˅" ve "Sıralama: Amazon sunar ˅" iki açılır, kartta gri "GÜNÜN FIRSATI" etiketi ve yeşil **"Kalan süre: 5:41:18"** [İ].

## Ürün sayfası (PDP)
incelenemedi: 503. Yorum bölümü [İ, eski görsel]: **"Müşteri değerlendirmeleri"**, "★★★★½ 4,7 / 5 yıldız", 5→1 yıldız yatay çubuk histogramı yüzdeleriyle ("5 Yıldız %86"), "Puanlar nasıl hesaplanır?", sıralama açılırı "En çok beğenilen müşteri yorumları", "Filtre »", "51 yorumdan 1-10 arası gösteriliyor", yorumda turuncu **"Doğrulanmış Alışveriş"**, varyant satırı "Renk: Prizma Siyah | Ölçü: 128 GB", "5 kişi bunu faydalı buldu", "Yorum yazın".

## Sepet ve satın alma kolaylığı
incelenemedi. Gözlenen ödeme mesajları [G]: "Peşin fiyatına 9 taksit*", "peşin fiyatına 9 aya varan taksit fırsatı", "İlk siparişinde kargo bedava", sepette indirim eşikleri ("300 TL'ye sepette 60 TL indirim!"). [İ]: "İlk alışverişine 150 TL indirim — *Minimum sipariş tutarı ve diğer koşullar geçerlidir".

## Mobil deneyim [G]
Konum çipi en üstte; hero kartlarında yatay kaydırma ve görünür sonraki kart; çerez penceresi ekranın ~%65'ini kaplıyor, butonlar **"Kabul Et"** (sarı dolgu) · **"Reddet"** (beyaz, çerçeveli) · "Kişiselleştirin" (link); metinde "Bu hizmette çerez kullanan 129 üçüncü taraf" ifadesi.

## Güven ve ikna unsurları
| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| "30 günün en düşük fiyatı" | Fırsat kartı | Fiyat çapası, şeffaflık | Evet, fiyat geçmişi kaydıyla |
| Teslimat konumu çipi | Header | Belirsizlik azaltma | Kısmen: il seçimine göre teslim tahmini |
| Yıldız histogramı | Yorumlar | Şeffaf sosyal kanıt | Evet |
| "Doğrulanmış Alışveriş" | Yorum | Güvenilirlik | Evet |
| "Kalan süre" sayacı | Günün fırsatı | Aciliyet | Yalnızca gerçek bitişte |
| Sepette eşik indirimi | Raf başlığı | Hedef gradyanı | Evet ("1.500 TL'ye 150 TL kaldı") |

> [!warning] Etik değerlendirme
> Dönemli fiyat iddiası ("30 günün en düşük fiyatı") en şeffaf indirim gösterimi; Ticari Reklam Yönetmeliği md. 14 ispat yükünü satıcıya verir (RG 10.01.2015). Geri sayım gerçek kampanya bitişine bağlı olmalı (Ek md. 7). Reddet butonunun Kabul Et ile aynı seviyede sunulması iyi uygulama.

## Performans ve teknik gözlem [G] (mobil ana sayfa)
TTFB 577 ms, DOMContentLoaded 1.818 ms, load 3.177 ms, 300 istek, ~3.695 KB aktarım, 264 görsel (jpg/png; `loading="lazy"` özniteliği 0). Bot koruması yoğun istek sonrası 503 döndürüyor.

## Güçlü yanlar / Zayıf yanlar
- Güçlü: şeffaf fiyat iddiaları, yorum histogramı, konuma dayalı teslim vaadi, okunur fiyat tipografisi.
- Zayıf: ana sayfa kampanya yoğunluğu (20+ raf), moda/ayakkabı keşfi zayıf; tasarım dili jenerik.

## KPT için çıkarımlar
- **Uygula:**
  - İndirimli fiyat bloğu: "%14" rozet (bordo #741E32 zemin, beyaz 12px 700, 4px radius) + güncel fiyat (20px 700, kuruş üst simge) + eski fiyat (14px #565959 üstü çizili). Fiyat geçmişi tutuluyorsa "Son 30 günün en düşük fiyatı" satırı.
  - Yorum özeti: ortalama puan (28px 700) + 5 satırlık yüzde histogramı + "Doğrulanmış alıcı" etiketi + yorumda "Numara: 42 · Renk: Beyaz".
  - Sepette eşik çubuğu: "Ücretsiz kargoya 230 TL kaldı" + ilerleme çubuğu.
  - Çerezde "Reddet"i "Kabul Et" ile eşit görünürlükte sun.
- **Uyarla:** Konum çipini PDP teslim satırına taşı: "İstanbul'a tahmini teslim: 7–8 Ekim" (il seçilebilir).
- **Kaçın:** 20+ kampanya rafı; Arial gibi jenerik tipografi; lazy-load'suz ağır görsel yükü (KPT'nin 900 KB hero sorunu).

## Ekran görüntüleri
![[amazontr-mobil-hero.jpg]]
Mobil ana sayfa [G]: konum çipi, kaydırmalı hero, "Peşin fiyatına 9 taksit*" etiketi ve dipnot.

![[amazontr-mobil-fiyat-rozet.jpg]]
Fırsat kartları [G]: "%14 İndirim", "30/90/365 günün en düşük fiyatı", kuruşu üst simge fiyat ve üstü çizili eski fiyat.

![[amazontr-app-yorumlar.jpg]]
Google Play görseli [İ, eski]: yıldız histogramı, "Doğrulanmış Alışveriş", varyant satırı, "faydalı buldu" sayacı.

## Kaynaklar
- Amazon.com.tr mobil ana sayfa, doğrudan yakalama (2026-10-04): https://www.amazon.com.tr/
- Amazon.com.tr Google Play: https://play.google.com/store/apps/details?id=com.amazon.mShop.android.shopping&hl=tr
- Ticari Reklam ve Haksız Ticari Uygulamalar Yönetmeliği (RG 10.01.2015): https://www.resmigazete.gov.tr/eskiler/2015/01/20150110-5.htm

Bağlantılı notlar: [[Hero ve Banner Desenleri]] · [[Ürün Sayfası]] · [[Sepet ve Ödeme]] · [[Güven Sinyalleri]] · [[Renk ve Tipografi]] · [[E-ticaret UX Verileri]] · [[KPT Store Denetimi]]
