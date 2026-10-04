---
tür: rakip-analizi
site: Zalando
url: https://www.zalando.co.uk/
ülke: UK (merkez DE)
segment: büyük ölçekli moda pazar yeri / platform
erişim: engellendi
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.zalando.co.uk/ (502), https://www.zalando.co.uk/mens-shoes-trainers/ (403), https://www.zalando.co.uk/faq/ (WebFetch, herkese açık yardım sayfası)]
etiketler: [rakip, moda-platformu, beden-kalip]
---

# Zalando

> [!summary] Özet
> Zalando, Berlin merkezli, 30 Avrupa pazarında 62 milyon aktif kullanıcıya satış yapan Avrupa'nın en büyük moda platformu (Wikipedia, 2026). Site tarayıcıyla incelenemedi. Bu not **ikincil kaynaklara**, özellikle Zalando mühendislerinin yazdığı **SizeFlags** makalesine (KDD 2021) dayanıyor. En değerli ders şu: **ürün bazlı "dar kalıp / geniş kalıp" uyarısı, kişisel beden önerisinden daha fazla iade azaltıyor.** Ayakkabıda boyuta bağlı iadeleri %3,8, tekstilde %4,3–6,6 azalttı. Kişiselleştirilmiş öneri ise dönüşümü %2,1 artırdı ama iadeyi anlamlı ölçüde azaltmadı (Nestler vd., 2021). KPT için uygulaması en kolay ve en yüksek getirili beden deseni bu.

> [!warning] Erişim notu
> Ana sayfa proxy üzerinden HTTP 502 "upstream request failed" döndürdü. Erkek sneaker PLP'si HTTP 403 ve Zalando'nun "Site can't be reached right now" engel sayfasını gösterdi. Kurallar gereği aşılmaya çalışılmadı. **Header, ana sayfa, PLP filtreleri, PDP ve sepet tarayıcıda gözlenemedi.** Aşağıda "Gözlem" diye işaretlenmeyen her bilgi ikincil kaynaktır.

## Kimlik ve konumlandırma
- Ekim 2008'de Berlin'de kuruldu. 30 Avrupa pazarında ve 62 milyon aktif kullanıcıya hizmet veriyor (Temmuz 2026). Gelir 2024'te 10,6 milyar €, 2025'te 12,3 milyar € (Wikipedia, 2026).
- Rakibi About You'yu 2025'te satın aldı (1,13 milyar €, Wikipedia, 2026).
- **İade politikası değişikliği:** 2025'te Almanya, Hollanda ve İtalya'da ücretsiz iade süresi 100 günden 30 güne indi (Wikipedia, 2026). UK yardım sayfası da "30-day return policy" diyor.

## Görsel dil
**Gözlem (yalnızca engel sayfasından, sınırlı):**
| Rol | Hex | Kullanım yeri |
|---|---|---|
| Birincil buton | `#000000` zemin / `#FFFFFF` metin | "Refresh" butonu |
| İkincil buton | şeffaf zemin, `#000000` metin ve çerçeve | "Send error report" |
| Sayfa zemini | `#EFEFF0` | Hata sayfası gövdesi |
| Header zemini | `#FFFFFF` | Logo şeridi |

- Font ailesi **HelveticaNow**. Başlık 32px, gövde 16px / 400.
- Butonlar 203×48px ve 0px radius. Birincil dolgulu, ikincil çerçeveli, yan yana eşit genişlikte duruyor.
- Bunun dışındaki renk, tipografi ve fotoğraf stili incelenemedi.

## Header ve navigasyon
Tarayıcıda incelenemedi. Yardım sayfasının metninden (WebFetch) alınan değer önerileri:
- **"Free standard delivery over £39.00 & free returns\*"**
- **"30-day return policy"**
- Yardım menüsünde "Find the right size" başlığı ayrı bir konu olarak duruyor (beden, yardımın ana konularından biri).
- Footer'daki ödeme linkleri: Mastercard, Visa, PayPal, Apple Pay.

## Ana sayfa ve banner/hero örnekleri
incelenemedi: ana sayfa 502 döndürdü.

## Kategori sayfası (PLP)
incelenemedi: 403 engeli. Elimizde yalnızca dolaylı veri var:
- Baymard, zalando.co.uk'yi Eylül 2016'dan beri 20 kez benchmark etmiş (son inceleme Temmuz 2024, 574 tasarım öğesi). **Masaüstü "Product List + Filtering" bölümünde 21 olumlu ve 16 olumsuz bulgu**, mobil PLP'de 16 olumlu ve 11 olumsuz bulgu var (Baymard Institute, 2024). Bulguların içeriği ücretli. Yani bu skor, filtre UX'inin kusursuz olmadığını gösteriyor.
- Filtre türleri (beden ızgarası, renk örnekleri, çipler, sonuç sayısı) **doğrulanamadı**. Bu nedenle bu notta Zalando filtresi için ölçü verilmiyor. Filtre desenleri için [[Kategori Sayfası ve Filtreler]] notuna bakın.

## Ürün sayfası (PDP)
Tarayıcıda incelenemedi. Baymard verisi: masaüstü "Product Page + Video & 360-Views" bölümünde 33 olumlu ve 18 olumsuz, mobil PDP'de 31 olumlu ve 20 olumsuz bulgu (Baymard Institute, 2024).

### Beden ve kalıp: SizeFlags (ikincil kaynak, en önemli bölüm)
Kaynak: Nestler, Karessli, Hajjar, Weffer, Shirvany (Zalando SE), *SizeFlags: Reducing Size and Fit Related Returns in Fashion E-Commerce*, KDD 2021.

- **Ne yapıyor:** Her ürün için "too small" (normalden küçük kalıyor) veya "too big" (normalden büyük kalıyor) bayrağı üretiyor ve PDP'de bunu müşteriye **beden tavsiyesi** olarak gösteriyor. Bayrak, ürünün kendi iade nedenlerinden ("çok küçük" / "çok büyük") hesaplanıyor. Yeni üründe veri yokken görsel analiz ve uzman etiketleri ön bilgi olarak kullanılıyor.
- **Tasarım felsefesi:** Kişiye "senin bedenin 43" demek yerine **ürün hakkında bilgi veriyor**. Makaleye göre bu yaklaşım bilişsel yükü düşük tutuyor. Kişisel öneri ise yanlış hissedildiğinde tamamen görmezden gelinme riski taşıyor. Müşteri kendi tercihine göre karar veriyor.
- **Ölçek:** Bayesci sürüm 2020 başında yayına girdi, 14 ülkede milyonlarca ürün için kullanılıyor.
- **Sonuçlar (A/B testleri, 2017):**

| Test | Örneklem | Sonuç |
|---|---|---|
| Ayakkabı (kadın + erkek) | Grup başına 720 bin müşteri | Bedene bağlı iade oranı **%3,8** (göreli) azaldı |
| Ayakkabı, yan etki | aynı | Aynı üründen 2+ beden sipariş etme oranı "too small" uyarısında **%11,1**, "too big" uyarısında **%19,0** arttı |
| Tekstil | Grup başına 180 binden fazla müşteri | Bedene bağlı iade "too small"da **%4,3**, "too big"da **%6,6** azaldı. Müşteriler "büyük kalıyor" uyarısına daha güçlü tepki veriyor |
| Kişiselleştirilmiş beden önerisi (karşılaştırma) | iki ardışık canlı test | Dönüşüm **+%2,1**, sepete ekleme **+%1,8**, ziyaret başına gelir **+%2,1**. Bedene bağlı iadede anlamlı azalma yok (**<%0,5**) |

- Makalenin aktardığı sektör verisi: online modada iade oranı genel olarak **%25–40**, bazı kategorilerde **%75'e** kadar çıkıyor (Nestler vd., 2021, literatürden).
- İnsan geri bildirimi (uzman etiketi) eklenince bayrak **%33 daha hızlı** açılıyor, yani daha az iade yaşanmadan uyarı devreye giriyor.

> [!warning] Doğrulanamayan
> Zalando sitesinde uyarının tam metni (örn. "We recommend ordering one size up") bu incelemede görülemedi. Aşağıdaki Türkçe metinler **KPT için önerilen** metinlerdir, Zalando alıntısı değildir.

## Sepet ve satın alma kolaylığı
Sepet incelenemedi. İletişim biçimi: ücretsiz kargo eşiği ve ücretsiz iade **tek cümlede** veriliyor ("Free standard delivery over £39.00 & free returns\*"). Yıldız işareti koşulları dipnota bırakıyor.

## Mobil deneyim
incelenemedi.

## Güven ve ikna unsurları
| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| Eşikli ücretsiz kargo ve ücretsiz iade tek satırda | Site geneli şerit / yardım | Hedef gradyanı, risk azaltma | Evet |
| Ürün bazlı kalıp uyarısı | PDP | Belirsizliği azaltma, düşük bilişsel yük | Evet, öncelikli |
| "Find the right size" yardım başlığı | Yardım merkezi | Yetkinlik desteği | Evet: "Numaramı nasıl bulurum?" sayfası |
| Çoklu ödeme (PayPal, Apple Pay, kart) | Footer | Sürtünmeyi azaltma | Türkiye karşılığı: taksit, Troy, havale |

## Performans ve teknik gözlem
Engel sayfası 403 döndü. Akamai/bot koruması headless Chromium'u ayırt ediyor. Başka ölçüm yapılamadı.

> [!example] ASOS ile kısa kıyas (ASOS da engellendi, bu yüzden ayrı not yok)
> Baymard'a göre (asos.co.uk, son inceleme Mart 2026, 901 tasarım öğesi) ASOS'un masaüstü "Product List + Filtering" bölümünde de **21 olumlu / 16 olumsuz** bulgu var. "Sorting Tool" masaüstü ve mobilde **0 olumlu / 2 olumsuz**. "Size Finder" **0 / 1**. Mobil web ve uygulamadaki "Added To Cart Confirmation" ise **0 olumlu / 1 olumsuz** (Baymard Institute, 2026). Yani iki dev bile sıralama ve sepete ekleme geri bildiriminde kusurlu. ASOS, Ekim 2024'ten itibaren **£3,95 iade ücreti** almaya başladı ve tutarsız kalıplardan şikâyet eden müşterilerden tepki gördü (Wikipedia/BBC, 2024).

## Güçlü yanlar / Zayıf yanlar
- **Güçlü:** Bilimsel olarak test edilmiş kalıp uyarısı sistemi. Net değer önerisi (£39 eşiği ve ücretsiz iade). Bedene ayrı yardım konusu.
- **Zayıf:** PLP/filtre bölümünde Baymard'ın 16 olumsuz bulgusu. İade süresinin 100 günden 30 güne kısaltılması (DE/NL/IT) cömert iade algısını zayıflattı. Bot koruması yüzünden dış denetim zor.

## KPT için çıkarımlar
- **Uygula:**
  - **PDP'de beden ızgarasının hemen üstüne kalıp satırı ekle.** Üç durum olsun:
    - Normal: "Kalıp: Standart, kendi numaranı seç." (ikon: ✓, renk `#171B1C`)
    - Dar: "Kalıp: Dar. Normal numaranın yarım/bir numara büyüğünü öneriyoruz." (zemin `#F3F4F1`, sol kenarda 3px `#741E32` şerit)
    - Geniş: "Kalıp: Geniş. Bir numara küçüğünü öneriyoruz."
    - Metin 14px Manrope 500, kutu 12px iç boşluklu, radius 4px.
  - Veri modeli: OpenCart ürününe `kalip` alanı ekle (`dar` / `standart` / `genis`, varsayılan `standart`). İlk aşamada marka ve model bilgisiyle elle doldur. Sonraki aşamada iade formuna zorunlu "İade nedeni: Küçük geldi / Büyük geldi / Beğenmedim / Diğer" seçimini ekle. Bir modelde "küçük geldi" iadeleri kategori ortalamasını belirgin biçimde aşınca (SizeFlags mantığı) bayrağı öner.
  - Üst şeritte eşik ve iadeyi tek cümlede ver: "X TL üzeri ücretsiz kargo · 14 gün ücretsiz iade". Aynı cümleyi PDP'deki "Sepete Ekle" butonunun altında 13px metin olarak tekrarla.
- **Uyarla:**
  - SizeFlags testinde "bir numara büyük al" uyarısı müşterileri **iki beden birden sipariş etmeye** itti (+%11–19). KPT'de buna karşı uyarının altına "Emin değil misin? Değişim ücretsiz" satırı ekle. Böylece müşteri iki çift yerine bir çift alır ve gerekirse değiştirir.
  - Kişiselleştirilmiş "senin numaran 43" önerisini daha sonra, giriş yapmış ve geçmiş siparişi olan kullanıcılar için ekle (dönüşüme +%2,1 etkisi var, iadeye değil).
- **Kaçın:**
  - Kalıp bilgisini yalnızca beden rehberi modalına gömmek. Uyarı, beden seçilmeden önce görünür olmalı.
  - Kuralları belirsiz yıldızlı vaatler: "ücretsiz iade\*" kullanıyorsan koşulu aynı satırda yaz.
  - İade süresini sessizce kısaltmak. Değişiklik varsa açıkça duyur.

İlgili desenler: [[Beden ve Kalıp]], [[Ürün Sayfası]], [[Kategori Sayfası ve Filtreler]], [[Güven Sinyalleri]], [[Sepet ve Ödeme]], [[E-ticaret UX Verileri]], [[Satın Alma Psikolojisi]], [[KPT Store Denetimi]].

## Ekran görüntüleri
Kasaya eklenmedi: yalnızca hata/engel sayfaları görüldü.

## Kaynaklar
- Nestler, A., Karessli, N., Hajjar, K., Weffer, R., Shirvany, R. (2021). *SizeFlags: Reducing Size and Fit Related Returns in Fashion E-Commerce.* KDD '21. https://arxiv.org/abs/2106.03532
- Zalando UK yardım sayfası (WebFetch, 2026-10-04): https://www.zalando.co.uk/faq/
- Baymard Institute, Zalando UX case study (son inceleme Temmuz 2024): https://baymard.com/ux-benchmark/case-studies/zalando
- Baymard Institute, ASOS UX case study (son inceleme Mart 2026): https://baymard.com/ux-benchmark/case-studies/asos
- Wikipedia, "Zalando" (erişim 2026-10-04): https://en.wikipedia.org/wiki/Zalando
- Wikipedia, "ASOS plc" (erişim 2026-10-04, BBC 2024'e atıfla): https://en.wikipedia.org/wiki/ASOS_plc
- Engellenen denemeler: https://www.zalando.co.uk/ (502), https://www.zalando.co.uk/mens-shoes-trainers/ (403)
