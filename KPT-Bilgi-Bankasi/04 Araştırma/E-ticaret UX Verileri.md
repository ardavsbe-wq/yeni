---
tür: araştırma
konu: E-ticaret UX verileri ve kılavuzları (checkout, navigasyon, PLP, PDP, arama, mobil, performans, erişilebilirlik, görsel)
güncellik: 2026-10-04
etiketler: [araştırma, ux, e-ticaret, baymard, nngroup, core-web-vitals, wcag-2-2, eaa, mobil, ürün-görseli]
ilgili: ["[[Satın Alma Psikolojisi]]", "[[Türkiye E-ticaret Pazarı]]", "[[Görsel Tasarım ve Trendler 2026]]", "[[KPT Store Denetimi]]"]
---

# E-ticaret UX Verileri

> [!summary] En önemli 15 rakamlı bulgu
> 1. Ortalama sepet terk oranı **%70,22**; değer 50 çalışmanın ortalaması (Baymard, Eylül 2025). `Güçlü kanıt`
> 2. Terk nedenleri: ekstra maliyet **%40**, yavaş teslimat %20, kart güvensizliği %19, zorunlu hesap %18, uzun checkout %17, toplamı göremeyen %12. "Sadece bakıyordum" grubu (~%42) hariç (Baymard, 2025). `Güçlü kanıt`
> 3. Sitelerin **%62'si** misafir ödemeyi en belirgin seçenek yapmıyor (Baymard, 2025). `Güçlü kanıt`
> 4. İdeal checkout **7–8 alan** (12–14 eleman). Ortalama 11,3 alan ve 5,1 adım (Baymard, 2024). `Güçlü kanıt`
> 5. Checkout yeniden tasarımıyla ortalama **%35,26** dönüşüm artışı potansiyeli (Baymard, 2025). `Orta` (model tahmini)
> 6. PLP ve filtreleme UX'i **mobilde %78, masaüstünde %58** zayıf–vasat (Baymard, 2025). `Güçlü kanıt`
> 7. Sitelerin %51'inde 5 temel filtrenin, **%69'unda 4 temel sıralamanın** hepsi yok (Baymard, 2025). `Güçlü kanıt`
> 8. Kullanıcıların **%39'u** bedeninin olmadığını ancak PDP'de öğrendi. Beden filtresi üstte ve açıkken **%90'ı** önce bedenle filtreledi (Baymard, 2024). `Orta`
> 9. Kullanıcıların **%56'sı** PDP'de ilk iş görsellere bakıyor; **%42'si** boyutu görselden kestirmeye çalışıyor. Sitelerin %37'sinde ölçek görseli yok (Baymard, 2017–2026). `Orta`/`Güçlü kanıt`
> 10. Sitelerin **%56'sı** arama ihtiyacını karşılamıyor. Kısaltma ve sembol aramalarında başarısızlık %54 (Baymard, 2026). `Güçlü kanıt`
> 11. Trafiğin **%69,9'u mobil**. Dönüşüm masaüstünde %3,4, mobilde %2,0 (Contentsquare, 2026; 99 milyar oturum). `Güçlü kanıt`
> 12. Mobilde **0,1 sn hızlanma** perakende dönüşümünü %8,4, sepet ortalamasını %9,2 artırdı (Deloitte/Google, 2020; 37 marka). `Orta` (korelasyonel)
> 13. Rakuten 24 A/B testinde CWV optimizasyonu: ziyaretçi başı gelir **+%53,37**, dönüşüm **+%33,13** (web.dev, 2022). Trendyol PLP'de INP'yi %50 düşürdü (2023). `Orta` (tek vakalar)
> 14. Mobil originlerin yalnızca **%48'i** CWV'yi geçiyor; LCP'de "iyi" oranı %62 (Web Almanac, 2025). `Güçlü kanıt`
> 15. Ana sayfaların %95,9'unda WCAG hatası var; alışveriş sitelerinde sayfa başına **71 hata** (WebAIM, 2026). Türkiye'de **2025/10 sayılı Genelge** e-ticarete WCAG 2.2 uyumu için **21 Haziran 2027**'ye kadar süre veriyor. `Güçlü kanıt`

> [!info] Güvenilirlik etiketleri
> - `Güçlü kanıt`: büyük örneklemli benchmark veya anket, resmi standart veya mevzuat; 2023 ve sonrası.
> - `Orta`: birincil kaynak ama eski, küçük örneklemli, tek vaka ya da korelasyonel.
> - `Zayıf`: ikincil aktarım, satıcı/ajans iddiası ya da doğrulanamamış veri.

Bağlantılı desen notları: [[Sepet ve Ödeme]], [[Header ve Navigasyon]], [[Kategori Sayfası ve Filtreler]], [[Ürün Sayfası]], [[Beden ve Kalıp]], [[Arama]], [[Mobil Deneyim]], [[Hero ve Banner Desenleri]], [[Güven Sinyalleri]], [[Footer]], [[Renk ve Tipografi]].

## Konu bazında temel veriler

| Konu | Bulgu | Kaynak / yıl | Güven |
|---|---|---|---|
| Checkout | Telefon vermekte isteksiz %70+; teslimat tarihi yerine hız yazan %48; kargo kesim saati göstermeyen %83; genel hata mesajı kullanan %94; zorunlu/isteğe bağlı alanı işaretlemeyen %61 | Baymard, 2025 | Güçlü kanıt |
| Checkout | Tek ad alanı kullanmayan %89; "Adres 2"yi gizlemeyen %75; hesap oluşturmayı ertelemeyen %84 | Baymard, 2024 | Güçlü kanıt |
| Checkout | Ev yapımı güven mührü bile çoğu SSL mührünü geçti; kart alanını görsel olarak kapsülleme önerisi | Baymard, 2023 | Orta |
| Navigasyon | Navigasyon UX'i masaüstünde %58, mobilde %67 vasat–kötü. Bulunulan kategoriyi vurgulamayan %95, hover gecikmesi olmayan %61, başlıkları tıklanamayan %33 | Baymard, 2025 | Güçlü kanıt |
| Navigasyon | Mega menü 0,5 sn hareketsizlikten sonra açılmalı, 0,1 sn içinde görünmeli. Gizli menü kullanımı mobilde %57, kombine menüde %86 | NN/g, 2016–2017 | Orta |
| PLP | Çoklu filtreyi kısıtlayan %14; uygulanan filtreleri göstermeyen %20–28 (mobilde %66); varyasyonları birleştirmeyen %42; yatay filtre çubuğu kullanan %24 | Baymard, 2025–2026 | Güçlü kanıt |
| PLP | "Daha fazla yükle" öneriliyor. Masaüstünde 10–30 ürün tembel yüklenip 50–100'den sonra buton; mobilde 15–30; aramada sonsuz kaydırma yok | Baymard, 2016 / 2026 | Orta |
| PDP | PDP UX'i masaüstünde %52, mobilde %62 vasat–kötü. Beden butonu kullanmayan %57 (giyimde %70); insan model görseli olmayan %23; iade politikasını öne çıkarmayan %44 | Baymard, 2026 | Güçlü kanıt |
| PDP | Yetersiz beden bilgisi %82; kalıp alt puanı olmayan %24; yorum görselleri arasında gezinme sunmayan %90 | Baymard, 2025 | Güçlü kanıt |
| PDP | Ana bölümlerde yatay sekme kullanan %29; özellik tablosu zayıf–vasat %64 | Baymard, 2026 | Güçlü kanıt |
| PDP | Stoksuz ürün görünce başka siteye giden %30; geçici stoksuzlukta sipariş aldırmayan %68 | Baymard, 2025 | Orta |
| PDP | Ziyaretlerin üçte biri PDP'de başlıyor; PDP ziyaretlerinin %61'i hemen çıkıyor | Contentsquare, 2026 | Güçlü kanıt |
| Yorumlar | 5 yorum satın alma olasılığını %270 artırıyor; ideal puan 4,0–4,7; doğrulanmış alıcı rozeti +%15 | Spiegel, 2017 | Orta |
| Sticky ATC | Bir testte dönüşüm +%6,2, diğerinde −%7,7 (sonuçsuz) | Clean Commit, 2025 | Zayıf |
| Arama | Otomatik tamamlama sunan %80, tam uygulayan %19; öneri sayısı masaüstünde ≤10, mobilde 4–8. Yazım hatasında öneri sunmayan %69 (2021) / mobilde %28 (2026); sonuçsuz aramadan çıkış yolu sunmayan ~%50 | Baymard, 2021–2026 | Orta/Güçlü kanıt |
| Mobil | Tek elle kullanım %49 | Hoober, 2013 | Orta |
| Mobil | Hedef boyutu: WCAG 2.5.8 ≥24 px (AA), 2.5.5 44 px (AAA); Android 48 dp ve 8 dp boşluk; Apple 44 pt | W3C, Google, Apple | Güçlü kanıt (Apple: Orta) |
| Performans | CWV eşikleri p75'te: LCP ≤2,5 sn, INP ≤200 ms, CLS ≤0,1 | web.dev | Güçlü kanıt |
| Performans | Sayfaların ~%16–17'si LCP görselini tembel yüklüyor; WebP payı %11 | Web Almanac, 2025 | Güçlü kanıt |
| Performans | Vodafone LCP −%31 ile satış +%8; redBus INP −%72 ile satış +%7 | web.dev, 2021–2023 | Orta |
| Performans | 1 sn'de yüklenen site 5 sn'dekinden 2,5 kat fazla dönüştürüyor | Portent, 2022 | Orta |
| Performans | 100 ms gecikme dönüşümü %7 düşürüyor | Akamai, 2017 | Orta |
| Erişilebilirlik | En sık hatalar: düşük kontrast %83,9, eksik alt metin %53,1, etiketsiz form %51, boş link %46,3 | WebAIM, 2026 | Güçlü kanıt |
| Erişilebilirlik | Engelli kullanıcıların %69'u zorlandığı siteyi terk ediyor (BK'de 17,1 milyar £) | Click-Away Pound, 2019 | Orta |
| Erişilebilirlik | Dünyada 1,3 milyar engelli (%16) | DSÖ, 2023 | Güçlü kanıt |
| Karusel | Masaüstü sitelerin %33'ünde karusel var, bunların %46'sında sorun. Otomatik geçiş 5–7 sn; mobilde otomatik dönme yok | Baymard, 2025 | Güçlü kanıt |
| Pop-up | Kullanıcıların en çok nefret ettiği teknik modal pop-up | NN/g, 2017 | Orta |
| Pop-up | Google içeriği engelleyen promosyon geçiş ekranlarını önermiyor | Google Search Central | Güçlü kanıt |
| Çerez | 3 eşit seçenek, küçük bant, katmanları üst üste koymama | NN/g, 2023 | Orta |
| AI görseli | Kaynak bilinmediğinde AI görseli stok fotoğrafla aynı güveni aldı (+0,2, anlamlı değil); AI'dan şüphelenince puan düştü. 77 kişi, hero görseli, ürün görseli değil | NN/g, Ağustos 2026 | Orta |
| 3D/AR | AR görüntüleyenlerde satın alma +%65 (Rebecca Minkoff vakası) | Shopify, 2026 | Zayıf |

## Mevzuat
- **Türkiye, Genelge 2025/10** (Resmî Gazete 21.06.2025, sayı 32933): E-ticaret hizmet sağlayıcıları 2 yıl içinde uyum sağlamalı. Referanslar WCAG 2.2 ve Aile ve Sosyal Hizmetler Bakanlığı'nın "Kontrol Listesi – A Seviyesi". Uyumlu sitelere 2 yıllık Erişilebilirlik Logosu veriliyor. İşletme büyüklüğü eşiği bulunamadı.
- **AB, EAA (Direktif 2019/882):** 28.06.2025'ten beri uygulanıyor. E-ticaret hizmetlerini ve AB tüketicisine satış yapan AB dışı satıcıları kapsıyor. Hizmet sunan mikro işletmeler (<10 çalışan ve ≤2 milyon €) muaf. Teknik referans EN 301 549 (WCAG 2.1 AA). Ayrıntılar ikincil kaynaklardan; `Orta`. KPT yalnız Türkiye'ye satıyorsa EAA doğrudan uygulanmaz.
- **WCAG 2.2'de yeni kriterler** (W3C, 2023): 2.4.11 Odak gizlenmemeli (AA), 2.5.7 Sürükleme alternatifi (AA), 2.5.8 Hedef boyutu (AA), 3.2.6 Tutarlı yardım (A), 3.3.7 Tekrarlı giriş (A), 3.3.8 Erişilebilir kimlik doğrulama (AA).
- **AB Yapay Zekâ Yasası, Madde 50:** 2 Ağustos 2026'dan itibaren sentetik görseller işaretlenmeli, deepfake içerik açıklanmalı.

## Çelişkili ve eksik veriler
- Sepet terk oranı bir sayfada %70,22, diğerinde %70,19.
- Ortalama form alanı 2024 blogunda 11,3; başka bir sayfada 14,88 (ölçüm tanımları farklı).
- Misafir ödemeyi öne çıkarmayan siteler 2023'te %47, 2025'te %62.
- Ekstra maliyet nedeni eski aktarımlarda %48, 2025 anketinde %40.
- Ölçek görseli eksikliği 2017'de %28, 2026'da %37.
- Yetersiz beden bilgisi 2025'te %82; ikincil kaynaklarda eski bir %94 değeri dolaşıyor.
- Yazım hatası desteği eksikliği %69 (2021) ile %28 (2026, mobil) arasında; gelişme mi ölçüm farkı mı belirsiz.
- "Sticky ATC +%7,9 (Baymard)" iddiasının birincil kaynağı bulunamadı.
- **Bulunamayanlar:** bağımsız ve güncel 360°/video/AR verisi; AI ile üretilmiş *ürün* görsellerinin güvene etkisini ölçen çalışma; Baymard'ın stok dışı beden ve bedene göre fiyat yönergelerinin ayrıntısı (Premium); KVKK çerez kuralları.

## KPT için uygulama kuralları

Renkler KPT paletinden: zemin #F3F4F1/#E5E8E3, metin #171B1C, vurgu #741E32. Kontrast oranları WCAG formülüyle hesaplandı. "(öneri)" ifadesi, kaynaktaki aralığın KPT'ye uyarlandığını gösterir.

**Sepet ve ödeme ([[Sepet ve Ödeme]])**
1. **Kural:** Checkout'un ilk ekranında en üstte 48px yükseklikte, #741E32 dolgulu "Üye olmadan devam et" butonu; altında çerçeveli "Giriş yap". Hesap oluşturma sipariş onay sayfasında sunulmalı. **Neden:** Görülmeyen misafir seçeneği yok sayılır. **Kanıt:** %62 site / %18 terk (Baymard, 2025).
2. **Kural:** Sepette "Ara toplam / Kargo / Toplam" yazmalı; kargo somut tutar olmalı. Eşik varsa "Ücretsiz kargoya ₺{x} kaldı" ilerleme çubuğu. **Neden:** Bir numaralı terk nedeni. **Kanıt:** %40 ekstra maliyet, %12 toplamı görememe (Baymard, 2025).
3. **Kural:** En fazla 8 görünür alan: Ad Soyad (tek alan), e-posta, telefon, il, ilçe, adres, posta kodu. "Daire/kat ekle" ve kupon alanı link arkasında. **Neden:** Kullanılabilirliği adım sayısından çok alan sayısı belirliyor. **Kanıt:** İdeal 7–8 alan; tek ad alanını %89 site kullanmıyor (Baymard, 2024).
4. **Kural:** "Fatura adresi teslimatla aynı" kutusu varsayılan olarak işaretli. **Neden:** Tekrar girişi önler. **Kanıt:** WCAG 3.3.7 (A).
5. **Kural:** Teslimat "Tahmini teslimat: 8–10 Ekim" gibi tarih aralığıyla verilmeli; gerçek veri varsa kesim saati eklenmeli. Önizlemede uydurma değer kullanılmamalı. **Neden:** Belirsizliği kaldırır. **Kanıt:** Hız yazan %48, kesim saati göstermeyen %83 (Baymard, 2025).
6. **Kural:** Telefon alanının altında "Kargo firması teslimat için arayabilir" açıklaması; alanlarda "*" ve "(isteğe bağlı)" işaretleri. **Neden:** Kullanıcılar telefon vermekte isteksiz. **Kanıt:** %70+ isteksiz, %49 site gerekçe yazmıyor (Baymard, 2025).
7. **Kural:** Hatalar alan çıkışında satır içinde ve duruma özel gösterilmeli ("Posta kodu 5 haneli olmalı"), `aria-describedby` ile alana bağlanmalı. **Neden:** Genel mesaj yol göstermiyor. **Kanıt:** %94 site genel mesaj kullanıyor (Baymard, 2025).
8. **Kural:** Kart alanları 1px #7A7F77 kenarlıklı, #F3F4F1 zeminli tek bir kutuda; başlıkta kilit ikonu, altta kart ve taksit logoları. **Neden:** Güven algısını artırır. **Kanıt:** %19 kart güvensizliğinden terk ediyor (Baymard, 2025).
9. **Kural:** Adet seçici 44px "−/+" butonlarıyla; şifre kuralı yalnızca "en az 8 karakter"; yapıştırmaya izin. **Neden:** Sürtünmeyi azaltır. **Kanıt:** Adet seçicide %97, şifre kuralında %65 site başarısız (Baymard, 2025); WCAG 3.3.8.

**Navigasyon ([[Header ve Navigasyon]])**
10. **Kural:** Header sırası: Logo | Erkek | Kadın | Çocuk | Markalar | Yeni Gelenler | İndirim | arama alanı (en az 320px) | Favoriler | Sepet. Her üst öğe tıklanabilir bir PLP'ye gitmeli. **Neden:** Bu ayrımlar giyimde birbirini dışlayan ürün boyutları. **Kanıt:** Başlıkları tıklanamayan %33 (Baymard, 2025); NN/g (2015).
11. **Kural:** Mega menü 400ms gecikmeyle açılıp kapanmalı (öneri), kaydırma gerektirmemeli; her sütunda "Tüm …" linki olmalı. **Neden:** Yanlışlıkla açılmayı önler. **Kanıt:** NN/g 0,5 sn (2017); %61 site gecikme uygulamıyor (Baymard, 2025).
12. **Kural:** Aktif kategori 2px #741E32 alt çizgiyle vurgulanmalı; PLP'de breadcrumb olmalı. **Neden:** Kullanıcı kapsamını görmeli. **Kanıt:** %95 site vurgulamıyor (Baymard, 2025).
13. **Kural:** "Erkek" gibi ara sayfalar alt kategorileri 4:5 oranlı görsel karolarla birincil içerik olarak göstermeli. "Numaranla başla" ızgarası `?beden=42` filtreli PLP'ye gitmeli. **Neden:** Bir sonraki adım net olmalı. **Kanıt:** %76 site alt kategorileri öne çıkarmıyor (Baymard, 2025).

**PLP ([[Kategori Sayfası ve Filtreler]])**
14. **Kural:** Filtre sırası: Beden (varsayılan açık, 48×44px buton ızgarası) → Cinsiyet → Marka → Fiyat → Renk → Kullanım. **Neden:** İlk eleme kriteri beden. **Kanıt:** %90 önce bedenle filtreledi; %39 bedensizliği PDP'de öğrendi (Baymard, 2024).
15. **Kural:** Tüm filtreler çoklu seçimli checkbox olmalı; tek seçimli açılır menü kaldırılmalı. Mobilde filtreler "128 ürünü göster" butonuyla uygulanmalı. **Neden:** Kullanıcılar değer birleşimleri istiyor. **Kanıt:** %14 site çoklu seçimi kısıtlıyor (Baymard, 2025).
16. **Kural:** Ham tedarikçi renkleri 12 ana renk ailesine eşlenmeli ve 24px swatch ile gösterilmeli. **Neden:** Ham değerler filtreyi kullanılmaz kılıyor. **Kanıt:** %51 site temel filtrelerde eksik; mobilde %73 site swatch eksik (Baymard, 2025–2026).
17. **Kural:** Her filtre seçeneğinin yanında sonuç sayısı ("42 (37)"); başlıkta "Erkek Sneaker · 128 ürün". **Neden:** Kullanıcı seçmeden önce sonucu görmeli. **Kanıt:** Baymard PLP rehberi, 2026.
18. **Kural:** Uygulanan filtre çipleri ızgaranın üstünde olmalı: 36px yükseklik, #E5E8E3 zemin, en az 24px'lik "×" hedefi ve "Tümünü temizle" linki. **Neden:** Kullanıcı neyin filtrelendiğini ve nasıl geri alacağını görmeli. **Kanıt:** Eksik %20–28, mobilde %66 (Baymard).
19. **Kural:** Sıralama seçenekleri: Önerilen, En çok satanlar, En yeniler, Fiyat ↑, Fiyat ↓ (yorum verisi gelince "En yüksek puan"). **Neden:** Temel sıralama türleri. **Kanıt:** %69 site eksik (Baymard, 2025).
20. **Kural:** Masaüstünde 24+24 ürün tembel yüklenmeli, sonra "Daha fazla göster" butonu ve "321 üründen 48'i" metni; mobilde 24 üründen sonra buton. Sonsuz kaydırma yok. PDP'den dönüşte konum korunmalı. **Neden:** Gezinme ile footer erişimi arasında denge. **Kanıt:** Baymard 2016 / 2026.
21. **Kural:** Ürün kartında renk varyasyonları tek kartta birleştirilmeli ("4 renk"); hover'da ikinci görsel; en fazla bir rozet ("YENİ", "İNDİRİM %20"). **Neden:** Liste şişmesini ve rozet körlüğünü önler. **Kanıt:** %42 site birleştirmiyor (Baymard, 2025); rozet rehberi (Baymard, 2026).
22. **Kural:** Mobilde 48px'lik sticky "Filtrele (3) | Sırala" çubuğu ve alttan açılan çekmece. **Neden:** Filtre her an erişilebilir olmalı. **Kanıt:** Mobil PLP'lerin %78'i zayıf (Baymard, 2025).

**PDP ([[Ürün Sayfası]], [[Beden ve Kalıp]])**
23. **Kural:** Beden seçici 48×44px buton ızgarası olmalı: varsayılan 1px #7A7F77 kenarlık (3,71:1), seçili #171B1C zemin ve beyaz metin; yanında "Beden rehberi" linki. **Neden:** Açılır liste stok durumunu gizliyor. **Kanıt:** %57–70 site buton kullanmıyor (Baymard, 2025–2026).
24. **Kural:** Stokta olmayan bedenler gösterilmeli: #6B7069 metin, çapraz çizgi, `aria-label="42 – stokta yok"`. Tıklanınca "Gelince haber ver" ve diğer renklerdeki stok gösterilmeli. **Neden:** Gizlenen beden alternatif yolu kapatıyor. **Kanıt:** %30 terk (Baymard, 2025); stil `(tahmin)`.
25. **Kural:** Beden rehberinde marka bazında EU/US/UK/cm tablosu, ayak ölçme talimatı ve yalnızca doğrulanmış kalıp notu yer almalı. **Neden:** Ayakkabıda iadenin ana nedeni beden. **Kanıt:** %82 site yetersiz beden bilgisi sunuyor (Baymard, 2025).
26. **Kural:** Her üründe en az 7 görsel: dış yan, ön 3/4, iç yan, üst, taban, topuk ve **ayakta ölçek görseli**. 1:1 oran, #F3F4F1 zemin, en az 2000px kaynak, zoom. **Neden:** PDP'de ilk eylem görsel inceleme. **Kanıt:** %56 / %42 / ölçek görseli eksik %37 (Baymard).
27. **Kural:** Açıklama tek dikey akışta, sekmesiz: Öne çıkanlar (3–5 madde) → Özellikler tablosu (malzeme, taban, ağırlık g, topuk-burun farkı mm, kalıp) → Bakım → Teslimat ve İade. Mobilde akordeon. **Neden:** Sekmelerdeki içerik gözden kaçıyor. **Kanıt:** %29 sekme kullanıyor, %64 tablo zayıf (Baymard, 2026).
28. **Kural:** Fiyat bedene göre değişiyorsa PLP'de "₺3.499'dan başlayan", PDP'de "Fiyat bedene göre değişir". Seçimle fiyat güncellenmeli ve `aria-live` ile duyurulmalı. **Neden:** Gizli fark sürpriz maliyet yaratır. **Kanıt:** %40 terk nedeni (Baymard, 2025); desen `(tahmin)`.
29. **Kural:** "Sepete ekle" altında 3 satırlık güven bloğu: teslimat tarihi, "{n} gün ücretsiz iade", taksit. Yalnızca gerçek değerler kullanılmalı. **Neden:** Belirsizlik terk ettiriyor. **Kanıt:** %44 site iade politikasını öne çıkarmıyor (Baymard, 2026). Bkz. [[Güven Sinyalleri]].
30. **Kural:** Mobilde sticky ATC çubuğu: 64px + safe area; beden, fiyat ve #741E32 "Sepete ekle". Beden seçilmemişse buton beden çekmecesini açmalı. A/B testiyle doğrulanmalı. **Neden:** Uzun sayfada CTA erişimi. **Kanıt:** Karışık sonuçlar (Clean Commit, 2025) — Zayıf.
31. **Kural:** Yorum modülünde kalıp alt puanı ("Küçük – Tam – Büyük"), yorum görselleri arasında gezinme, doğrulanmış alıcı rozeti ve olumsuz yorumlara yanıt olmalı. **Neden:** Beden kararı hızlanır. **Kanıt:** 5 yorumla +%270 (Spiegel, 2017); kalıp puanı eksik %24 (Baymard, 2025).

**Arama ([[Arama]])**
32. **Kural:** Otomatik tamamlama: mobilde en fazla 6, masaüstünde en fazla 8 öneri ve 3 ürün kartı; tamamlanan kısım kalın; ok tuşu desteği; satırlar en az 48px. **Neden:** Seçim felcini önler. **Kanıt:** Masaüstünde ≤10, mobilde 4–8 (Baymard, 2022).
33. **Kural:** Arama Türkçe karakterleri katlamalı (ı/i, ş/s, ğ/g, ü/u, ö/o, ç/c), yazım hatasına tolerans göstermeli ve eş anlamlıları tanımalı ("naik→nike", "nb→new balance", "spor ayakkabı→sneaker", "42 numara→beden 42"). **Neden:** Hatalı sorgular sıfır sonuca düşüyor. **Kanıt:** %69 / %28 başarısız; kısaltmalarda %54 (Baymard).
34. **Kural:** Sonuç yok sayfası: "Bunu mu demek istediniz", kategori karoları, çok satanlar ve WhatsApp/telefon yardımı içermeli. **Neden:** Çıkmaz sokak terk ettiriyor. **Kanıt:** ~%50 site başarısız (Baymard, 2025).

**Mobil ([[Mobil Deneyim]])**
35. **Kural:** Tüm dokunma hedefleri en az 44×44px ve aralarında 8px boşluk; küçük ikonlarda tıklama alanı en az 24px. **Neden:** Yanlış dokunmayı önler. **Kanıt:** WCAG 2.5.8 / 2.5.5; Android 48dp.
36. **Kural:** 5 öğeli alt sekme çubuğu: Ana sayfa, Kategoriler, Ara, Favoriler, Sepet; aktif sekme #741E32. Birincil CTA'lar ekranın alt üçte birinde. **Neden:** Görünür navigasyon daha çok kullanılıyor; tek elle kullanım yaygın. **Kanıt:** Gizli menü %57, kombine %86 (NN/g, 2016); tek el %49 (Hoober, 2013).

**Performans**
37. **Kural:** Mobil p75 hedefleri: LCP ≤2,0 sn, INP ≤200ms, CLS ≤0,05. Hero PNG'den AVIF/WebP'ye çevrilmeli: mobilde ≤120 KB, masaüstünde ≤200 KB (öneri), `fetchpriority="high"`, lazy yok, `width`/`height` veya `aspect-ratio` tanımlı. **Neden:** 900 KB'lık PNG büyük olasılıkla LCP öğesi. **Kanıt:** Deloitte +%8,4; Rakuten +%33; LCP görselini lazy yükleyen %16–17 (Almanac, 2025).
38. **Kural:** Filtre ve beden işleyicilerinde uzun görevler `scheduler.yield()` ile bölünmeli; kaydırmaya debounce; 24'lük tembel yükleme grupları. **Neden:** INP etkileşim hissini belirliyor. **Kanıt:** Trendyol INP −%50; redBus satış +%7 (web.dev).

**Erişilebilirlik ([[Renk ve Tipografi]], [[Footer]])**
39. **Kural:** Hedef WCAG 2.2 AA, son tarih 21.06.2027. Token'lar: `--text-muted #5C615A` (5,74:1), `--border-ui #7A7F77` (en az 3:1). Odak halkası 2px #741E32, 2px offset. Sticky çubuklar için `scroll-padding` tanımlanmalı. Alt metin şablonu "{Marka} {Model} {Renk} – {açı}"; görünür `<label>` ve `autocomplete`; fiyat kaydırıcısına sayı alanları; yardım kanalları her sayfada aynı sırada. **Neden:** Yasal zorunluluk ve en yaygın hatalar. **Kanıt:** Genelge 2025/10; WebAIM 2026; WCAG 2.4.11, 2.5.7, 3.2.6.

**Hero, pop-up, çerez ve görseller ([[Hero ve Banner Desenleri]], [[Görsel Tasarım ve Trendler 2026]])**
40. **Kural:** Hero statik olmalı. Dönen animasyon kalacaksa 5 sn içinde durmalı ya da 44px "Duraklat" butonu olmalı; `prefers-reduced-motion` desteklenmeli. Mobilde karusel otomatik dönmemeli. **Neden:** Erişilebilirlik ve görünürlük. **Kanıt:** WCAG 2.2.2; Baymard 2025; NN/g 2013.
41. **Kural:** Açılışta modal pop-up olmamalı; e-bülten footer'da sunulmalı. Çerez bandı altta olmalı ve 3 eşit buton içermeli ("Tümünü kabul et / Yalnızca zorunlu / Tercihler"); diğer katmanlarla üst üste binmemeli. **Neden:** Modal en nefret edilen teknik. **Kanıt:** NN/g 2017, 2023; Google Search Central.
42. **Kural:** Ürünü temsil eden görseller gerçek fotoğraf olmalı. AI görseli yalnız atmosfer ve hero için, hatasız (çift pozlama yok) ve gerektiğinde etiketli kullanılmalı. Video ve AR, statik görsel seti tamamlandıktan ve A/B testinden sonra eklenmeli. **Neden:** AI şüphesi algıyı düşürüyor; AR ve video kanıtı zayıf. **Kanıt:** NN/g 2026; AB Yapay Zekâ Yasası Madde 50; Shopify vakası (Zayıf).

## Kaynaklar
- https://baymard.com/lists/cart-abandonment-rate
- https://baymard.com/research/checkout-usability
- https://baymard.com/blog/checkout-flow-average-form-fields
- https://baymard.com/blog/make-guest-checkout-prominent
- https://baymard.com/blog/current-state-of-checkout-ux
- https://baymard.com/blog/perceived-security-of-payment-form
- https://baymard.com/blog/ecommerce-navigation-best-practice
- https://baymard.com/research-articles/current-state-product-list-and-filtering
- https://baymard.com/blog/product-listing-page-plp-ux
- https://baymard.com/blog/horizontal-filtering-sorting-design
- https://baymard.com/blog/apparel-put-size-filter-near-top-and-expand-for-sidebar-filtering
- https://baymard.com/blog/apparel-5-best-practices
- https://baymard.com/blog/badge-ui
- https://baymard.com/blog/current-state-ecommerce-product-page-ux
- https://baymard.com/blog/in-scale-product-images
- https://baymard.com/blog/ensure-sufficient-image-resolution-and-zoom
- https://baymard.com/blog/avoid-horizontal-tabs
- https://baymard.com/blog/product-spec-sheet-ux-design
- https://baymard.com/blog/handling-out-of-stock-products
- https://baymard.com/guidelines/850-size-variation-selector-implementation-details
- https://baymard.com/guidelines/421-product-variations-in-product-lists
- https://baymard.com/blog/ecommerce-search-query-types
- https://baymard.com/blog/autocomplete-design
- https://baymard.com/blog/offer-autocomplete-suggestions-for-misspellings
- https://baymard.com/blog/no-results-page
- https://baymard.com/blog/mobile-ux-ecommerce
- https://baymard.com/blog/homepage-carousel
- https://www.smashingmagazine.com/2016/03/pagination-infinite-scrolling-load-more-buttons/
- https://www.nngroup.com/articles/mega-menus-work-well/
- https://www.nngroup.com/articles/audience-based-navigation/
- https://www.nngroup.com/articles/hamburger-menus/
- https://www.nngroup.com/articles/mobile-navigation-patterns/
- https://www.nngroup.com/articles/touch-target-size/
- https://www.nngroup.com/articles/auto-forwarding/
- https://www.nngroup.com/articles/most-hated-advertising-techniques/
- https://www.nngroup.com/articles/cookie-permissions/
- https://www.nngroup.com/articles/ai-generated-images/
- https://web.dev/articles/vitals
- https://web.dev/articles/optimize-lcp
- https://almanac.httparchive.org/en/2025/performance
- https://web.dev/case-studies/rakuten
- https://web.dev/case-studies/vodafone
- https://web.dev/case-studies/trendyol-inp
- https://web.dev/case-studies/redbus-inp
- https://web.dev/case-studies/milliseconds-make-millions
- https://www.deloitte.com/ie/en/services/consulting/research/milliseconds-make-millions.html
- https://www.akamai.com/fr/newsroom/press-release/akamai-releases-spring-2017-state-of-online-retail-performance-report
- https://www.portent.com/blog/analytics/research-site-speed-hurting-everyone.htm
- https://contentsquare.com/guides/digital-experience-benchmark/traffic/
- https://contentsquare.com/guides/digital-experience-benchmark/conversions/
- https://contentsquare.com/guides/digital-experience-benchmark/engagement/
- https://www.uxmatters.com/mt/archives/2013/02/how-do-users-really-hold-mobile-devices.php
- https://support.google.com/accessibility/android/answer/7101858
- https://developer.apple.com/design/human-interface-guidelines/accessibility (metin okunamadı)
- https://spiegel.medill.northwestern.edu/how-online-reviews-influence-sales/
- https://cleancommit.io/ab-tests/sticky-mobile-add-to-cart-button/
- https://cleancommit.io/ab-tests/mobile-bottom-sticky-add-to-cart-button/
- https://www.shopify.com/blog/3d-ecommerce
- https://www.w3.org/WAI/standards-guidelines/wcag/new-in-22/
- https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html
- https://webaim.org/projects/million/
- https://www.who.int/campaigns/international-day-of-persons-with-disabilities/2023
- https://abilitynet.org.uk/news-blogs/research-shows-businesses-lose-17-billion-ignoring-accessibility-needs
- https://commission.europa.eu/strategy-and-policy/policies/justice-and-fundamental-rights/disability/union-equality-strategy-rights-persons-disabilities-2021-2030/european-accessibility-act_en
- https://e-include.eu/web-accessibility/european-accessibility-act/ (ikincil)
- https://www.erdem-erdem.av.tr/bilgi-bankasi/web-siteleri-ve-mobil-uygulamalarin-erisilebilirligi-hakkinda-2025-10-sayili-cumhurbaskanligi-genelgesi-yayimlandi
- https://ikas.com/tr/blog/e-ticaret-siteleri-icin-yeni-zorunluluk-web-erisilebilirligi
- https://webrazzi.com/2025/06/30/web-siteleri-ve-uygulamalar-icin-erisilebilirlik-zorunlulugu-geliyor/
- https://artificialintelligenceact.eu/article/50/
- https://developers.google.com/search/docs/appearance/avoid-intrusive-interstitials
