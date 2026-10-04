---
tür: araştırma
konu: E-ticarette belgelenmiş A/B testleri ve dönüşüm vakaları (moda/sneaker öncelikli)
güncellik: 2026-10-04
vaka-sayısı: 81
etiketler: [araştırma, dönüşüm, ab-test, cro, sneaker, moda]
---

# Dönüşüm Vaka Çalışmaları

Kod ajanları için "hangi değişiklik ne kadar etki yaptı" veri notu. Bağlam: [[KPT Store Denetimi]], [[E-ticaret UX Verileri]], [[Satın Alma Psikolojisi]].

> [!summary] En etkili 15 değişiklik
> 1. **Hız:** LCP -%31 → satış +%8 (Vodafone). 100 ms → gelir +%0,7 (Zalando). **Güçlü**
> 2. **PLP→PDP prerender:** CR mobilde +%101, masaüstünde +%156 (Ray-Ban). **Orta**
> 3. **0→5 yorum:** Satın alma olasılığı +%270 (Spiegel). **Güçlü**
> 4. **Beden önerici:** CR +%3,4, iade -%13,6 (Foot Locker EU). **Orta**
> 5. **Misafir ödeme:** Satın alan müşteri +%45. **Orta**
> 6. **Checkout düzeltmeleri:** +%35 potansiyel (Baymard). **Güçlü**
> 7. **Apple Pay:** CR +%22,3 (Stripe). **Orta**
> 8. **BNPL/taksit:** Satış +%20 (JFE 2025). **Güçlü**
> 9. **Teslim tarihi:** CR +%22,4 (Rylee + Cru). **Zayıf**
> 10. **Sticky ATC:** Medyan +%5,1. İçinde varyant seçiciyle ATC +%75. **Orta**
> 11. **Kargo eşiği CTA yanında:** Satın alma +%90 (NuFace). **Orta**
> 12. **360° görüntüleyici:** Ayakkabıda işlem +%16 (Nubikk). **Orta**
> 13. **Büyük görsel:** Satış +%9,5 (Mall.cz). **Orta**
> 14. **Çoklu filtre:** CR +%8,7, AOV -%9. **Zayıf**
> 15. **"0" sayılı paylaşım butonlarını kaldırmak:** ATC +%11,9. Checkout sayacı ise CR -%3–4. **Orta/Zayıf**

**Güvenilirlik:**
- **Güçlü:** Hakemli çalışma, yöntemi açık büyük A/B testi ya da Baymard.
- **Orta:** Adı verilen şirkette A/B testi; kaynak satıcı veya ajans.
- **Zayıf:** Vendor iddiası, yöntemsiz, önce/sonra ya da seçim yanlılığı.
- **"(özet)":** Kaynakta doğrulanamadı.

Yüzdeler göreli değişimdir.

## Vaka tabloları

### Sticky sepete ekle — [[Mobil Deneyim]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V01 | Sticky CTA, 26 testin meta-analizi | GoodUI #41 | Medyan satış +%5,1, ilerleme +%2,8 | 2026 | GoodUI (özet) | Orta |
| V02 | Mobil sticky ATC, butonda fiyat | AFTCO, giyim | CR +%6,2, RPV +%3,6, AOV -%2,5 | ~2025 | Clean Commit | Orta |
| V03 | Sticky ATC ve içinde varyant seçici | Füm, DTC | ATC +%75, RPV +%15. Sticky tek başına ATC +%6 | 2024 | Single Grain | Orta |
| V04 | ATC'yi altta sabitlemek | U-Digital | Sepete tıklama +%21,5 (7.200 ziyaretçi) | 2020 | VWO | Orta |
| V05 | Sticky ATC altta | Little Bible Stories | CR +%7, **mobil RPV -%18** | ~2025 | Blend | Zayıf |
| V06 | Yüzen satın alma kutusu | Etsy | 2 ay sonra reddedildi | — | GoodUI leak #98 | Orta |

### Checkout ve ödeme — [[Sepet ve Ödeme]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V07 | "Register" yerine "Continue" | Büyük ABD perakendecisi | Satın alan +%45, ilk yıl +300 M $ | 2009 | UIE | Orta |
| V08 | Checkout'tan "kayıt" ifadeleri kaldırıldı | ASOS | Yarıda bırakma -%50 | ~2010'lar | QueryClick | Zayıf |
| V09 | Bırakma nedenleri | Baymard | Zorunlu hesap %18, uzun checkout %17 | 2025 | Baymard | Güçlü |
| V10 | Checkout UX potansiyeli | Baymard | CR +%35,26. 23,48 form öğesine karşılık ideal 12–14 | 2025 | Baymard | Güçlü |
| V11 | Tek sayfa ve çok adımlı checkout | Vancouver 2010 Olimpiyat mağazası | +%21,8 (606 işlem). Baymard'a göre adım değil alan sayısı belirleyici | 2010 | Elastic Path (özet) | Zayıf |
| V12 | Apple Pay sunmak | Stripe holdback | CR +%22,3, gelir +%22,5. Yerel ödeme yöntemleri CR +%7,4 | 2025 | Stripe | Orta |
| V13 | Shop Pay | Shopify | Misafir ödemeye göre +%50'ye kadar | 2023 | Shopify | Zayıf |
| V14 | Çekmecede ekspres ödeme butonları | Singular Sound | CR +%35,4, RPV +%56,8 (13 gün) | ~2025 | Blend | Orta |
| V15 | Sepet çekmecesi ve ödül çubuğu | "Moda mağazası" | Checkout +%12. **Rakamlar "temsili"** | ~2026 | Cartylabs | Zayıf |

### Kargo eşiği ve teslim tarihi — [[Güven Sinyalleri]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V16 | "Free shipping over $75!" CTA'nın üstünde | NuFace | Satın alma +%90, AOV +%7,3 | ~2014 | VWO | Orta |
| V17 | Minicart'ta kargo ilerleme çubuğu | İsimsiz Shopify mağazası | AOV +%9,2, **CR -%5,9**, RPV +%3,2 | 2025 | Clean Commit | Zayıf |
| V18 | Sepette ilerleme çubuğu (£175) | Lüks giyim | Gelir +%2, masaüstü işlem +%7 (4 hafta) | 2025 | Webtrends | Orta |
| V19 | PDP'de tek bağlamsal kargo mesajı | Marsh Wear, giyim | **CR -%5,5, RPV -%9** | 2026 | Clean Commit | Zayıf |
| V20 | Bırakma nedenleri | Baymard | Ek maliyet %40, yavaş teslimat %20, toplam görünmüyor %12 | 2025 | Baymard | Güçlü |
| V21 | PDP, sepet ve checkout'ta teslim tarihi | Rylee + Cru, çocuk giyim | CR +%22,4, yeni ziyaretçi +%37,3 | ~2025 | Shoplift | Zayıf |
| V22 | Teslimat bilgisi ekranın ilk görünen kısmında | İngiliz banyo perakendecisi | Gelir +%5, ATC +%4 | — | SiteSpect (özet) | Zayıf |

### Taksit / BNPL — [[Türkiye E-ticaret Pazarı]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V23 | BNPL sunmak | Berg ve ark. | Satış +%20 | 2025 | JFE/NBER | Güçlü |
| V24 | Klarna on-site mesajı | Indochino, giyim | AOV +%16 | 2021 | FashionUnited | Zayıf |
| V25 | Afterpay reklamları | Afterpay iş ortakları | Sipariş +%15. Afterpay kullananların AOV'si +%28 | 2022–23 | SmartCompany | Zayıf |
| V26 | Türkiye'de kartla e-ticarette taksit payı | BKM/GÖSAŞ | %34,4 veya %57,8 (kaynakta iki rakam, tanım belirsiz) | 2025 | Capital | Orta |

### Yorumlar — [[Ürün Sayfası]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V27 | 0→5 yorum | Hediye perakendecisi (15,5 M görüntüleme) | Satın alma olasılığı +%270 (ucuz üründe +%190, pahalıda +%380). Zirve 4,0–4,7 yıldız | 2017 | Spiegel | Güçlü |
| V28 | "Doğrulanmış alıcı" rozeti | 122 bin yorum | Satışa olumlu etki | 2017 | Spiegel | Güçlü |
| V29 | UGC'ye bakanlar ile bakmayanlar | Yotpo (163 M sipariş) | +%161, giyimde +%207 | 2018 | Yotpo | Zayıf |
| V30 | Yorum galerisiyle etkileşim | PowerReviews | CR +%110,7 | ~2023 | PowerReviews | Zayıf |
| V31 | Yotpo yorumları | Princess Polly | CR +%498 | — | Yotpo (özet) | Zayıf |

### Beden önerici — [[Beden ve Kalıp]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V32 | Fit Finder ile statik tablo A/B (500 bin+, 6 ay) | **Foot Locker EU** | CR +%3,38, iade -%13,55 | 2026 | Fit Analytics | Orta |
| V33 | Aynı test | **SIDESTEP** | CR +%13,04, iade -%6,61 | 2026 | Fit Analytics | Orta |
| V34 | Aynı test | **Runners Point** | CR +%5,82, iade -%7,39 | 2026 | Fit Analytics | Orta |
| V35 | Fit Finder A/B (645 bin, 2 ay) | **SNIPES** | CR +%3, iade -%2, çoklu beden siparişi -%8 | 2026 | Fit Analytics | Orta |
| V36 | Fit Finder | Weird Fish | CR +%8 (kullananlarda) | — | Fit Analytics | Zayıf |
| V37 | Fit Finder | THE ICONIC | CR +%1 | — | Fit Analytics | Zayıf |
| V38 | Fit Finder | Mammut, Breuninger, ARMEDANGELS | CR +%22 / +%40 / +%29,9 | — | Fit Analytics | Zayıf |
| V39 | True Fit | M&Co | CR +%1,5, iade -%9,8 | 2019 | BusinessWire | Zayıf |
| V40 | True Fit ortalaması | True Fit müşterileri | CR +%2 | ~2025 | True Fit | Zayıf |
| V41 | Beden/kalıp araçları | **Zalando** | Bedenle ilgili iadelerin %8'i önlendi (2025). 2023'te -%10. Sanal kabin pilotunda -%40'a kadar | 2023–26 | Zalando | Orta |

### Görsel, video, 360° — [[Ürün Sayfası]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V42 | Büyük görsel, açıklama hover'da | Mall.cz | Satış +%9,46 | ≤2019 | VWO | Orta |
| V43 | 3D/360° görüntüleyici (24 ürün, 36 gün) | **Nubikk, ayakkabı** | İşlem +%16, mobil +%18,7, ATC +%10,9. Masaüstü anlamsız | 2023 | Fibbl | Orta |
| V44 | 360° görünüm (10 bin ziyaretçi) | **SoftMoc, ayakkabı** | ATC +%150 | ~2014 | Ortery | Zayıf |
| V45 | Demo videoları | **Zappos** | Satış +%6–30 | ~2009 | Retail Dive (özet) | Zayıf |
| V46 | Ölçek görseli | Baymard | Kullanıcıların %42'si boyutu görsellerden anlamaya çalışıyor | 2017 | Baymard | Güçlü |
| V47 | Bilgiler akordeonda, özellikler kartlarda | AFTCO | CR +%15,7, RPV +%19,7 | 2026 | Clean Commit | Zayıf |
| V48 | Kullanım görselleri galeride geriye itildi, beden bulucu küçültüldü | Spor ürünü | **RPV -%10, CR -%9** | 2026 | Clean Commit | Zayıf |

### Filtre ve arama — [[Kategori Sayfası ve Filtreler]], [[Arama]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V49 | Çoklu seçim, beden/renk/stok filtreleri, aktif çipler | İsimsiz mağaza | CR +%8,7, **AOV -%9**, RPV -%1,5 | 2026 | Clean Commit | Zayıf |
| V50 | Koleksiyonda tıklanabilir beden butonları | İsimsiz mağaza | CR %0 | ~2026 | Clean Commit | Zayıf |
| V51 | Alt kategori kartları | İsimsiz mağaza | CR -%2,2 | ~2026 | Clean Commit | Zayıf |
| V52 | Liste/filtre kullanılabilirliği (344 site) | Baymard | Bırakma vasat sitede %67–90, iyi sitede %17–33 | 2025 | Baymard | Güçlü |
| V53 | Arama sorgu desteği | Baymard | Sitelerin %41'i 8 temel sorgu türünü desteklemiyor | 2024 | Baymard (özet) | Orta |
| V54 | Dynamic Re-ranking A/B | **END. Clothing** | Site CR +%1,47 | ~2023 | Algolia | Orta |
| V55 | Beden stok oranına göre sıralama | **JD Sports** | Koleksiyon CR +%142 (1 hafta) | — | Kimonix | Zayıf |
| V56 | Algolia araması | Under Armour | Arama yapanlarda CR +%35 | 2017+ | Algolia | Zayıf |

### Hero ve kişiselleştirme — [[Hero ve Banner Desenleri]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V57 | Karusel etkileşimi | Notre Dame | ~%1 tıklama, tıklamaların %84'ü 1. slayta | 2013 | Runyon | Orta |
| V58 | Hero'da fayda cümleleri | İsimsiz mağaza | CR +%7,7, RPV +%3,4 | 2026 | Clean Commit | Zayıf |
| V59 | Pop-up'ı 60 saniye geciktirmek | İsimsiz mağaza | CR +%7,9, RPV +%4,8 | 2026 | Clean Commit | Zayıf |
| V60 | Banner altında kişiselleştirilmiş öneriler | Bandier | CR +%9,7 (18 gün) | — | Nosto | Zayıf |
| V61 | Ana sayfa kişiselleştirme | Saks | CR +%9,5 | 2025 | Mastercard (özet) | Zayıf |
| V62 | Story Row | **Footasylum** | CR +%8 (önce/sonra) | 2023 | Storyly | Zayıf |

### Sosyal kanıt ve aciliyet — [[Satın Alma Psikolojisi]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V63 | "Hot item" bannerı, "New Color" etiketi ve 30 dk sayaç (birlikte) | **Foot Locker** Güneydoğu Asya | Mobil PDP CR +%56,5, ATC +%41 | 2026 | Insider | Zayıf |
| V64 | Sepette "yüksek talep" mesajı | İsimsiz mağaza | CR +%2,7 | 2025 | Clean Commit | Zayıf |
| V65 | Sayısı 0 olan paylaşım butonlarını kaldırmak | Taloon | ATC +%11,9 (%95) | 2019 | VWO | Orta |
| V66 | Checkout'ta geri sayım | Enerji şirketi | **CR -%3–4** | ~2024 | Atticus Li | Zayıf |
| V67 | Karanlık desen taraması (11 bin site) | Princeton | 183 site aldatıcı (sahte sayaç/stok) | 2019 | arXiv | Güçlü |

### Sayfa hızı — [[Mobil Deneyim]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V68 | LCP -%31 (SSR, görsel optimizasyonu), A/B | Vodafone | Satış +%8 | 2021 | web.dev | Güçlü |
| V69 | Core Web Vitals A/B | Rakuten 24 | RPV +%53, CR +%33 | 2022 | web.dev | Güçlü |
| V70 | 0,1 sn hızlanma (37 marka) | Deloitte/Google | Perakende CR +%8,4 | 2020 | web.dev | Orta |
| V71 | 100 ms hızlanma, A/B | **Zalando** | Oturum başı gelir +%0,7 | 2018 | Zalando Eng. | Güçlü |
| V72 | LCP etkisi | **Farfetch** | +100 ms'de CR -%1,3. PDP'de LCP -600 ms A/B'de CR +%1–5 | 2022 | web.dev | Güçlü/Orta |
| V73 | Speculation Rules prerender | **Ray-Ban** | CR mobil +%101, masaüstü +%156 | 2025 | web.dev | Orta |
| V74 | LCP -%55, CLS -%91 | Swappie | Mobil gelir +%42 (önce/sonra) | 2021 | web.dev | Orta |

### Güven ve iade — [[Güven Sinyalleri]]
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V75 | Checkout'ta Norton rozeti | buyakilt.com | Sipariş +%17 | ~2012 | Convert (özet) | Zayıf |
| V76 | Norton/VeriSign mührü | USCutter, Blue Fountain | Satış +%11 / +%42 | 2008–11 | Inflow, CrazyEgg | Zayıf |
| V77 | Rozet güven anketi | Baymard | Norton %36, McAfee %23, "fikrim yok" %49 | 2013 | Baymard | Orta |
| V78 | Bırakma nedenleri | Baymard | Güvensizlik %19, iade politikası %13 | 2025 | Baymard | Güçlü |
| V79 | PDP'de iade politikasını vurgulamak | İsimsiz mağaza | **ATC -%3,6** | 2025 | Clean Commit | Zayıf |

### Terk edilen sepet
| # | Değişiklik | Şirket/Sektör | Sonuç | Yıl | Kaynak | Güven. |
|---|---|---|---|---|---|---|
| V80 | E-posta / SMS akışı | Klaviyo (110 bin+ müşteri) | Alıcı başına gelir: e-posta 6,77 $, SMS 4,48 $. Tıklama %6 / %10,3 | 2026 | Klaviyo | Orta |
| V81 | Otomasyon payı | Omnisend (150 bin marka) | Terk edilen sepet ve hoş geldin akışları otomasyon siparişlerinin %76'sı | 2026 | Omnisend | Orta |

## Önceliklendirme matrisi

KPT önizlemede, A/B testi şimdilik yapılamaz. Güçlü/Orta kanıtlı değişiklikler doğrudan uygulanır, Zayıf olanlar canlıda test edilir. Efor değerleri OpenCart için tahmindir.

| Öncelik | Değişiklik | Kanıtlı etki | Kanıt | Efor |
|---|---|---|---|---|
| P0 | Hero'yu AVIF/WebP'ye çevirmek, LCP ≤2,5 sn | 100 ms ≈ +%0,7–1,3 | Güçlü | Düşük |
| P0 | Mobil sticky ATC, içinde numara seçici | +%5 medyan, seçiciyle ATC +%75'e kadar | Orta | Düşük |
| P0 | Tüm numaralar görünür, beden tablosu ve kalıp notu | Beden önericide CR +%3–6, iade -%2…-14 | Orta | Düşük |
| P0 | CTA altında teslimat/iade/taksit satırları | +%4–22. Kargo ve teslimat bırakma nedenlerinde %40 ve %20 | Orta | Düşük |
| P0 | Misafir ödeme, en fazla 8 form alanı | +%45, +%35 potansiyel | Güçlü | Orta |
| P1 | Çoklu filtre, normalize renk, numara ızgarası | CR +%8,7; bırakma %67–90'dan %17–33'e | Güçlü | Orta |
| P1 | Speculation Rules prerender | CR +%101–156 | Orta | Düşük |
| P1 | Yorumlar: doğrulanmış alıcı, fotoğraf, kalıp çubuğu | +%270 | Güçlü | Orta |
| P1 | Fiyatın altında taksit satırı | Satış +%20 | Güçlü | Düşük |
| P1 | En az 6 büyük ürün görseli | +%9,5 | Orta | Orta |
| P2 | Sepet çekmecesi ve ekspres ödeme | +%22–35 | Orta | Orta |
| P2 | Kargo ilerleme çubuğu (**test et**) | AOV +%9, CR -%6 | Zayıf | Düşük |
| P2 | Terk edilen sepet akışı (canlıda) | Alıcı başına 4,5–6,8 $ | Orta | Orta |
| P3 | 360° görüntüleyici, kişiselleştirme, harici beden önerici | +%3–16 | Orta/Zayıf | Yüksek |
| Kaçın | Otomatik karusel, checkout sayacı, sahte stok, sayaçlı paylaşım butonu | ~%1 tıklama, CR -%3–4 | Orta | — |

## Uyarılar

> [!warning] Rakamları beklenen etkinin üst sınırı olarak okuyun

1. **Yayın yanlılığı:** Başarısız testler yayımlanmıyor. Kayıplarını da yayımlayan Clean Commit'in ilk 12 testinin 5'i sıfır veya negatif. GoodUI medyanı +%5, oysa tekil başlıklar +%75–150. KPT için gerçekçi beklenti değişiklik başına **+%1–5**.
2. **Vendor raporları:** Fit Analytics, True Fit, Yotpo, Insider, Klarna, Afterpay, Shopify, Algolia ve Nosto kendi ürününü satıyor. Shopify'ın +%50'sinin yöntemi yok. Cartylabs rakamları "temsili". Aynı satıcıda bile sonuçlar +%1'den (THE ICONIC) +%40'a (Breuninger) uzanıyor.
3. **Seçim yanlılığı:** "Etkileşenler daha çok dönüştü" rakamları (V29–V31, V56) nedensellik göstermez. Niyetli kullanıcı zaten yorum okur ve arama yapar.
4. **Küçük örneklem / kısa süre:** U-Digital 7.200 ziyaretçi, Olimpiyat mağazası 606 işlem. JD Sports 1 hafta, Singular Sound 13 gün sürdü. Nubikk %91,9 kesinlikte. Testler en az 2 hafta sürmeli.
5. **Paket değişiklik:** Foot Locker SEA, Rylee + Cru ve Cartylabs'ta birden çok şey birlikte değişti. Hangi parçanın etkili olduğu bilinmiyor.
6. **Metrik çatışması:** Kargo çubuğu AOV'yi artırıp CR'yi düşürdü. Filtre iyileştirmesi CR'yi artırıp RPV'yi düşürdü. Birincil metrik **RPV** olmalı, AOV ve iade koruma metriği olarak izlenmeli.
7. **Yaş ve pazar farkı:** Bazı vakalar eski ($300M butonu 2009, rozetler 2008–13, Zappos ~2009). Veri çoğunlukla ABD/AB kaynaklı. Türkiye'de taksit ve kargo beklentisi farklı, Apple Pay/Shop Pay verisi doğrudan aktarılamaz (tahmin).

## KPT için uygulama kuralları

Tasarım değerleri: #741E32 bordo vurgu, #171B1C metin, #F3F4F1 / #E5E8E3 zemin, Manrope.

1. **Hız (V68–V73):**
   - Hero AVIF/WebP: masaüstü ≤150 KB, mobil ≤80 KB (tahmin). `fetchpriority="high"`, `width`/`height` belirtilmiş.
   - Alttaki kartlarda `loading="lazy"`.
   - PLP'de `speculationrules` prerender: masaüstü `moderate`, mobilde ilk 4 kart `immediate`.
2. **Sticky ATC (V01–V05):**
   - Ana buton kaybolunca belirir: 64 px + safe-area, #FFFFFF zemin, üstte 1 px #E5E8E3.
   - Solda 40 px görsel ve fiyat.
   - Sağda 48 px #741E32 buton: "Numara Seç" (alttan numara ızgarası açar) veya "Sepete Ekle".
3. **CTA altı blok (V16, V20–V22, V79):** 3 satır, 14 px:
   - "Tahmini teslimat: 9–11 Ekim"
   - "₺X üzeri ücretsiz kargo · 14 gün iade"
   - "Peşin fiyatına 3 taksit"
   - Yalnız gerçek politikalar. Uzun iade metni yok.
4. **Taksit (V23, V26):** Fiyatın altında "veya 3 x ₺1.433" (13 px). Dokununca taksit tablosu açılır.
5. **Numara seçici (V32–V41, V48):**
   - Tüm numaralar 48×48 px hücrelerde. Tükenenler %35 opaklık ve çapraz çizgi.
   - "Beden Tablosu" bağlantısı ve "Kalıp: Normal" notu.
6. **Yorumlar (V27–V28, V65):**
   - 0 yorumda yıldız yok, yerine "İlk yorumu sen yaz".
   - Doğrulanmış alıcı rozeti, fotoğraf, "Dar – Tam – Geniş" çubuğu.
   - Uydurma yorum yok.
7. **Filtreler (V49–V55):** Çoklu seçim, numara ızgarası, ~12 normalize renk, aktif çipler. Mobilde "128 Ürünü Göster" butonu.
8. **Hero (V57–V59):** Statik görsel, karusel yok. Altında fayda şeridi. Pop-up ≥60 sn sonra.
9. **Aciliyet (V63–V67):** Yalnız gerçek stoktan "Bu numaradan son 2 çift". Sayaç, sahte izleyici sayısı, sayaçlı paylaşım butonu yok.
10. **Checkout (V07–V15):**
    - Sağdan çekmece (420 px), toplam ve kargo baştan görünür.
    - "E-posta ile devam et" varsayılan, en fazla 8 alan.
    - Hesap sipariş sonrası önerilir.
    - Kargo çubuğu yalnız A/B testiyle.

## Kaynaklar

- GoodUI #41: https://goodui.org/patterns/41
- Clean Commit (V02, V17, V19, V47–V51, V58, V59, V64, V79): https://cleancommit.io/ab-tests/
  - https://cleancommit.io/ab-tests/sticky-mobile-add-to-cart-button/
  - https://cleancommit.io/ab-tests/visual-free-shipping-progress-indicator
  - https://cleancommit.io/ab-tests/context-aware-shipping-message/
  - https://cleancommit.io/ab-tests/simplified-product-detail-page/
  - https://cleancommit.io/ab-tests/enhancing-trust-and-clarity-on-pdp/
  - https://cleancommit.io/ab-tests/enhanced-collection-filters/
  - https://cleancommit.io/ab-tests/homepage-hero-benefits/
  - https://cleancommit.io/ab-tests/delaying-promo-pop-up-boosts-user-engagement/
  - https://cleancommit.io/ab-tests/scarcity-message-boosts-cart-conversion/
  - https://cleancommit.io/ab-tests/implementing-returns-policy-advertising/
- Füm: https://www.singlegrain.com/wp-content/uploads/2024/05/fum-case-study.pdf
- U-Digital: https://wingify.com/success-stories/udigital/
- Little Bible Stories: https://blendcommerce.com/blogs/ab-tests-shopify/better-placed-sticky-add-to-cart-product-page-conversion
- Singular Sound: https://blendcommerce.com/en-gb/blogs/ab-tests-shopify/adding-express-checkout-in-the-cart-drawer
- $300M Button: https://articles.centercentre.com/three_hund_million_button/
- ASOS: https://www.queryclick.com/blog/guest-checkout-could-it-improve-conversion-rates-this-christmas/
- Baymard checkout: https://baymard.com/lists/cart-abandonment-rate
- Baymard tek sayfa: https://baymard.com/blog/one-page-checkout
- Elastic Path: https://www.elasticpath.com/blog/single-vs-two-page-checkout
- Stripe: https://stripe.com/blog/testing-the-conversion-impact-of-50-plus-global-payment-methods
- Shopify: https://www.shopify.com/enterprise/blog/shopify-checkout
- Cartylabs: https://cartylabs.com/case-studies/fashion-store-cart-abandonment/
- NuFace: https://wingify.com/success-stories/nuface
- Webtrends: https://www.webtrends-optimize.com/blog/case-study-optimising-your-checkout-to-increase-the-average-order-value/
- Rylee + Cru: https://www.shoplift.ai/success-stories/how-fenix-commerce-helped-rylee-cru-increase-conversion-rate
- SiteSpect: https://www.sitespect.com/blog-case-study-ecommerce-updated-pdp-information-increase-sales/
- BNPL JFE: https://www.isb.edu/faculty-and-research/research-directory/the-economics-of-buy-now-pay-later-a-merchant-s-perspective/
- NBER: https://nber.org/system/files/working_papers/w33152/w33152.pdf
- Indochino: https://fashionunited.uk/news/retail/indochino-reveals-results-of-partnering-with-klarna/2021080657215
- Afterpay: https://www.smartcompany.com.au/partner-content/articles/unlocking-merchant-growth-with-afterpay/
- BKM/GÖSAŞ: https://www.capital.com.tr/haberler/tum-haberler/kartli-odemelere-iliskin-guclu-buyume-devam-etti
- Spiegel: https://www.xait.com/hubfs/Spiegel_Online-Review_eBook_Jun2017_FINAL.pdf
- Yotpo: https://www.yotpo.com/blog/increase-conversion-rate-ecommerce/
- Princess Polly: https://www.yotpo.com/case-studies/princess-polly-case-study-reviews/
- PowerReviews: https://www.powerreviews.com/products/ratings-reviews/image-video/
- Fit Analytics Foot Locker EU: https://fitanalytics.com/case-studies/footlocker-eu
- Fit Analytics SNIPES: https://www.fitanalytics.com/case-studies/snipes
- Fit Analytics tüm vakalar: https://fitanalytics.com/case-studies
- M&Co: https://www.businesswire.com/news/home/20191209005017/en/4677272/MCo-Achieves-10-Reduction-Returns-Users-Engage
- True Fit: https://truefit.com/reduce-returns-improve-margins
- Zalando beden: https://corporate.zalando.com/en/node/11013
- Zalando 2023: https://www.mind.eu.com/retail/en/zalando-returns-drop-by-10-thanks-to-sizing-recommendations/
- Mall.cz: https://static.wingify.com/vwo/uploads/2019/03/optimics-product-images-mall-increased-sales_2019-03-18-09-43-38.pdf
- Nubikk: https://fibbl.com/increase-sales-on-your-product-pages-using-a-360-viewer/
- SoftMoc: https://www.ortery.com/case-studies/softmoc
- Zappos: https://www.retaildive.com/news/online-video-the-next-best-thing-to-in-store-shopping/401191/
- Baymard ölçek görseli: https://baymard.com/research-articles/in-scale-product-images
- Baymard ürün listesi: https://baymard.com/research/ecommerce-product-lists
- Baymard arama: https://baymard.com/ecommerce-search/articles
- END.: https://www.algolia.com/customers/END.
- JD Sports: https://kimonix.com/customers/jd-sports
- Under Armour: https://www.algolia.com/customers/under-armour
- Notre Dame: https://www.erikrunyon.com/2013/01/carousel-interaction-stats/
- Bandier: https://www.nosto.com/case-studies/bandier/
- Saks: https://www.mastercard.com/us/en/news-and-trends/Insights/2025/saks-fifth-avenue.html
- Footasylum: https://storyly.io/customer-story/footasylum-opens-shoppertainment-channel-with-storyly-stories
- Foot Locker SEA: https://insiderone.com/case-studies/foot-locker/
- Taloon: https://wingify.com/blog/removing-social-sharing-buttons-from-ecommerce-product-page-increase-conversions/
- Atticus Li: https://www.atticusli.com/blog/posts/stop-adding-urgency-timers-to-your-checkout-the-data-says-youre-wrong/
- Princeton: https://arxiv.org/abs/1907.07032
- Vodafone: https://web.dev/vodafone/
- Rakuten 24: https://web.dev/case-studies/rakuten
- Milliseconds Make Millions: https://web.dev/case-studies/milliseconds-make-millions
- Zalando hız: https://engineering.zalando.com/posts/2018/06/loading-time-matters.html
- Farfetch: https://web.dev/case-studies/farfetch
- Ray-Ban: https://web.dev/case-studies/rayban-speculation-rules
- Swappie: https://web.dev/case-studies/swappie
- buyakilt: https://blog.convert.com/buyakilt-com-lifts-conversions-by-245-percent-using-convert-experiments.html
- USCutter: https://www.goinflow.com/blog/norton-security-seal-increases-ecommerce-conversion-rate-case-study/
- Blue Fountain: https://www.crazyegg.com/blog/trust-seal-ecom
- Baymard rozet: https://baymard.com/blog/site-seal-trust
- Klaviyo: https://www.klaviyo.com/blog/abandoned-cart-benchmarks
- Omnisend: https://www.omnisend.com/2026-ecommerce-marketing-report
