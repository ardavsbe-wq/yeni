---
tür: araştırma
konu: E-ticaret kullanıcı deneyimi verileri, benchmark'ları ve kılavuzları (checkout, navigasyon, PLP, PDP, arama, mobil, performans, erişilebilirlik, görsel)
güncellik: 2026-10-04
kapsam-yılları: 2023–2026 öncelikli; temel kabul edilen eski çalışmalar yılıyla işaretli
birincil-kaynaklar: [Baymard Institute, Nielsen Norman Group, web.dev, HTTP Archive Web Almanac, Contentsquare, Deloitte, Akamai, W3C/WAI, WebAIM, AB Erişilebilirlik Yasası, T.C. Cumhurbaşkanlığı Genelgesi 2025/10]
etiketler: [araştırma, ux, e-ticaret, baymard, nngroup, checkout, plp, pdp, arama, mobil, core-web-vitals, erişilebilirlik, wcag-2-2, eaa, ürün-görseli]
ilgili: ["[[Satın Alma Psikolojisi]]", "[[Türkiye E-ticaret Pazarı]]", "[[Görsel Tasarım ve Trendler 2026]]", "[[KPT Store Denetimi]]"]
---

# E-ticaret UX Verileri

> [!summary] En önemli 15 rakamlı bulgu
> 1. Belgelenmiş ortalama **sepet terk oranı %70,22**'dir; değer 50 çalışmanın ortalamasıdır (Baymard, Eylül 2025). `Güçlü kanıt`
> 2. Terk nedenlerinin başında **%40 ile ekstra maliyetler** (kargo, vergi, ücret) geliyor. Onu %20 ile yavaş teslimat, %19 ile kart güvensizliği ve %18 ile zorunlu hesap izliyor. "Sadece bakıyordum" grubu (~%42) bu oranlara dahil değil (Baymard, 2025). `Güçlü kanıt`
> 3. Sitelerin **%62'si misafir ödemeyi en belirgin seçenek yapmıyor** (Baymard Checkout benchmark, 2025). `Güçlü kanıt`
> 4. İdeal checkout **7–8 form alanı** (12–14 form elemanı) içerir. 2024'te ortalama 11,3 alan ve 5,1 adımdı (Baymard, 2024). `Güçlü kanıt`
> 5. Checkout yeniden tasarımıyla ortalama **%35,26 dönüşüm artışı** potansiyeli hesaplanıyor (Baymard, 2025). `Orta` (model tahmini)
> 6. Ürün listeleme ve filtrelemede **mobil sitelerin %78'i, masaüstü sitelerin %58'i** "zayıf–vasat" seviyede (Baymard, 2025). `Güçlü kanıt`
> 7. Sitelerin **%51'inde 5 temel filtre türünün** (fiyat, puan, renk, beden, marka) hepsi yok. **%69'unda 4 temel sıralamanın** hepsi yok (Baymard, 2025). `Güçlü kanıt`
> 8. Giyim testlerinde katılımcıların **%39'u** beğendiği ürünün kendi bedeninde olmadığını ancak PDP'de öğrendi. Beden filtresi en üstte ve açık durduğunda katılımcıların **%90'ı** önce bedene göre filtreledi (Baymard, 2024). `Orta`
> 9. Kullanıcıların **%56'sı** PDP'de ilk iş olarak görsellere bakıyor. **%42'si** ürünün boyutunu görsellerden anlamaya çalışıyor (Baymard, 2017–2020). `Orta`
> 10. Sitelerin **%56'sı** kullanıcıların arama ihtiyacını karşılamıyor. Kısaltma ve sembol içeren aramalarda başarısızlık %54, ürün dışı aramalarda %66 (Baymard, 2026). `Güçlü kanıt`
> 11. Trafiğin **%69,9'u mobilden** geliyor. Dönüşüm oranı masaüstünde %3,4, mobilde %2,0; perakendede bu fark %3,7'ye %2,0 (Contentsquare, 2026; 99 milyar oturum). `Güçlü kanıt`
> 12. Mobil sitenin **0,1 sn hızlanması** perakendede dönüşümü %8,4, sepet ortalamasını %9,2 artırdı (Deloitte/Google "Milliseconds Make Millions", 2020; 37 marka, 30 milyon+ oturum). `Orta` (korelasyonel)
> 13. Rakuten 24'ün A/B testinde Core Web Vitals optimizasyonu **ziyaretçi başına geliri %53,37, dönüşümü %33,13** artırdı (web.dev, 2022). `Orta` (tek vaka)
> 14. Mobil originlerin yalnızca **%48'i** Core Web Vitals'ı geçiyor; en zayıf metrik LCP (%62 iyi) (Web Almanac, 2025). `Güçlü kanıt`
> 15. Ana sayfaların **%95,9'unda** WCAG hatası tespit edildi. Alışveriş sitelerinde sayfa başına ortalama **71 hata** var (WebAIM Million, 2026). Türkiye'de **2025/10 sayılı Genelge**, e-ticaret sitelerine WCAG 2.2 uyumu için 21 Haziran 2027'ye kadar süre tanıyor. `Güçlü kanıt`

> [!info] Güvenilirlik etiketleri
> - `Güçlü kanıt`: büyük örneklemli birincil benchmark veya anket (Baymard, Contentsquare, Web Almanac, WebAIM), resmi standart veya mevzuat; 2023 ve sonrası.
> - `Orta`: birincil kaynak ama eski (2023 öncesi), küçük örneklemli, tek şirketin vakası ya da korelasyonel veri.
> - `Zayıf`: ikincil aktarım, satıcı veya ajans iddiası, metodolojisi belirsiz ya da bu oturumda birincil kaynağı doğrulanamamış veri.

Bu not, KPT Store'u ([[KPT Store Denetimi]]) yeniden tasarlayacak kod ajanları için kanıt tabanıdır. Desen notları ([[Header ve Navigasyon]], [[Kategori Sayfası ve Filtreler]], [[Ürün Sayfası]], [[Beden ve Kalıp]], [[Sepet ve Ödeme]], [[Arama]], [[Mobil Deneyim]], [[Hero ve Banner Desenleri]], [[Güven Sinyalleri]], [[Footer]], [[Renk ve Tipografi]]) buradaki rakamlara dayanmalıdır. Psikolojik ilkeler için [[Satın Alma Psikolojisi]], Türkiye'ye özgü pazar verileri için [[Türkiye E-ticaret Pazarı]] notuna bakın.

---

## 1. Sepet terk, checkout ve misafir ödeme

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| Ortalama belgelenmiş sepet terk oranı | %70,22 (50 çalışma) | Baymard, güncelleme 22.09.2025 | Güçlü kanıt |
| Terk nedeni: ekstra maliyetler çok yüksek | %40 | Baymard anketi, 2025 | Güçlü kanıt |
| Terk nedeni: teslimat çok yavaş | %20 | Baymard, 2025 | Güçlü kanıt |
| Terk nedeni: kart bilgisi için siteye güvenmedi | %19 | Baymard, 2025 (1.026 ABD'li yetişkin) | Güçlü kanıt |
| Terk nedeni: hesap oluşturma zorunluluğu | %18–19 | Baymard, 2025 | Güçlü kanıt |
| Terk nedeni: uzun/karmaşık checkout | %17 | Baymard, 2025 | Güçlü kanıt |
| Terk nedeni: site hatası/çökme | %17 | Baymard, 2025 | Güçlü kanıt |
| Terk nedeni: iade politikası yetersiz | %13 | Baymard, 2025 | Güçlü kanıt |
| Terk nedeni: toplam maliyet önceden görülemedi | %12 | Baymard, 2025 | Güçlü kanıt |
| Terk nedeni: kart reddedildi / yetersiz ödeme yöntemi | %10 / %9 | Baymard, 2025 | Güçlü kanıt |
| İdeal checkout | 12–14 form elemanı, 7–8 form alanı | Baymard, 2024–2025 | Güçlü kanıt |
| Ortalama checkout | 5,1 adım, 11,3 alan (2019: 12,7; 2021: 11,8) | Baymard, Haziran 2024 | Güçlü kanıt |
| Ortalama ABD checkout'u (farklı ölçüm) | 23,48 form elemanı, 14,88 alan | Baymard sepet terk sayfası, 2025 | Orta (ölçüm tanımı farklı) |
| Checkout tasarımıyla geri kazanılabilir dönüşüm | %35,26; ABD+AB'de 260 milyar $ | Baymard, 2025 | Orta (model) |
| Checkout UX'i "vasat veya kötü" olan siteler | masaüstü %64, mobil web %63, uygulama %46 | Baymard, Kasım 2025 | Güçlü kanıt |
| Checkout UX'i "iyi" olan siteler | masaüstü %2, mobil %2, uygulama %7; "mükemmel" %0 | Baymard, 2025 | Güçlü kanıt |
| Telefon numarası vermekte isteksiz kullanıcılar | %70+ | Baymard, 2025 | Güçlü kanıt |

**Checkout'ta en sık 10 hata ve bunu yapan site oranı** (Baymard, 2025; 41.000+ performans puanı):

| Hata | Sitelerin oranı |
|---|---|
| Misafir ödeme en belirgin seçenek değil | %62 |
| Şifre kuralları gereğinden karmaşık | %65 |
| Teslimat tarihi yerine teslimat hızı yazıyor ("2–3 iş günü") | %48 |
| Kargo kesim saati için geri sayım yok | %83 |
| Adet seçici iyi tasarlanmamış | %97 |
| Kargo adımında teslimat seçenekleri eksik | %52 |
| Zorunlu ve isteğe bağlı alanlar işaretli değil | %61 |
| İsteğe bağlı girdi için yanlış arayüz kullanılmış | %32 |
| Hata mesajları genel, duruma uyarlanmamış | %94 |
| Telefon neden zorunlu, açıklanmıyor | %49 |

**Form alanı uygulamaları** (Baymard, 2024):

| Uygulama | Uygulamayan site oranı |
|---|---|
| Ad ve soyad tek alanda | %89 |
| "Adres satırı 2" gizli | %75 |
| Hesap oluşturma sona erteleniyor | %84 |
| Kupon alanı gizli | %35 |
| Fatura adresi alanları gizli ("teslimatla aynı") | %24 |

### Kılavuz maddeleri
- Kullanılabilirlik açısından adım sayısından çok **görünen form alanı sayısı** önemlidir. Baymard 2012'den beri ortalamanın ~5 adım olduğunu ve asıl sorunun alan kalabalığı olduğunu belirtiyor (2024).
- Misafir ödeme **buton olarak**, hesap seçimi adımının **en üstünde** ve açık bir etiketle sunulmalıdır ("Misafir olarak devam et"). "Devam" gibi belirsiz etiketler kullanılmamalı; seçenek, e-posta girildikten sonra değil **en başta** görünmelidir (Baymard, 2023). Kullanıcı seçeneği göremezse etkisi, hiç sunulmamış olmasıyla aynıdır.
- Kart alanları kenarlık, arka plan veya gölgeyle **görsel olarak kapsüllenmeli**, bu alanın içine 1–2 güven ikonu konmalıdır. Testte sahte, "ev yapımı" bir güven mührü bile bilinen SSL mühürlerinin çoğundan iyi sonuç verdi; kullanıcı algısında güven, teknik gerçekliğin önüne geçiyor (Baymard, 2023 verisi).
- Teslimatta "3–5 iş günü" yerine **somut tarih aralığı** ve kargo kesim saati verilmeli.
- Sitelerin %94'ü genel hata mesajı kullanıyor; **uyarlanabilir satır içi hata mesajı** fark yaratır.

### İyi / kötü örnek
- **İyi (desen):** Hesap seçimi ekranında en üstte tam genişlik "Misafir olarak devam et" butonu, altında daha küçük "Giriş yap" seçeneği. Hesap oluşturma, sipariş onay sayfasında "Şifre belirle, siparişini takip et" teklifiyle sunuluyor.
- **Kötü (desen):** Misafir ödeme yalnızca küçük bir metin linki. Ad ve soyad ayrı alanlarda, "Adres 2" ve "Firma adı" açıkta, kupon alanı büyük ve göz önünde. Kullanıcı kupon aramak için siteden ayrılıyor.
- **KPT notu:** Site önizlemede ve gerçek ödeme yok. Checkout akışı tasarlanırken aşağıdaki kurallar baştan uygulanmalı ([[Sepet ve Ödeme]]).

**KPT için kurallar:** 1–9 (aşağıda).

---

## 2. Ana sayfa ve kategori navigasyonu

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| Ana sayfa ve kategori navigasyonu "vasat–kötü" | masaüstü %58, mobil %67 | Baymard, 30.09.2025 (180+ site, 16.000+ puan) | Güçlü kanıt |
| Bulunulan kategoriyi navigasyonda vurgulamayan siteler | %95 | Baymard, 2025 | Güçlü kanıt |
| Ara kategori sayfalarında alt kategorileri ana içerik yapmayanlar | %76 | Baymard, 2025 | Güçlü kanıt |
| İlham görsellerinden ürünlere doğrudan bağlantı vermeyenler | %70 | Baymard, 2025 | Güçlü kanıt |
| Açılır menüde hover gecikmesi uygulamayanlar | %61 | Baymard, 2025 | Güçlü kanıt |
| Kategorileri yönetilebilir gruplara bölmeyenler | %60 | Baymard, 2025 | Güçlü kanıt |
| Mobilde ana sayfa linklerinin kapsamını netleştirmeyenler | %59 | Baymard, 2025 | Güçlü kanıt |
| Ana sayfada aşırı reklam yerleşimi | %55 | Baymard, 2025 | Güçlü kanıt |
| Alt kategori küçük görselleri eksik veya belirsiz | %55 | Baymard, 2025 | Güçlü kanıt |
| Tıklanabilir alanı belli olmayan arayüz öğeleri | %51 | Baymard, 2025 | Güçlü kanıt |
| Kategori başlıkları tıklanabilir değil | %33 | Baymard, 2025 | Güçlü kanıt |
| Gizli (hamburger) menünün kullanım oranı | masaüstü %27 (görünür menüde %48); mobil %57 (kombine menüde %86) | NN/g, 2016 (179 katılımcı) | Orta (eski ama temel) |
| Gizli navigasyonda içeriği keşfetme | %20'den fazla düşüş | NN/g, 2016 | Orta |

### Kılavuz maddeleri
- **Mega menü (NN/g, 2017):** İmleç 0,5 sn hareketsiz kalınca menü açılmalı, 0,1 sn içinde görünmeli. İmleç alandan çıkınca menü 0,5 sn sonra kapanmalı. Menüye doğru çapraz hareket ("diagonal problem") menüyü kapatmamalı. Menünün tamamı kaydırma gerektirmeden görünmeli. Üst seviye öğeler de tıklanabilir olmalı ve kendi sayfalarına götürmeli. Her seçenek menüde yalnızca bir kez yer almalı.
- **Hedef kitleye göre navigasyon (NN/g, 2015):** Kategoriler birbirini dışlıyorsa, jargonsuzsa ve gruplar arası geçiş kolaysa kabul edilebilir. Giyim ve ayakkabıda Erkek/Kadın/Çocuk ayrımı ürünün kendi özelliğidir, birbirini dışlar ve sektörde beklenen bir yapıdır. Yine de **Marka** ve **Kategori** yolları da sunulmalı; unisex ürünler her iki tarafta görünmeli. (Uyarlama: NN/g'nin genel uyarısının giyim bağlamına uygulanması.)
- **Mobil:** Gizli navigasyon keşfedilebilirliği düşürür. Ana kategoriler mümkünse görünür kalmalı: ana sayfada yatay kaydırılabilir kategori çipleri ve alt sekme çubuğu kullanılmalı (NN/g, 2015–2016).

### İyi / kötü örnek
- **İyi (desen):** Masaüstünde "Erkek" üzerine gelince 0,5 sn sonra açılan mega menü. Sütunlar: "Ayakkabı" (Sneaker, Koşu, Basketbol, Terlik), "Giyim" (Mont, ...), "Markalar" (7 logo/metin), "Öne çıkan" (1 görsel kart ve bağlantısı).
- **Kötü (KPT mevcut):** Erkek/Kadın/Çocuk menüsü yok. Kullanıcı yalnızca ana sayfa ızgarası ve filtrelerle ilerleyebiliyor ([[KPT Store Denetimi]]).
- **Kötü (desen):** Kategori başlığı tıklanamıyor, yalnızca alt öğeler link. Kullanıcı "Tüm Erkek Ayakkabıları" sayfasına ulaşamıyor.

**KPT için kurallar:** 10–14 ([[Header ve Navigasyon]]).

---

## 3. Ürün listeleme sayfası (PLP): filtreler, çipler, sıralama, ürün kartı, sayfalama

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| PLP UX'i "zayıf–vasat" | masaüstü %58, mobil %78 | Baymard, 09.09.2025 (170+ site, 21.000+ parametre) | Güçlü kanıt |
| PLP'lerinde ciddi kullanılabilirlik kusuru olan siteler | %80 | Baymard, 20.08.2026 | Güçlü kanıt |
| 5 temel filtrenin (fiyat, puan, renk, beden, marka) hepsini sunmayanlar | %51 | Baymard, 2025 | Güçlü kanıt |
| 4 temel sıralamanın (fiyat, puan, en çok satan, en yeni) hepsini sunmayanlar | %69 | Baymard, 2025 | Güçlü kanıt |
| Aynı filtre türünde birden çok değer seçtirmeyenler | %14 | Baymard, 2025 | Güçlü kanıt |
| Uygulanan filtrelerin özetini göstermeyenler | %20 (2025 özeti); %28 (PLP makalesi, 2026); **mobilde %66** | Baymard, 2025–2026 | Güçlü kanıt (ölçüm kapsamları farklı) |
| Ürün varyasyonlarını tek kartta birleştirmeyenler | %42 | Baymard, 2025 | Güçlü kanıt |
| Listede 3'ten fazla ürün küçük görseli sunmayanlar | %80 | Baymard, 2025 | Güçlü kanıt |
| Mobilde eksik renk swatch'ları | %73 | Baymard Mobil, 2026 | Güçlü kanıt |
| Yatay filtre çubuğu kullanan siteler | %24 (2020'den beri sabit) | Baymard, Mart 2025 | Güçlü kanıt |
| Beden filtresi en üstte ve açıkken önce bedene göre filtreleyenler | %90 (Levi's testi) | Baymard, Haziran 2024 | Orta (tek site) |
| Ürünün kendi bedeninde olmadığını PDP'de öğrenenler | %39 | Baymard, 2024 | Orta |
| "Daha fazla yükle" butonu olan sitelerde geri dönüşte kaydırma konumunu korumayanlar | %90'dan fazla | Baymard / Smashing, 2016 | Orta (eski) |

### Kılavuz maddeleri
- **Filtre türleri:** Fiyat, renk, beden ve marka temel filtrelerdir. Puan filtresi, yorum verisi olduğunda eklenir. Bunlara kategoriye özgü filtreler eklenir; sneaker için kullanım (koşu, günlük, basketbol), cinsiyet, taban veya teknoloji. Her seçeneğin yanında **sonuç sayısı** gösterilmeli ve çoklu seçim mümkün olmalı (Baymard, 2026).
- **Beden filtresi:** Kenar çubuğunda en üstte (ya da kapalı bir Kategori filtresinin hemen altında), varsayılan olarak **açık** ve **ızgara** düzeninde olmalı. Açılır liste veya dikey liste kullanılmamalı (Baymard, 2024).
- **Uygulanan filtreler:** Ürün ızgarasının üstünde, tek tek kaldırılabilen çipler halinde ve yanında "Tümünü temizle" bağlantısıyla gösterilmeli (Baymard, 2026).
- **Yatay filtre çubuğu:** Ancak 6–8 filtreye kadar iş görür. Daha fazlası için kenar çubuğu daha güvenilir bir yapıdır (Baymard, 2025).
- **Sayfalama, "daha fazla yükle" ve sonsuz kaydırma:** Baymard'ın güncel önerisi **"Daha fazla yükle" + makul büyüklükte gruplar** (2026). 2016 testinde sonsuz kaydırmada kullanıcılar en çok ürünü gördü ama footer'a hiç ulaşamadılar; sayfalamada en az ürün görüldü. Öneri: masaüstü kategoride 10–30 ürünü tembel yükle, 50–100 üründen sonra buton göster. Arama sonuçlarında varsayılan 25–75 ürün kullan, **sonsuz kaydırma kullanma**. Mobilde 15–30 ürün sonra buton (Baymard/Smashing, 2016). PDP'den dönen kullanıcı listede **kaldığı yere** dönmeli.
- **Ürün kartı:** Görsel, marka ve model adı, fiyat (indirimde eski fiyatın üstü çizili), renk sayısı veya swatch, en fazla bir anlamlı rozet. Ürün özellikleri başlıktan ayrı satırda ve tutarlı biçimde yazılmalı (Baymard, 2026).
- **Rozetler:** Yalnızca karar değiştirecek bilgi için kullanılmalı ("Yeni", "İndirim", "Çok satan", "Az stok"). Listede ürünlerin çoğunda rozet varsa rozetler sinyal değerini kaybeder. Kampanya iç adları rozet metni olmamalı (Baymard, Eylül 2026).
- **Mobil:** Sabit (sticky) "Filtrele" butonu ve alttan açılan filtre çekmecesi kullanılmalı (Baymard, 2026).

### İyi / kötü örnek
- **İyi (Baymard'ın örneği):** Levi's beden filtresini kenar çubuğunun üstünde, açık ve ızgara halinde gösteriyor; katılımcıların %90'ı önce bedene göre filtreledi (2024).
- **Kötü (KPT mevcut):** Kategori filtreleri tek seçimli açılır menü ve ham tedarikçi renk verisi içeriyor. "Lacivert/Beyaz-Gri" gibi yüzlerce benzersiz değer oluşuyor, renk filtresi işe yaramaz hale geliyor ([[KPT Store Denetimi]]).
- **Kötü (desen):** Sonsuz kaydırmalı PLP'de footer'daki "İade koşulları" bağlantısına ulaşılamıyor. Ürüne girip geri dönen kullanıcı listenin başına atılıyor.

**KPT için kurallar:** 15–24 ([[Kategori Sayfası ve Filtreler]]).

---

## 4. Ürün sayfası (PDP)

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| PDP UX'i "vasat veya kötü" | masaüstü %52, mobil %62, uygulama %64 | Baymard, güncelleme 18.03.2026 (155+ site) | Güçlü kanıt |
| Beden seçiminde buton kullanmayanlar | %57 (tüm PDP'ler); %70 (giyim) | Baymard, 2026 / 2025 | Güçlü kanıt |
| "Ölçekli" (in-scale) görseli olmayanlar | %37 (2026); %28 (2017, 60 büyük site) | Baymard | Güçlü kanıt |
| İnsan model görseli olmayanlar | %23 (PDP genel); %21 (giyim) | Baymard, 2026 / 2025 | Güçlü kanıt |
| Yeterli beden bilgisi sunmayan giyim siteleri | %82 | Baymard, Şubat 2025 | Güçlü kanıt |
| Toplu "kalıp" (fit) alt puanı sunmayanlar | %24 | Baymard, 2025 | Güçlü kanıt |
| Yorumlar arasında yorumcu görselleriyle gezinme sunmayanlar | %90 (giyim); %63 (genel) | Baymard, 2025–2026 | Güçlü kanıt |
| Olumsuz yorumlara yanıt vermeyenler | %89 | Baymard, 2026 | Güçlü kanıt |
| İade politikasını belirgin göstermeyenler | %44 | Baymard, 2026 | Güçlü kanıt |
| Toplam sipariş maliyeti tahmini sunmayanlar | %67 | Baymard, 2026 | Güçlü kanıt |
| PDP'deki ilk eylemi görselleri incelemek olan kullanıcılar | %56 | Baymard, 2020 | Orta |
| Ürünün boyutunu görsellerden anlamaya çalışanlar | %42 | Baymard, 2017 | Orta |
| Görsel çözünürlüğü veya zoom'u yetersiz olanlar | %25 | Baymard, 2020 | Orta |
| Ana ürün bölümlerinde yatay sekme kullananlar | %29 | Baymard, güncelleme 08.07.2026 | Güçlü kanıt |
| Teknik özellik tablosu "zayıf–vasat" | %64; benzer ürünler arasında ciddi tutarsızlık %30 | Baymard, 24.09.2026 | Güçlü kanıt |
| Stokta olmayan ürüne rastlayınca başka siteye gidenler | %30 | Baymard, 2017 (2025'te güncellendi) | Orta |
| Geçici olarak stokta olmayan ürüne sipariş aldırmayanlar | %68 | Baymard, 2025 | Güçlü kanıt |
| Ziyaretlerin PDP'de başlama oranı | 3 ziyaretten 1'i; PDP ziyaretlerinin %61'i hemen çıkıyor | Contentsquare, 2026 | Güçlü kanıt |
| Yorumlu ürünlerde satın alma olasılığı (5 yorum, yorumsuza göre) | %270 daha yüksek; pahalı üründe %380 | Spiegel Research Center, 2017 | Orta (eski) |
| Satın alma olasılığının zirve yaptığı puan aralığı | 4,0–4,7 yıldız (5,0'a yaklaştıkça düşüyor) | Spiegel, 2017 | Orta |
| "Doğrulanmış alıcı" rozetinin etkisi | Satın alma olasılığı +%15 | Spiegel, 2017 | Orta |
| Mobil sticky "Sepete ekle" A/B testi (AFTCO) | Dönüşüm +%6,2, sepete ekleme +%3,9 | Clean Commit, 2025 | Zayıf (ajans, örneklem açıklanmamış) |
| Mobil sticky "Sepete ekle" A/B testi (isimsiz Shopify mağazası) | Sepete ekleme +%6,8 ama dönüşüm −%7,7, ziyaretçi başı gelir −%22,1 (sonuçsuz) | Clean Commit, 2025 | Zayıf |

### Kılavuz maddeleri
- **Görseller:** Ölçekli görsel türleri: ürün insan üzerinde, kullanım ortamında, boyutu bilinen bir nesnenin yanında, elde tutulurken, kullanılırken (Baymard, 2017). Ayakkabıda bunun karşılığı **ayakta (on-foot) görseldir**. Yaşam tarzı görseli ölçekli görselin yerini tutmaz. Baymard'a göre bilgisayarla üretilmiş görseller gerçek fotoğrafı **tamamlamalı, yerine geçmemeli** (2017).
- **Açıklama yapısı:** Yatay sekme kullanılmamalı. Kullanıcı içeriğe dikey kaydırarak ulaşacağını varsayar ve sayfa kaydırılınca sekmeler görünmez olur. Masaüstünde bölümler açık durmalı (isteğe bağlı sabit içindekiler), mobilde dikey akordeon kullanılmalı (Baymard, 2026). Teknik özellik tablosu tek sütunlu olmalı: etiket solda, en önemli özellikler önce, satırlar dönüşümlü arka planla ayrılmalı. Birimler hep yazılmalı ve aynı kategoride etiketler ile sıra tutarlı olmalı (Baymard, Eylül 2026).
- **Beden bilgisinin 10 bileşeni** (Baymard, 2025): geleneksel ve sayısal beden, inç **ve** cm ölçüleri, uluslararası dönüşüm, ölçü alma talimatı, seçicinin yanında beden rehberi linki, rehberin içinde müşteri hizmetleri linki ve benzerleri. Toplu "kalıp" puanı ("küçük – tam – büyük" çubuğu) yüzlerce yorumu okuma ihtiyacını ortadan kaldırır.
- **Beden seçici:** Butonlar açılır listeden iyidir. Açılır liste stok durumunu gizler ve seçeneklerin gözden kaçmasına yol açar (Baymard #850, 2026). Stokta olmayan bedenler **gizlenmemeli**. Gösterim biçiminin ayrıntıları Baymard Premium'da; ücretsiz kaynaklarda net bir yönerge bulunamadı. Kural 26'daki görsel stil (üstü çizili, soluk ve tıklanabilir) bu ilkelerden türetilmiş bir uygulamadır `(tahmin)`.
- **Bedene göre değişen fiyat:** Baymard'ın "listede ürün varyasyonları" yönergesi (#421, Temmuz 2026) varyasyonların tek kartta birleştirilmesini istiyor. Fiyat aralığının nasıl gösterileceği Premium içerik. Kural 30'daki "…'dan başlayan" deseni, toplam maliyeti erken gösterme ilkesinden türetilmiştir `(tahmin)`.
- **Stok dışı:** Geçici stoksuzlukta uzun teslim süresiyle sipariş alınmalı. Kalıcı olarak satıştan kalkan ürün sayfanın üstünde açıkça "Satıştan kalktı" diye işaretlenmeli ve alternatifler öne çıkarılmalı. "Stoğa gelince haber ver" tek başına yetersizdir; kullanıcı hemen alternatif görmek ister (Baymard, 2025).
- **Sticky "Sepete ekle":** Kanıtlar karışık. Bir ajans testi kazandı, bir başkası dönüşümde düşüş gösterdi (2025). Mobilde CTA'nın sürekli erişilebilir olması mantıklı, fakat **A/B testiyle doğrulanmalı** ve beden seçimi atlanmamalı.

### İyi / kötü örnek
- **İyi (Baymard'ın örneği):** Home Depot'nun tek sütunlu, alt başlıklı özellik tablosu; Best Buy'ın dönüşümlü satır renkleri ve teknik terimler için ipuçları; Lowe's'un mobilde katlanır bölümleri (Baymard, 2026).
- **Kötü (KPT mevcut):** Yalnızca stoktaki bedenler gösteriliyor, açıklama boş. Butonun yanında teslimat, iade ve taksit bilgisi yok. Mobilde sticky sepete ekle çubuğu yok ([[KPT Store Denetimi]]).

**KPT için kurallar:** 25–35 ([[Ürün Sayfası]], [[Beden ve Kalıp]], [[Güven Sinyalleri]]).

---

## 5. Site içi arama

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| Arama ihtiyacını yeterince karşılamayan siteler | %56 ("iyi" veya "makul" %44) | Baymard, güncelleme 29.04.2026 (170+ site) | Güçlü kanıt |
| Arama UX'i "vasat veya kötü" | masaüstü %46, mobil %58, uygulama %64 | Baymard, 2026 | Güçlü kanıt |
| Sorgu türüne göre sorunlu siteler | tam ad %12, ürün türü %20, semptom %37, özellik %39, kullanım amacı %43, uyumluluk %44, kısaltma/sembol %54, ürün dışı %66 | Baymard, 2026 | Güçlü kanıt |
| Aramayı ürün bulmada tercih eden kullanıcılar | yaklaşık yarısı (diğer yarısı menüyü kullanıyor) | Baymard, 2026 | Güçlü kanıt |
| Otomatik tamamlama sunan siteler | %80 (2014'te %72); tam uygulayanlar %19 | Baymard, 2022 | Orta |
| Yazım hatalı sorgularda öneri sunmayanlar | %69 (2021); mobilde %28 (2026 mobil benchmark) | Baymard | Orta (iki ölçüm çelişiyor, aşağıya bkz.) |
| Mobilde arama "gönder" butonu olmayanlar | %27 | Baymard Mobil, 2026 | Güçlü kanıt |
| Sonuçsuz aramadan etkili çıkış yolu sunmayanlar | yaklaşık %50 | Baymard, güncelleme 18.02.2025 | Güçlü kanıt |
| "Sonuç yok" sayfası çıkmaz sokak olanlar (yalnızca genel arama ipuçları) | %68 | Baymard (eski ölçüm, ikincil aktarım) | Zayıf |

### Kılavuz maddeleri
- **Otomatik tamamlama** (Baymard, 2022): Masaüstünde en fazla 10, mobilde 4–8 öneri, en az 4. Masaüstünde kaydırma çubuğu olmamalı. Kullanıcının **yazmadığı** tamamlanan kısım vurgulanmalı. Kategori kapsamlı öneriler farklı biçimde gösterilmeli ("koşu ayakkabısı — *Erkek* içinde"). Aktif öneri arka planla vurgulanmalı; ok tuşlarıyla gezinilmeli, Enter ile gönderilmeli. Mobilde sabit header, sohbet balonu ve "uygulamayı indir" bandı gibi rakip öğeler azaltılmalı; satırlar arasında ayırıcı çizgi ve geniş dokunma alanı olmalı.
- **Yazım hatası:** Kullanıcı hatalı yazınca dört tepkiden biri görülüyor: fark edip hızlıca düzeltiyor, 30 sn'den fazla uğraşıyor, aramayı bırakıp kategori menüsüne geçiyor ya da siteyi terk ediyor (Baymard, 2021). Çözüm: yazım denetimi ve arama loglarından sık hataları elle eşlemek.
- **Sonuç yok sayfası** (Baymard, 2025): İlgili kategoriler, ürün önizlemeli alternatif sorgular, son görüntülenen ürünler, müşteri hizmetleri (telefon ve canlı destek) ve popüler ürünler gösterilmeli. "Arama ipuçları" tek başına işe yaramaz.

### İyi / kötü örnek
- **İyi (desen):** "nıke aır" yazınca otomatik tamamlama "**Nike Air** Max" önerisini, 3 ürün kartını ve "Erkek Sneaker içinde" kapsam önerisini gösteriyor.
- **Kötü (desen):** "new balans" için "0 sonuç bulundu. Yazımınızı kontrol edin" mesajı; başka hiçbir yol sunulmuyor.

**KPT için kurallar:** 36–39 ([[Arama]]).

---

## 6. Mobil e-ticaret

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| Mobil trafik payı | %69,9 (masaüstü ~%30 ama zamanın %47'si) | Contentsquare, Mart 2026 (6.000+ site, 99 milyar oturum) | Güçlü kanıt |
| Dönüşüm oranı masaüstü / mobil | %3,4 / %2,0 (masaüstü %74–75 yüksek); perakendede %3,7 / %2,0 | Contentsquare, 2026 | Güçlü kanıt |
| Oturum süresi masaüstü / mobil | 4:46 / 2:20 dk | Contentsquare, 2026 | Güçlü kanıt |
| Kaydırma oranı masaüstü / mobil | %50,5 / %45,2 | Contentsquare, 2026 | Güçlü kanıt |
| Dünya e-ticaretinde mobil payı | ~%59 (2025 projeksiyonu) | Statista'ya atfen ikincil kaynaklar | Zayıf |
| Mobil UX'i "vasat" olan siteler | %75 ("vasat" veya "makul" %95; "iyi" yalnız 1 site) | Baymard Mobil, güncelleme 14.07.2026 (150+ site) | Güçlü kanıt |
| Telefonu tek elle kullananlar | %49 (kucaklama %36, iki el %15); tek elde sağ başparmak %67 | Hoober / UXmatters, 2013 (1.333 gözlem) | Orta (eski ama temel) |
| WCAG 2.2 hedef boyutu (2.5.8, AA) | en az 24×24 CSS px veya 24 px çaplı boşluk dairesi | W3C, 2023 | Güçlü kanıt |
| WCAG 2.5.5 (AAA) | 44×44 CSS px | W3C | Güçlü kanıt |
| Android önerisi | 48×48 dp, aralık ≥8 dp (~9 mm) | Google Android Erişilebilirlik Yardımı | Güçlü kanıt |
| iOS önerisi | 44×44 pt | Apple HIG (bu oturumda sayfa metni okunamadı) | Orta |
| NN/g önerisi | en az 1×1 cm | NN/g, 2019 | Orta |
| Alt sekme çubuğu öğe sayısı | 4–5'i geçmemeli | NN/g, 2015 | Orta |

### Kılavuz maddeleri
- Mobil trafiğin %70'ini, gelirin ise daha küçük bir kısmını getiriyor. Mobildeki dönüşüm farkı en büyük fırsat alanıdır ([[Mobil Deneyim]]).
- Alt sekme çubuğu sürekli görünür ve gizli menüden daha keşfedilebilirdir. Gizli menüde içerik keşfi %20'den fazla düşer (NN/g, 2016).
- "Başparmak bölgesi": Tek elle kullanım yaygın (%49). Birincil eylemler (sepete ekle, filtrele, ödeme) ekranın alt üçte birinde olmalı (Hoober, 2013 verisinden çıkarım).
- Dokunma hedeflerinde yasal alt sınır 24 px'tir (WCAG AA). Pratik hedef 44–48 px ve aralarında en az 8 px boşluk.
- Mobilde arama gönder butonu, renk swatch'ları ve uygulanan filtre özeti en sık atlanan öğeler (Baymard, 2026).

**KPT için kurallar:** 40–42.

---

## 7. Performans ve dönüşüm (Core Web Vitals)

### Eşikler (75. yüzdelik dilim, mobil ve masaüstü ayrı ölçülür)

| Metrik | İyi | Geliştirilmeli | Kötü | Not |
|---|---|---|---|---|
| LCP (en büyük içerik boyaması) | ≤2,5 sn | 2,5–4,0 sn | >4,0 sn | Yükleme |
| INP (etkileşimden sonraki boyamaya kadar geçen süre) | ≤200 ms | 200–500 ms | >500 ms | 2024'te FID'in yerini aldı |
| CLS (kümülatif düzen kayması) | ≤0,1 | 0,1–0,25 | >0,25 | Görsel kararlılık |

Kaynak: web.dev, "Web Vitals" (iyi eşikleri ve p75 kuralı doğrulandı; ara eşikler web.dev'in standart sınıflandırmasıdır). `Güçlü kanıt`

### Güncel rakamlar ve vaka çalışmaları

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| Core Web Vitals'ı geçen originler | mobil %36 → %44 → %48 (2023→2025); masaüstü %48 → %55 → %56 | Web Almanac, Ocak 2026 | Güçlü kanıt |
| 2025'te metrik bazında "iyi" oranı (mobil) | LCP %62, INP %77, CLS %81 | Web Almanac, 2025 | Güçlü kanıt |
| LCP öğesi görsel olan sayfalar | masaüstü %85,3, mobil %76 | Web Almanac, 2025 | Güçlü kanıt |
| LCP görselini tembel yükleyen (lazy) sayfalar | ~%16–17 (hata) | Web Almanac, 2025 | Güçlü kanıt |
| Görsel formatları | JPG %57, PNG %26, WebP %11 | Web Almanac, 2025 | Güçlü kanıt |
| Mobil hızda 0,1 sn iyileşmenin etkisi | perakende dönüşüm +%8,4, AOV +%9,2; seyahat dönüşüm +%10,1; lüks sayfa görüntüleme +%8,6 | Deloitte/55/Google, 2020 (37 marka, 30 milyon+ oturum) | Orta (korelasyonel) |
| Rakuten 24 A/B (CWV optimizasyonu) | ziyaretçi başı gelir +%53,37, dönüşüm +%33,13, AOV +%15,20, çıkış oranı −%35,12; CLS %92,72 iyileşti | web.dev, 2022 | Orta (tek vaka, A/B) |
| Vodafone A/B | LCP %31 iyileşti, satış +%8, sepet/ziyaret +%11 | web.dev, 2021 | Orta |
| **Trendyol** (Türkiye) PLP'de INP | 963 ms → ~650 ms (−%50), PLP'den PDP'ye tıklama +%1 | web.dev, Aralık 2023 | Orta (tek vaka) |
| redBus INP | −%72, satış +%7 | web.dev, 2023 | Orta |
| The Economic Times INP | yaklaşık 4 kat iyileşme, hemen çıkma −%50 | web.dev (arama özetinden) | Zayıf (bu oturumda doğrudan okunmadı) |
| Yükleme süresine göre e-ticaret dönüşümü | 1 sn %3,05; 2 sn %1,68; 3 sn %1,12; 4 sn %0,67; 1 sn'deki site 5 sn'dekinden 2,5 kat fazla dönüştürüyor | Portent, 2022 (6 B2C site, 5,6 milyon oturum) | Orta |
| 100 ms gecikmenin etkisi | dönüşüm −%7; 2 sn gecikme hemen çıkmayı %103 artırıyor | Akamai, 2017 (~10 milyar ziyaret) | Orta (eski) |
| 3 sn'den uzun yüklemede mobil terk | %53 | Akamai 2017'de aktarılan, aslen Google 2016 | Zayıf |

### Kılavuz maddeleri
- LCP'nin bileşenleri ve hedef payları: TTFB ~%40, kaynak yükleme gecikmesi <%10, kaynak yükleme süresi ~%40, öğe render gecikmesi <%10 (web.dev). LCP görseli ilk HTML'de keşfedilebilir olmalı ve `fetchpriority="high"` almalı. LCP görselinde **asla** `loading="lazy"` kullanılmamalı. AVIF veya WebP ile görsel CDN tercih edilmeli.
- INP için uzun görevler `scheduler.yield()` (yoksa `setTimeout`) ile bölünmeli. Kaydırma işleyicilerine debounce uygulanmalı. Tembel yükleme grupları küçültülmeli: redBus 30 yerine 10 sonuç yükledi (web.dev, 2023).
- CLS için görsellere `width`/`height` veya `aspect-ratio` verilmeli. Sonradan yerleşen bant ve banner'lar için yer önceden ayrılmalı.
- **KPT sorunu:** Hero görseli 900 KB PNG ([[KPT Store Denetimi]]). Web Almanac'a göre mobilde LCP öğesinin %76'sı bir görsel; KPT'de LCP öğesi büyük olasılıkla bu hero `(tahmin)`.

**KPT için kurallar:** 43–46.

---

## 8. Erişilebilirlik: WCAG 2.2 AA, EAA, Türkiye Genelgesi ve iş etkisi

### Mevzuat

| Düzenleme | KPT'ye etkisi | Kaynak | Güven |
|---|---|---|---|
| **T.C. Cumhurbaşkanlığı Genelgesi 2025/10**, "Web Siteleri ve Mobil Uygulamaların Erişilebilirliği" (Resmî Gazete, 21.06.2025, sayı 32933) | E-ticaret hizmet sağlayıcıları kapsamda; **2 yıl** içinde (→ **21 Haziran 2027**) uyum gerekiyor. Referanslar: WCAG 2.2 ve Aile ve Sosyal Hizmetler Bakanlığı'nın "Kontrol Listesi – A Seviyesi". Uyumlu sitelere 2 yıllık "Erişilebilirlik Logosu" veriliyor. | Erdem & Erdem, ikas, Webrazzi, Lexpera (2025) | Güçlü kanıt (mevzuat); kapsam eşikleri belirsiz |
| **AB Erişilebilirlik Yasası (EAA)**, Direktif (AB) 2019/882 | 28 Haziran 2025'ten beri uygulanıyor; e-ticaret hizmetlerini kapsıyor. AB dışı satıcılar da AB tüketicisine satış yapıyorsa kapsamda. Hizmet sunan mikro işletmeler (<10 çalışan **ve** ≤2 milyon € ciro) muaf. Teknik referans EN 301 549 (web için WCAG 2.1 AA). Öncesinde kullanılan ürünlerle hizmet sunumu için geçiş süresi 28 Haziran 2030'a kadar. | AB Komisyonu (kapsam); ikincil hukuk ve uyum kaynakları (eşikler, standart, tarihler) | Orta (EUR-Lex metni bu oturumda okunamadı) |

KPT yalnızca Türkiye'ye TRY ile satıyorsa EAA doğrudan uygulanmaz. Türkiye Genelgesi ise uygulanır. Genelge A seviyesine atıf yapsa da bu kasa **WCAG 2.2 AA'yı** hedef kabul eder: hem EAA hem sektör pratiği AA düzeyinde.

### WCAG 2.2'de yeni kriterler (W3C, 5 Ekim 2023)

| No | Ad | Seviye | E-ticaret karşılığı |
|---|---|---|---|
| 2.4.11 | Focus Not Obscured (Minimum) | AA | Klavye odağı sabit header, sticky ATC veya çerez bandının altında **tamamen** kaybolmamalı |
| 2.4.13 | Focus Appearance | AAA | Odak göstergesi ≥2 px kalınlıkta ve odaklı/odaksız durumlar arasında 3:1 kontrastta |
| 2.5.7 | Dragging Movements | AA | Fiyat kaydırıcısı, karusel ve 360° görüntüleyici sürükleme olmadan da kullanılabilmeli |
| 2.5.8 | Target Size (Minimum) | AA | Hedefler ≥24×24 px ya da 24 px'lik boşluk dairesine sahip; satır içi linkler muaf |
| 3.2.6 | Consistent Help | A | Yardım ve iletişim kanalları her sayfada aynı göreli sırada |
| 3.3.7 | Redundant Entry | A | Daha önce girilen bilgi tekrar istenmemeli: fatura adresi = teslimat adresi |
| 3.3.8 | Accessible Authentication (Minimum) | AA | Girişte bilişsel test olmamalı; şifre yapıştırma ve şifre yöneticisi desteklenmeli |
| 4.1.1 | Parsing | — | WCAG 2.2'de kaldırıldı |

Mevcut kriterlerden e-ticarette kritik olanlar: 1.1.1 metin alternatifi (ürün görselleri), 1.4.3 metin kontrastı 4,5:1 (devre dışı bileşenler muaf), 1.4.11 metin dışı kontrast 3:1 (buton ve girdi kenarları, seçili beden), 2.2.2 Duraklat/Durdur/Gizle (5 sn'den uzun süren otomatik hareket), 2.1.1 klavye, 3.3.1–3.3.3 hata tanımlama ve öneri, 4.1.2 ad/rol/değer (özel beden seçicileri).

### Güncel rakamlar ve iş etkisi

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| WCAG hatası tespit edilen ana sayfalar | %95,9 (2025: %94,8); sayfa başına 56,1 hata | WebAIM Million, Şubat 2026 | Güçlü kanıt |
| Alışveriş kategorisinde sayfa başına hata | 71,0 (ortalamanın %26,6 üstü) | WebAIM, 2026 | Güçlü kanıt |
| En sık hatalar | düşük kontrast %83,9, eksik alt metin %53,1, etiketsiz form girdisi %51, boş link %46,3, boş buton %30,6, belge dili yok %13,5 (bu 6 tür hataların %96'sı) | WebAIM, 2026 | Güçlü kanıt |
| Önemli düzeyde engelli nüfus | 1,3 milyar (%16, her 6 kişiden 1'i) | DSÖ, 2023 | Güçlü kanıt |
| Zorlandıkları siteyi terk eden engelli çevrimiçi alışverişçiler | %69; Birleşik Krallık'ta 17,1 milyar £ kayıp | Click-Away Pound, 2019 | Orta (eski, BK) |
| Erişilebilir olduğunu bildiği sitelerden alışveriş yapanlar | %83; erişilebilir siteden daha pahalıya alanlar %86 | Click-Away Pound, 2019 | Orta |

### KPT renk paleti kontrast hesabı (WCAG formülüyle hesaplandı)

| Ön plan / arka plan | Oran | Sonuç |
|---|---|---|
| #171B1C / #F3F4F1 | 15,72:1 | AA/AAA geçer |
| #171B1C / #E5E8E3 | 14,04:1 | geçer |
| #741E32 / #F3F4F1 | 9,63:1 | geçer (metin ve odak halkası için uygun) |
| #FFFFFF / #741E32 | 10,64:1 | geçer (bordo dolgu butonda beyaz metin) |
| #5C615A / #F3F4F1 | 5,74:1 | ikincil metin için uygun |
| #6B7069 / #F3F4F1 | 4,59:1 | sınırda geçer; #E5E8E3 üstünde 4,10:1 **kalır** |
| #7A7F77 / #F3F4F1, #E5E8E3, #FFFFFF | 3,71 / 3,31 / 4,09 | metin dışı kenarlık (1.4.11 için ≥3:1) |
| #8A8F87 / #F3F4F1 | 2,99:1 | kenarlık olarak **kalır** |

**KPT için kurallar:** 47–53 ([[Renk ve Tipografi]], [[Footer]]).

---

## 9. Karuseller, otomatik oynayan hero'lar, pop-up ve çerez pencereleri

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| Ana sayfasında karusel olan büyük siteler (masaüstü) | %33 | Baymard, güncelleme 03.04.2025 | Güçlü kanıt |
| Karuseli olan sitelerde kullanılabilirlik sorunu | %46 (navigasyon benchmark'ında hatalı uygulama oranı %32) | Baymard, 2025 | Güçlü kanıt |
| Otomatik geçiş süresi önerisi | az metinli slaytta 5–7 sn, metin ağırlıklı slaytta 10 sn'ye kadar; mobilde otomatik dönme **yok** | Baymard, 2025 | Güçlü kanıt |
| Kullanıcıların en çok nefret ettiği reklam teknikleri | modal pop-up, otomatik video, içeriği kaydıran içerik içi reklam, içerik gibi görünen aldatıcı linkler (ortalama 7 üzerinden 5,23; mobilde 5,45) | NN/g, 2017 (452 kişi) | Orta |
| Otomatik dönen karusel sorunları | içerik geçiyor diye bulunamıyor, reklam körlüğü, okuma süresi yetmiyor, motor becerisi düşük kullanıcı tıklayamıyor | NN/g, 2013 | Orta (eski ama temel) |
| Çerez izin kullanıcı tipleri | Reddeden, Şüpheci, Teknoloji meraklısı, Sabırsız ("Tümünü kabul"), Hevesli | NN/g, Kasım 2023 | Orta |

### Kılavuz maddeleri
- **Karusel (Baymard, 2025):** Kontroller ilk bakışta fark edilmeli, iki yanda olmalı ve zeminle kontrast oluşturmalı. Masaüstünde hover'da durmalı ve kullanıcı etkileşiminden sonra **kalıcı olarak** durmalı. Mobilde kaydırma (swipe) desteklenmeli, otomatik dönme olmamalı. Görselin içine gömülü yazı yerine HTML metin kullanılmalı.
- **WCAG 2.2.2 (A):** Otomatik başlayan ve 5 sn'den uzun süren hareket (dönen ayakkabı animasyonu dahil) için duraklatma, durdurma veya gizleme mekanizması zorunlu.
- **Pop-up:** Google, içeriği engelleyen promosyon geçiş ekranlarını (interstitial) önermiyor. Çerez onayı ve yaş doğrulaması gibi yasal zorunluluklar ile küçük bantlar kabul edilebilir (Google Search Central). NN/g'ye göre modal pop-up en nefret edilen teknik.
- **Çerez bandı (NN/g, 2023):** Üç seçenek aynı anda sunulmalı: "Tümünü kabul et", "Yalnızca zorunlu" ve "Ayarları yönet". Kabul butonu diğerlerinden daha belirgin yapılmamalı ve kapatma düğmesi belirsiz olmamalı. Bant küçük tutulmalı (NN/g üstte konumlandırmayı tercih ediyor). Aynı anda birden fazla katman (çerez + bülten + sohbet) gösterilmemeli. Türk mevzuatı (KVKK çerez rehberi) bu notta doğrulanmadı; [[Güven Sinyalleri]] ve hukuk incelemesine bırakıldı.

### İyi / kötü örnek
- **Kötü (NN/g'nin örneği):** Siemens karuseli 5 sn'de bir dönüyordu; kullanıcı "Okumaya vaktim olmadı, çok hızlı değişiyor" dedi (2013).
- **Kötü (KPT mevcut):** Hero'da AI ile üretilmiş, dönen ve çift pozlanmış görünen ayakkabı görseli; 900 KB PNG ([[Hero ve Banner Desenleri]]).

**KPT için kurallar:** 54–57.

---

## 10. Ürün fotoğrafçılığı: kalite, sayı, 360°, video, AR ve yapay zekâ görselleri

### Güncel rakamlar

| Bulgu | Değer | Kaynak / yıl | Güven |
|---|---|---|---|
| PDP'deki ilk eylemi görselleri incelemek olanlar | %56 | Baymard, 2020 | Orta |
| Boyutu görsellerden anlamaya çalışanlar | %42 | Baymard, 2017 | Orta |
| Ölçekli görseli olmayan siteler | %37 | Baymard, 2026 | Güçlü kanıt |
| Masaüstünde görsel zoom'u sunan siteler | %93; zoom seviyesi yetersiz %11 | Baymard, 2020 | Orta |
| Listede 3'ten fazla ürün görseli sunmayanlar | %80 | Baymard, 2025 | Güçlü kanıt |
| 3D modeli görüntüleyenlerde sepete ekleme / sipariş | +%44 / +%27; AR'da görüntüleyenlerde satın alma +%65 (Rebecca Minkoff) | Shopify blogu, 2026 (vaka tarihi belirtilmemiş) | Zayıf (satıcı vakası) |
| 3D/AR'nin iadeye etkisi | Shopify blogunda nicel veri yok, yalnızca nitel iddia | Shopify, 2026 | Bulunamadı |
| AI ile üretilmiş görsel ve güven | Kullanıcı kaynağı bilmediğinde AI görselleri stok fotoğraf kadar iyi puan aldı: güven +0,2, profesyonellik +0,2 (anlamlı değil), özgünlük +0,4 (anlamlı ama küçük). Kullanıcı AI'dan **şüphelendiğinde** siteyi daha düşük puanladı. | NN/g, 21.08.2026 (77 ABD'li yetişkin, katılımcı içi desen, 7'li ölçek, danışmanlık sitesi hero'su) | Orta (küçük örneklem; ürün görseli değil) |
| AB Yapay Zekâ Yasası, Madde 50 | Sentetik görsel üreten sistemlerin sağlayıcıları çıktıları makine tarafından okunabilir biçimde işaretlemeli. Mevcut nesneleri gerçekmiş gibi gösteren "deepfake" içerikleri kullananlar bunu açıklamalı. Uygulama tarihi: **2 Ağustos 2026**. | artificialintelligenceact.eu (Madde 50, 113) | Güçlü kanıt (sonraki değişiklik önerileri doğrulanmadı) |

### Kılavuz maddeleri
- Görsel türleri, ölçek ve insan model gereği için Bölüm 4'e bakın. Yeterli çözünürlük ve zoom olmazsa kullanıcı ürün kalitesini düşük algılar ve bazen siteyi terk eder (Baymard, 2020).
- **AI görselleri:** NN/g'nin bulgusu insan içerikli hero görselleri için geçerli. Ürün görselinde temsil doğruluğu daha kritik: renk, doku ve form gerçek ürünle uyuşmazsa beklenti boşa çıkar ve iade riski artar `(tahmin; nicel çalışma bulunamadı)`. NN/g'nin kontrol listesi: amaç ve mesaj uyumu, temsil, anatomik veya teknik hatalar (çift kontur, bozuk logo, fazla parmak), eğitim verisi ve ticari kullanım hakları, AB Yapay Zekâ Yasası kapsamında açıklama gereği.
- **Video, 360° ve AR:** 2023–2026 için bağımsız, rakamlı ve güvenilir bir çalışma bu araştırmada **bulunamadı**. Satıcı vakaları olumlu sonuç gösteriyor (Zayıf). KPT için önce statik görsel setini tamamlamak (Kural 28) daha yüksek getirili ve kanıtlı adım.

**KPT için kurallar:** 58–60 ([[Görsel Tasarım ve Trendler 2026]]).

---

## 11. Çelişkili ve eksik veriler

- **Sepet terk:** Baymard'ın listesinde %70,22 (50 çalışma), checkout araştırma sayfasında %70,19. Fark güncelleme zamanlamasından; ~%70 kullanılmalı.
- **Form alanı:** 2024 blogunda ortalama 11,3 alan; sepet terk sayfasında "ortalama ABD checkout'u 14,88 alan / 23,48 eleman". Ölçüm tanımları (eleman ile alan, örneklem) farklı. İdeal hedef her iki kaynakta da aynı: 7–8 alan.
- **Misafir ödeme:** Belirgin olmayan site oranı 2023'te %47, 2025'te %62 (benchmark kapsamı değişti). Zorunlu hesap nedeniyle terk 2022'de %24, 2025'te %18–19.
- **Terk nedenleri 2025'te düştü:** Önceki yıllarda yaygın olarak aktarılan "%48 ekstra maliyet" değeri 2025 anketinde %40. Eski rakamlar kullanılmamalı.
- **Ölçekli görsel eksikliği:** 2017'de %28 (60 site), 2026'da %37 (155+ site). **Beden butonu kullanmayan:** genel PDP'de %57, giyimde %70. **Beden bilgisi yetersiz:** 2025 güncellemesinde %82; ikincil kaynaklarda daha eski bir %94 değeri dolaşıyor.
- **Uygulanan filtre özeti eksikliği:** %20 (2025 PLP özeti), %28 (2026 PLP makalesi), %66 (mobil benchmark). Her biri farklı kapsamda ölçülmüş.
- **Yazım hatası desteği:** %69 (2021, genel) ile %28 (2026, mobil) arasında büyük fark var. Gelişme mi yoksa ölçüm farkı mı olduğu belirsiz.
- **Sticky sepete ekle:** Ajans testleri birbiriyle çelişiyor. İkincil sitelerde "Baymard 2025: %7,9 artış" diye aktarılan değerin birincil kaynağı bulunamadı; kullanılmamalı.
- **Bulunamayanlar:** bağımsız ve güncel 360°/video/AR dönüşüm ve iade verisi; AI ile üretilmiş **ürün** görsellerinin güvene etkisini ölçen nicel çalışma; Baymard'ın stok dışı varyasyon ve bedene göre fiyat gösterimine dair ayrıntılı yönergeleri (Premium); Apple HIG ve EUR-Lex sayfalarının metni (bu oturumda okunamadı); Türkiye Genelgesi'nin e-ticaret için işletme büyüklüğü eşiği.

---

## KPT için uygulama kuralları

> [!tip] Okuma biçimi
> Her kural **Kural / Neden / Kanıt** biçiminde. Px değerleri CSS px. Renkler KPT paletinden: zemin #E5E8E3/#F3F4F1, metin #171B1C, vurgu #741E32. "(öneri)" ile işaretli sayılar kaynaktaki aralıktan KPT'ye uyarlanmış değerlerdir.

### Sepet ve ödeme ([[Sepet ve Ödeme]])

1. **Kural:** Checkout'un ilk ekranında en üstte tam genişlik, 48px yükseklikte, #741E32 dolgulu ve beyaz 16px/600 Manrope "Üye olmadan devam et" butonu olmalı. Altında #171B1C 1px çerçeveli "Giriş yap" butonu yer almalı. Hesap oluşturma, sipariş onay sayfasında yalnızca şifre alanıyla teklif edilmeli.
   **Neden:** Görülmeyen misafir seçeneği hiç sunulmamış gibidir.
   **Kanıt:** Sitelerin %62'si misafir ödemeyi öne çıkarmıyor; kullanıcıların %18–19'u zorunlu hesap yüzünden terk ediyor (Baymard, 2025) — Güçlü kanıt.
2. **Kural:** Sepet çekmecesinde ve sepet sayfasında "Ara toplam / Kargo / Toplam" satırları gösterilmeli. Kargo "Ücretsiz" ya da somut tutar olmalı, "ödeme adımında hesaplanır" yazılmamalı. Ücretsiz kargo eşiği varsa ilerleme çubuğuyla gösterilmeli: "Ücretsiz kargoya ₺{x} kaldı".
   **Neden:** Terkin bir numaralı nedeni sonradan çıkan maliyet.
   **Kanıt:** Ekstra maliyet %40, toplamı önceden görememe %12 (Baymard, 2025) — Güçlü kanıt.
3. **Kural:** Teslimat adımında en fazla 8 görünür alan olmalı: Ad Soyad (tek alan), E-posta, Telefon, İl, İlçe, Adres, Posta kodu (isteğe bağlı) ve gerekiyorsa bir alan daha. "Daire/kat/firma ekle" bir metin linkiyle açılmalı. Kupon alanı "İndirim kodun var mı?" linkinin arkasında durmalı.
   **Neden:** Kullanılabilirliği adım sayısından çok alan sayısı belirliyor.
   **Kanıt:** İdeal 7–8 alan, ortalama 11,3. Tek ad alanını %89, gizli "Adres 2"yi %75 site uygulamıyor (Baymard, 2024) — Güçlü kanıt.
4. **Kural:** "Fatura adresim teslimat adresiyle aynı" kutusu varsayılan olarak işaretli olmalı; kaldırılınca fatura alanları açılmalı.
   **Neden:** Gereksiz tekrar girişi önler.
   **Kanıt:** WCAG 2.2 3.3.7 Redundant Entry (A); fatura alanlarını gizlemeyen site %24 (Baymard, 2024) — Güçlü kanıt.
5. **Kural:** Teslimat süresi tarih aralığı olarak yazılmalı: "Tahmini teslimat: 8–10 Ekim". Gerçek kargo verisi geldiğinde kesim saati gösterilmeli: "14:00'e kadar verilen siparişler bugün kargoda". Önizlemede gerçek olmayan tarih gösterilmemeli.
   **Neden:** Hız yerine somut tarih belirsizliği kaldırır; yavaş teslimat terk nedenlerinin %20'si.
   **Kanıt:** %48 site hız yazıyor, %83 kesim saati göstermiyor (Baymard, 2025) — Güçlü kanıt.
6. **Kural:** Telefon alanının altında 13px #5C615A renkte açıklama olmalı: "Kargo firması teslimat için arayabilir." Zorunlu alanlar "*", isteğe bağlı alanlar "(isteğe bağlı)" ile işaretlenmeli.
   **Neden:** Kullanıcılar telefon vermekte isteksiz ve alanın zorunlu olup olmadığını tahmin etmek zorunda kalıyor.
   **Kanıt:** Kullanıcıların %70'ten fazlası telefon vermekte isteksiz; %49 site gerekçe yazmıyor; %61 site alanları işaretlemiyor (Baymard, 2025) — Güçlü kanıt.
7. **Kural:** Hatalar alan çıkışında (blur) satır içinde ve duruma özel gösterilmeli: "Posta kodu 5 haneli olmalı (ör. 34710)". Hata mesajı alanın altında 13px #741E32 metin ve ikon ile verilmeli, `aria-describedby` ile alana bağlanmalı. Yalnızca kırmızı kenarlık yeterli değil.
   **Neden:** Genel hata mesajı hangi alanın neden reddedildiğini söylemiyor.
   **Kanıt:** %94 site uyarlanabilir hata mesajı kullanmıyor (Baymard, 2025); WCAG 3.3.1/3.3.3 — Güçlü kanıt.
8. **Kural:** Kart alanları 1px #7A7F77 kenarlıklı, #F3F4F1 zeminli ve 16px iç boşluklu tek bir kutuda toplanmalı. Kutunun başlığında kilit ikonu ve "Ödeme bilgilerin şifrelenir" yazmalı. Kutunun altında kabul edilen kart ve taksit logoları yer almalı.
   **Neden:** Güven algısı görsel kapsüllemeyle artıyor.
   **Kanıt:** %19 kart güvensizliğinden terk ediyor (Baymard, 2025). Ev yapımı mühür bile çoğu SSL mühründen iyi sonuç verdi (Baymard, 2023 testi) — Orta.
9. **Kural:** Adet seçici 44×44px "−" ve "+" butonlarından ve ortadaki sayıdan oluşmalı. Şifre kuralı yalnızca "en az 8 karakter" olmalı ve canlı bir gösterge eklenmeli. Şifre alanında yapıştırmaya ve şifre yöneticisine izin verilmeli (`autocomplete="new-password"`).
   **Neden:** Karmaşık şifre kuralları ve küçük adet kontrolleri sürtünme yaratıyor.
   **Kanıt:** %97 site adet seçicide, %65 site şifre kuralında başarısız (Baymard, 2025); WCAG 3.3.8 — Güçlü kanıt.

### Navigasyon ve ana sayfa ([[Header ve Navigasyon]])

10. **Kural:** Masaüstü header sırası: Logo (Archivo Black) | Erkek | Kadın | Çocuk | Markalar | Yeni Gelenler | İndirim | arama alanı (en az 320px genişlik) | Favoriler | Sepet (adet rozetli). Her üst öğe kendi PLP'sine giden bir link olmalı.
    **Neden:** Giyim ve ayakkabıda cinsiyet ve yaş birbirini dışlayan ürün boyutları; kategori başlıkları tıklanabilir olmalı.
    **Kanıt:** %33 site başlıkları tıklanabilir yapmıyor (Baymard, 2025); NN/g hedef kitle navigasyonunda birbirini dışlayan kategorileri kabul ediyor (2015) — Güçlü kanıt / Orta.
11. **Kural:** Mega menü imleç 300–500ms (öneri: 400ms) hareketsiz kalınca açılmalı, imleç çıkınca 400ms sonra kapanmalı. Çapraz hareket menüyü kapatmamalı ve menü kaydırma gerektirmemeli. Sütunlar: "Ayakkabı", "Giyim ve Aksesuar", "Markalar" (7 marka) ve "Öne çıkan" (1 görsel kart). Her sütunun en üstünde "Tüm Erkek Ayakkabıları" linki olmalı.
    **Neden:** Gecikme olmazsa menü yanlışlıkla açılıyor. Kategorileri gruplara bölmek taramayı kolaylaştırıyor.
    **Kanıt:** NN/g 0,5 sn öneriyor (2017); %61 site hover gecikmesi, %60 site gruplama uygulamıyor (Baymard, 2025) — Güçlü kanıt.
12. **Kural:** Bulunulan üst kategori header'da 2px #741E32 alt çizgiyle vurgulanmalı. PLP'de breadcrumb olmalı: "Ana sayfa / Erkek / Sneaker".
    **Neden:** Kullanıcı hangi kapsamda olduğunu görmeli.
    **Kanıt:** %95 site (mobilde %94) mevcut kapsamı vurgulamıyor (Baymard, 2025–2026) — Güçlü kanıt.
13. **Kural:** Ara kategori sayfaları ("Erkek") alt kategorileri birincil içerik olarak sunmalı: 4:5 oranlı fotoğraflı karolar (Sneaker, Koşu, Terlik, Mont) ve her karoda 16px/600 etiket. Promosyon banner'ı en fazla bir tane olmalı ve karoların altında yer almalı.
    **Neden:** Kullanıcı ara sayfada bir sonraki adımı arıyor.
    **Kanıt:** %76 site alt kategorileri ana içerik yapmıyor, %55 site alt kategori görselini eksik ya da belirsiz bırakıyor (Baymard, 2025) — Güçlü kanıt.
14. **Kural:** Ana sayfada en fazla bir promosyon alanı olmalı. Görsel kartlardaki ürünler PDP'ye linklenmeli ("Ürünü gör →"). "Numaranla başla" beden ızgarası korunmalı ve her beden, beden filtresi uygulanmış PLP'ye gitmeli (`/erkek-sneaker?beden=42`).
    **Neden:** Agresif reklam yerleşimi ve linksiz ilham görselleri çıkmaz yaratıyor.
    **Kanıt:** %55 site agresif reklam, %70 site linksiz ilham görseli kullanıyor (Baymard, 2025) — Güçlü kanıt.

### PLP ([[Kategori Sayfası ve Filtreler]])

15. **Kural:** Filtre kenar çubuğunun sırası: Beden (varsayılan açık, 5 sütunlu ızgara, 48×44px butonlar, 8px boşluk) → Cinsiyet → Marka → Fiyat → Renk → Kullanım → İndirim. Mobilde Beden filtresi çekmecenin en üstünde ve açık olmalı.
    **Neden:** Ayakkabı alışverişinde ilk eleme kriteri beden.
    **Kanıt:** Beden filtresi üstte ve açıkken %90 önce bedenle filtreledi; %39 bedensizliği PDP'de öğrendi (Baymard, 2024) — Orta.
16. **Kural:** Tüm filtreler çoklu seçimli checkbox olmalı; renkte swatch, bedende buton kullanılmalı. Tek seçimli açılır liste kaldırılmalı. Seçim yapınca liste yeniden yüklenmeli (masaüstünde anında, mobilde "128 ürünü göster" butonuyla).
    **Neden:** Kullanıcı "42 veya 42,5" ya da "Nike veya adidas" gibi birleşimler istiyor.
    **Kanıt:** Çoklu seçimi kısıtlayan site %14 (Baymard, 2025); KPT'de şu anda tek seçimli açılır menü var — Güçlü kanıt.
17. **Kural:** Ham tedarikçi renk adları 12 ana renk ailesine eşlenmeli: Siyah, Beyaz, Gri, Lacivert, Mavi, Yeşil, Kırmızı, Bordo, Kahverengi, Bej, Pembe, Çok renkli. Her aile 24px dairesel swatch ve etiketle gösterilmeli. Tedarikçi renk adı yalnızca PDP'de "Renk: Lacivert/Beyaz-Gri" olarak kalmalı.
    **Neden:** Yüzlerce benzersiz değer renk filtresini kullanılmaz hale getiriyor.
    **Kanıt:** Mobilde %73 site eksik renk swatch'ı gösteriyor (Baymard, 2026); 5 temel filtre eksikliği %51 (Baymard, 2025) — Güçlü kanıt.
18. **Kural:** Her filtre seçeneğinin yanında sonuç sayısı olmalı ("42 (37)"). Sonuç vermeyecek seçenekler soluk ve devre dışı gösterilmeli. Başlığın altında toplam görünmeli: "Erkek Sneaker · 128 ürün".
    **Neden:** Kullanıcı seçmeden önce kaç ürün kalacağını görmeli.
    **Kanıt:** Baymard PLP rehberi, 2026 — Güçlü kanıt.
19. **Kural:** Uygulanan filtreler ızgaranın üstünde çip olarak gösterilmeli. Çip: 36px yükseklik, 18px radius, #E5E8E3 zemin, 14px #171B1C metin, sağda en az 24×24px "×" hedefi. Çiplerin sonunda "Tümünü temizle" metin linki olmalı. Mobilde çipler sticky filtre çubuğunun altında yatay kaydırılabilir olmalı.
    **Neden:** Kullanıcı neyin filtrelendiğini ve nasıl geri alacağını görmeli.
    **Kanıt:** Uygulanan filtre özeti eksikliği %20–28, mobilde %66 (Baymard, 2025–2026) — Güçlü kanıt.
20. **Kural:** Sıralama seçenekleri: Önerilen (varsayılan), En çok satanlar, En yeniler, Fiyat: Düşükten yükseğe, Fiyat: Yüksekten düşüğe. Yorum verisi olunca "En yüksek puan" eklenmeli.
    **Neden:** Bunlar temel sıralama türleri.
    **Kanıt:** %69 site 4 temel sıralamanın hepsini sunmuyor (Baymard, 2025) — Güçlü kanıt.
21. **Kural:** Masaüstünde 4 sütunda 24 ürün yüklenmeli, ardından 24 ürün daha tembel yüklenmeli. 48. üründen sonra "Daha fazla göster" butonu çıkmalı (240px genişlik, 48px yükseklik, #171B1C çerçeve). Butonun üstünde "321 üründen 48'i gösteriliyor" metni ve 4px ilerleme çubuğu olmalı. Mobilde 2 sütunda 24 üründen sonra buton gelmeli. Sonsuz kaydırma kullanılmamalı. PDP'den dönüşte `history.scrollRestoration` ve yüklü ürün sayısı korunmalı.
    **Neden:** "Daha fazla yükle" gezinme miktarı ile footer erişimi arasında en iyi denge.
    **Kanıt:** Baymard 2026'da "Daha fazla yükle"yi öneriyor; 2016 testinde masaüstünde 50–100, mobilde 15–30 ürün önerisi; %90'dan fazla site geri dönüş konumunu koruyamıyor — Orta/Güçlü kanıt.
22. **Kural:** Ürün kartı: 1:1 görsel (#F3F4F1 zemin), hover'da ikinci görsel (yan veya ayakta). Altında 13px büyük harf marka, 15px/500 model adı ve 15px/700 fiyat yer almalı. İndirimde eski fiyat solda üstü çizili #5C615A, yeni fiyat #741E32 olmalı. Altta "4 renk" metni ya da en fazla 4 mini swatch bulunmalı. Renk varyasyonları tek kartta birleştirilmeli.
    **Neden:** Birleştirilmemiş varyasyonlar listeyi şişiriyor ve karşılaştırmayı zorlaştırıyor.
    **Kanıt:** %42 site varyasyonları birleştirmiyor, %80 site 3'ten fazla görsel sunmuyor (Baymard, 2025); Baymard #421 "Essential" — Güçlü kanıt.
23. **Kural:** Kartta en fazla bir rozet olmalı (sol üst, 24px yükseklik, 12px/700 büyük harf): "YENİ", "İNDİRİM %20", "ÇOK SATAN" ya da "SON 2 ÇİFT". Listedeki ürünlerin en fazla %25'inde rozet olmalı (öneri).
    **Neden:** Her üründe rozet varsa hiçbiri fark edilmiyor.
    **Kanıt:** Baymard, Eylül 2026 (oran belirtilmemiş) — Orta.
24. **Kural:** Mobil PLP'de başlığın altında sticky bir çubuk olmalı (48px yükseklik, #F3F4F1 zemin): sol yarıda "Filtrele (3)", sağ yarıda "Sırala: Önerilen". Filtre, ekranın %90'ını kaplayan alttan açılır çekmecede açılmalı. Çekmecede en altta sabit "128 ürünü göster" (#741E32, 48px) ve "Temizle" butonları bulunmalı.
    **Neden:** Mobilde filtre her an erişilebilir olmalı.
    **Kanıt:** Mobil PLP'lerin %78'i zayıf–vasat; sticky filtre deseni öneriliyor (Baymard, 2025–2026) — Güçlü kanıt.

### PDP ([[Ürün Sayfası]], [[Beden ve Kalıp]])

25. **Kural:** Beden seçici buton ızgarası olmalı: 48×44px butonlar, 8px boşluk, masaüstünde 6, mobilde 4–5 sütun. Varsayılan buton 1px #7A7F77 kenarlık ve #171B1C metin kullanmalı; seçili buton #171B1C zemin ve #FFFFFF metin. EU bedeni ana etiket olmalı. Seçicinin üstünde "Beden (EU)" ve sağda "Beden rehberi" linki yer almalı.
    **Neden:** Butonlar, açılır listenin gizlediği stok durumunu ve seçenekleri görünür kılıyor.
    **Kanıt:** Beden butonu kullanmayan site %57–70 (Baymard, 2025–2026); 1.4.11 kenarlık kontrastı 3,71:1 (hesap) — Güçlü kanıt.
26. **Kural:** Stokta olmayan bedenler **gösterilmeli**: #F3F4F1 zemin, #6B7069 metin, butonu çapraz kesen 1px #7A7F77 çizgi ve `aria-label="42 – stokta yok"`. Tıklanınca çekmece açılmalı: "Bu beden şu an yok. Gelince haber verelim mi?" ve altında aynı modelin diğer renklerinde 42 numara stoğu. Yalnızca stoktaki bedenleri göstermek yasak.
    **Neden:** Gizlenen beden "bu model bende yok" ile "tükendi"yi ayırt ettirmiyor ve alternatif yolu kapatıyor.
    **Kanıt:** Stoksuzlukta %30 başka siteye gidiyor, %68 site sipariş aldırmıyor (Baymard, 2025); ayrıntılı gösterim Baymard #850 Premium'da `(tahmin: stil)` — Orta.
27. **Kural:** Beden rehberi çekmecesi şunları içermeli: EU / US / UK / cm tablosu (marka bazında: Nike, adidas, New Balance, Skechers, Puma, Vans, Columbia), "Ayağını ölç" 3 adımlı talimatı ve SVG çizimi, kalıp notu ("Bu model dar kalıptır; geniş ayaklar için yarım numara büyük önerilir" — yalnızca doğrulanmış veriyle) ve müşteri hizmetleri linki.
    **Neden:** Ayakkabıda iadenin ana nedeni beden; markalar arasında kalıp farklı.
    **Kanıt:** %82 giyim sitesi yetersiz beden bilgisi sunuyor; 10 bileşenli beden bilgisi önerisi (Baymard, 2025) — Güçlü kanıt.
28. **Kural:** Her üründe en az 7 görsel olmalı, sabit sırayla: (1) dış yan profil, (2) ön 3/4, (3) iç yan, (4) üstten, (5) taban, (6) topuk/arka, (7) **ayakta (on-foot) ölçek görseli**; isteğe bağlı (8) malzeme detayı. Format 1:1, zemin #F3F4F1, kaynak en az 2000px, zoom açık olmalı. Mobilde yatay kaydırmalı galeri ve "1/8" sayacı kullanılmalı.
    **Neden:** Kullanıcıların çoğu PDP'ye görsellerle başlıyor ve boyutu görselden kestirmeye çalışıyor.
    **Kanıt:** İlk eylem görsel %56; boyutu görselden anlamaya çalışan %42; ölçek görseli eksik %37; insan model görseli eksik %23; çözünürlük veya zoom yetersiz %25 (Baymard, 2017–2026) — Güçlü/Orta.
29. **Kural:** Açıklama tek dikey akışta olmalı; sekme kullanılmamalı. Sıra: "Öne çıkanlar" (3–5 madde) → "Özellikler" tablosu (Üst malzeme, İç astar, Taban, Ağırlık (g, 42 numara), Topuk-burun farkı (mm), Kalıp, Ürün kodu) → "Bakım" → "Teslimat ve İade". Masaüstünde bölümler açık olmalı, mobilde 56px başlıklı akordeon kullanılmalı (ilki açık). Tablo tek sütunlu olmalı: etiket solda #5C615A, değer sağda #171B1C, satırlar dönüşümlü #F3F4F1 zeminli.
    **Neden:** Sekmelerdeki içerik gözden kaçıyor; tutarsız özellik tablosu karşılaştırmayı bozuyor.
    **Kanıt:** Ana bölümlerde yatay sekme kullanan site %29; özellik tablosu zayıf–vasat %64, ciddi tutarsızlık %30 (Baymard, 2026) — Güçlü kanıt.
30. **Kural:** Fiyat bedene göre değişiyorsa PLP kartında "₺3.499'dan başlayan" yazmalı. PDP'de beden seçilmeden "₺3.499 – ₺3.899" ve altında 13px "Fiyat bedene göre değişir" gösterilmeli. Beden seçilince fiyat anında güncellenmeli ve değişiklik `aria-live="polite"` ile duyurulmalı. Farklı fiyatlı bedenlerin butonunda 11px "+₺200" etiketi olmalı.
    **Neden:** Gizli fiyat farkı sepette sürpriz maliyet yaratır.
    **Kanıt:** Sürpriz maliyet terk nedenlerinin başında (%40) ve toplam maliyeti gösteremeyen PDP %67 (Baymard, 2025–2026); gösterim deseni `(tahmin)` — Orta.
31. **Kural:** "Sepete ekle" butonunun hemen altında 3 satırlık güven bloğu olmalı (14px, 20px ikonlar): "Tahmini teslimat: {tarih aralığı}", "{n} gün içinde ücretsiz iade" (linkli), "{banka} kartlarına {n} taksit". Değerler gerçek politikadan gelmeli; önizlemede uydurma değer yazılmamalı.
    **Neden:** Teslimat, iade ve maliyet belirsizliği terk nedenlerinin önemli kısmı.
    **Kanıt:** İade politikasını belirgin göstermeyen PDP %44; terk nedenleri: iade %13, yavaş teslimat %20 (Baymard, 2025–2026) — Güçlü kanıt. Ayrıntı: [[Güven Sinyalleri]].
32. **Kural:** Mobilde ana CTA ekrandan çıkınca alttan sticky çubuk çıkmalı: 64px + `env(safe-area-inset-bottom)` yükseklik, #FFFFFF zemin, üstte 1px #E5E8E3 çizgi. Solda seçili beden ("EU 42" ya da "Beden seç") ve fiyat, sağda 48px yükseklikte ve en az 160px genişlikte #741E32 "Sepete ekle" butonu. Beden seçilmemişse buton beden çekmecesini açmalı. Uygulama A/B testiyle doğrulanmalı.
    **Neden:** Uzun mobil PDP'de CTA erişilebilirliği; ancak kanıt karışık.
    **Kanıt:** Bir test dönüşümde +%6,2, bir başkası −%7,7 (sonuçsuz) gösterdi (Clean Commit, 2025) — Zayıf.
33. **Kural:** Sticky header ve sticky ATC olan sayfalarda `scroll-padding-top` header yüksekliğine (ör. 64px), `scroll-padding-bottom` ise 80px'e eşitlenmeli. Klavye odağı hiçbir zaman bu çubukların altında kaybolmamalı.
    **Neden:** Klavye kullanıcısı odaklanan öğeyi görebilmeli.
    **Kanıt:** WCAG 2.2 2.4.11 Focus Not Obscured (AA) — Güçlü kanıt.
34. **Kural:** Kalıcı olarak satıştan kalkan ürün sayfası silinmemeli. Başlığın üstünde "Bu ürün artık satılmıyor" bandı olmalı; satın alma alanının yerine "Benzer modeller" (aynı marka ve kullanım, 4 ürün) gelmeli. Geçici stoksuzlukta gerçek bir tedarik tarihi varsa ön sipariş alınmalı.
    **Neden:** Çıkmaz sokak kullanıcıyı rakibe gönderiyor.
    **Kanıt:** %30 terk; %68 site sipariş aldırmıyor (Baymard, 2025) — Orta.
35. **Kural:** Yorum modülü (veri geldiğinde): ortalama puan, puan dağılım çubukları, "Kalıp: Küçük – Tam – Büyük" alt puan çubuğu, yorumcu fotoğrafları arasında yorumlar arası gezinme, "Doğrulanmış alıcı" rozeti ve olumsuz yorumlara marka yanıtı. İlk hedef her çok satan model için en az 5 yorum.
    **Neden:** Yorumların etkisi ilk 5 yorumda en yüksek; kalıp alt puanı beden kararını hızlandırıyor.
    **Kanıt:** 5 yorumla satın alma olasılığı +%270, ideal puan 4,0–4,7, doğrulanmış alıcı +%15 (Spiegel, 2017) — Orta. Kalıp puanı eksik %24; yorum görseli gezinmesi eksik %90; olumsuz yoruma yanıt vermeyen %89 (Baymard, 2025–2026) — Güçlü kanıt.

### Arama ([[Arama]])

36. **Kural:** Otomatik tamamlama ilk karakterden sonra 150ms debounce ile açılmalı. Mobilde en fazla 6, masaüstünde en fazla 8 sorgu önerisi ve yanında 3 ürün kartı gösterilmeli; kaydırma çubuğu olmamalı. Tamamlanan kısım kalın yazılmalı. Kapsam önerisi italik #5C615A ile gösterilmeli ("sneaker — *Erkek* içinde"). Ok tuşu ve Enter desteklenmeli; aktif satır #E5E8E3 zeminle vurgulanmalı. Mobilde her satır en az 48px olmalı ve satırlar 1px ayırıcıyla ayrılmalı.
    **Neden:** Uzun liste seçim felci yaratıyor; mobilde klavye ile öneri listesi arasında alan dar.
    **Kanıt:** Masaüstünde ≤10, mobilde 4–8 öneri; yalnızca %19 site tam uyguluyor (Baymard, 2022) — Orta.
37. **Kural:** Arama indeksi Türkçe karakterleri katlamalı (ı→i, İ→i, ş→s, ğ→g, ü→u, ö→o, ç→c). Küçük harfe çevirmede yerel ayara dikkat edilmeli (`toLocaleLowerCase('tr')` ile katlama tutarlı olmalı). Yazım hatası toleransı (Levenshtein ≤1–2) ve eş anlamlı sözlüğü olmalı: "naik/nıke→nike", "addidas/adıdas→adidas", "nb/new balans→new balance", "sketchers→skechers", "spor ayakkabı→sneaker", "kar botu→bot", "42 numara→beden filtresi 42".
    **Neden:** Hatalı ya da Türkçe karakterli sorgular sıfır sonuca düşüyor.
    **Kanıt:** Yazım hatasında öneri sunmayan %69 (2021), mobilde %28 (2026); kısaltma ve sembol aramalarında %54 başarısızlık (Baymard, 2026) — Güçlü/Orta.
38. **Kural:** Sonuç yok sayfası: "'{sorgu}' için sonuç bulamadık" başlığı, "Bunu mu demek istediniz: {düzeltme}" (ürün önizlemeli), 6 popüler kategori karosu, "Çok satanlar" 4'lü ızgara, son görüntülenen ürünler ve "Yardım: WhatsApp / telefon" bağlantısı. "Arama ipuçları" listesi tek başına kullanılmamalı.
    **Neden:** Sonuçsuz arama terkin bir numaralı tetikleyicisi.
    **Kanıt:** Yaklaşık %50 site etkili çıkış yolu sunmuyor (Baymard, 2025) — Güçlü kanıt.
39. **Kural:** Mobilde arama header'da ikon değil, görünür bir alan olmalı (tam genişlik, 44px yükseklik, placeholder "Marka, model veya numara ara"). Klavyede "Ara" tuşu (`enterkeyhint="search"`) ve görünür gönder butonu bulunmalı. Arama sonuçlarında sonsuz kaydırma olmamalı.
    **Neden:** Kullanıcıların yaklaşık yarısı ürünü aramayla buluyor.
    **Kanıt:** Aramayı tercih eden ~%50; mobilde gönder butonu olmayan %27 (Baymard, 2026) — Güçlü kanıt.

### Mobil ([[Mobil Deneyim]])

40. **Kural:** Tüm dokunma hedefleri en az 44×44px olmalı, hedefler arasında en az 8px boşluk bırakılmalı. Swatch, çip "×" ve sayfa noktası gibi küçük öğelerde görsel boyut küçük kalabilir ama tıklama alanı en az 24×24px'e (WCAG AA alt sınırı) genişletilmeli.
    **Neden:** Küçük ve sık hedefler yanlış dokunmaya yol açıyor.
    **Kanıt:** WCAG 2.5.8 (AA) 24px; 2.5.5 (AAA) 44px; Android 48dp ve 8dp; NN/g 1 cm — Güçlü kanıt.
41. **Kural:** Mobilde 5 öğeli alt sekme çubuğu olmalı (56px + safe area, #FFFFFF zemin, 24px ikonlar, 11px etiketler): Ana sayfa, Kategoriler, Ara, Favoriler, Sepet (rozetli). Aktif sekmenin ikonu ve etiketi #741E32 olmalı. PDP'de sticky ATC görünürken çubuk gizlenmeli.
    **Neden:** Görünür navigasyon gizli menüden daha çok kullanılıyor.
    **Kanıt:** Gizli menü %57, kombine menü %86 kullanım; keşifte %20'den fazla düşüş (NN/g, 2016); tab bar ≤5 öğe (NN/g, 2015) — Orta.
42. **Kural:** Birincil eylemler (Sepete ekle, Filtrele, Ödemeye geç, "128 ürünü göster") ekranın alt üçte birinde ve tam ya da yarım genişlikte olmalı. Kapatma (×) ve geri butonları en az 44px olmalı; üst köşedeki kritik eylemler için alt bölgede bir alternatif sunulmalı.
    **Neden:** Tek elle kullanımda ekranın üst köşelerine ulaşmak zor.
    **Kanıt:** Kullanıcıların %49'u telefonu tek elle, bunların %67'si sağ başparmakla kullanıyor (Hoober, 2013) — Orta.

### Performans

43. **Kural:** Mobilde p75 hedefleri: LCP ≤2,0 sn (Google eşiği 2,5), INP ≤200ms, CLS ≤0,05 (eşik 0,1). Her deploy'da Lighthouse CI ve `web-vitals` ile saha verisi toplanmalı.
    **Neden:** Hız ile dönüşüm arasındaki ilişki birden çok çalışmada tekrarlanıyor.
    **Kanıt:** 0,1 sn hızlanmada perakende dönüşüm +%8,4 (Deloitte, 2020); Rakuten 24 dönüşüm +%33 (2022); mobil originlerin yalnız %48'i CWV'yi geçiyor (Almanac, 2025) — Orta/Güçlü kanıt.
44. **Kural:** Hero görseli PNG'den AVIF'e (WebP yedekli) çevrilmeli: `<picture>` ve `srcset` ile 640/960/1280/1920 genişlikler sunulmalı. Hedef ağırlık mobilde ≤120 KB, masaüstünde ≤200 KB (öneri). `fetchpriority="high"` eklenmeli, `loading="lazy"` kullanılmamalı, `width`/`height` verilmeli. Hero dışındaki görseller `loading="lazy"` ve `decoding="async"` almalı.
    **Neden:** 900 KB'lık PNG büyük olasılıkla LCP öğesi; görsel, mobilde LCP öğesinin %76'sı.
    **Kanıt:** Sayfaların ~%16–17'si LCP görselini tembel yüklüyor; PNG %26, WebP %11 (Almanac, 2025); web.dev LCP rehberi — Güçlü kanıt.
45. **Kural:** Tüm ürün görseli kapsayıcılarında `aspect-ratio: 1/1`, hero'da sabit oran olmalı. Duyuru bandı, çerez bandı ve rozetler için yer önceden ayrılmalı veya bunlar overlay olarak yerleştirilmeli. Web fontlarında (Manrope, Cormorant Garamond, Archivo Black) `font-display: swap` ve boyut uyumlu yedek font (`size-adjust`) kullanılmalı.
    **Neden:** Düzen kaymaları yanlış tıklamaya ve güven kaybına yol açıyor.
    **Kanıt:** Rakuten 24 CLS'yi %92,7 iyileştirdi, dönüşüm +%33 (web.dev, 2022) — Orta.
46. **Kural:** Filtre değişimi, beden seçimi ve galeri kaydırma gibi işleyiciler 50ms'den uzun görev üretmemeli. Önce görsel geri bildirim verilmeli (buton durumu), ağır iş `scheduler.yield()` (yoksa `setTimeout(0)`) ile sonraya bırakılmalı. Kaydırma ve tembel yükleme işleyicilerine debounce uygulanmalı. PLP tembel yüklemesi 24'lük gruplarla yapılmalı.
    **Neden:** INP etkileşim hissini belirliyor; ağır PLP'ler en riskli sayfalar.
    **Kanıt:** Trendyol PLP'de INP −%50 ve PLP'den PDP'ye tıklama +%1 (2023); redBus INP −%72 ve satış +%7 (2023) — Orta.

### Erişilebilirlik ([[Renk ve Tipografi]])

47. **Kural:** Uyum hedefi WCAG 2.2 AA; son tarih 21 Haziran 2027. Kontrol listesi: kontrast, alt metin, form etiketleri, klavye, odak, hedef boyutu ve hareket. Her sürümde axe-core ile otomatik test ve en az bir klavye ve ekran okuyucu (NVDA veya VoiceOver) turu yapılmalı.
    **Neden:** Türkiye Genelgesi e-ticareti kapsıyor; alışveriş siteleri ortalamadan kötü durumda.
    **Kanıt:** Genelge 2025/10 (2 yıl, WCAG 2.2); alışverişte sayfa başına 71 hata (WebAIM, 2026) — Güçlü kanıt.
48. **Kural:** Renk token'ları: `--text #171B1C`, `--text-muted #5C615A` (en az 4,5:1), `--accent #741E32`, `--border-ui #7A7F77` (en az 3:1), `--bg #F3F4F1`, `--bg-alt #E5E8E3`. #8A8F87 ve daha açık griler metin veya kontrol kenarlığında kullanılmamalı. #6B7069 yalnızca #F3F4F1 veya beyaz zeminde ve devre dışı durumda kullanılmalı.
    **Neden:** Düşük kontrast en yaygın WCAG hatası.
    **Kanıt:** Ana sayfaların %83,9'unda düşük kontrast (WebAIM, 2026); oranlar bu notta WCAG formülüyle hesaplandı — Güçlü kanıt.
49. **Kural:** Odak göstergesi tüm etkileşimli öğelerde `outline: 2px solid #741E32; outline-offset: 2px` olmalı; `outline: none` yasak. Koyu zeminde beyaz halka kullanılmalı.
    **Neden:** Klavye kullanıcısı nerede olduğunu görmeli.
    **Kanıt:** WCAG 2.4.7 (AA), 2.4.13 (AAA) 2px ve 3:1; bordo/#F3F4F1 9,63:1 — Güçlü kanıt.
50. **Kural:** Ürün görsellerinde alt metin şablonu: "{Marka} {Model} {Renk} – {açı}" (ör. "New Balance 530 Beyaz/Gümüş – dış yan görünüm"). Dekoratif görseller `alt=""` almalı. İkon butonlarda `aria-label` olmalı ("Sepete git, 2 ürün"). Sayfada `<html lang="tr">` tanımlı olmalı.
    **Neden:** Eksik alt metin, boş link ve boş buton en yaygın hatalar arasında.
    **Kanıt:** Eksik alt metin %53,1, boş link %46,3, boş buton %30,6, dil eksik %13,5 (WebAIM, 2026) — Güçlü kanıt.
51. **Kural:** Her form alanında görünür `<label>` olmalı; placeholder etiket yerine kullanılmamalı. Alanlar uygun `autocomplete` değerlerini almalı (`name`, `email`, `tel`, `address-line1`, `postal-code`, `cc-number`, `one-time-code`). Hatalar `aria-invalid` ve `aria-describedby` ile duyurulmalı.
    **Neden:** Etiketsiz alan ekran okuyucuda anlamsız; autocomplete yeniden yazmayı ortadan kaldırıyor.
    **Kanıt:** Etiketsiz girdi %51 (WebAIM, 2026); WCAG 1.3.5, 3.3.7, 3.3.8 — Güçlü kanıt.
52. **Kural:** Fiyat filtresindeki çift tutamaçlı kaydırıcının yanında "En az ₺" ve "En çok ₺" sayı alanları olmalı. Galeri ve karusellerde ok butonları sürüklemeye alternatif sunmalı. 360° görüntüleyici varsa "←/→ döndür" butonları eklenmeli.
    **Neden:** Sürükleme hareketi yapamayan kullanıcılar bu işlevlere erişemiyor.
    **Kanıt:** WCAG 2.2 2.5.7 Dragging Movements (AA) — Güçlü kanıt.
53. **Kural:** Yardım kanalları ("Yardım", "WhatsApp", "0 850 …", "İade ve değişim") header'daki yardım menüsünde ve footer'da her sayfada aynı sırayla bulunmalı.
    **Neden:** Kullanıcı yardımı her sayfada aynı yerde bulmalı.
    **Kanıt:** WCAG 2.2 3.2.6 Consistent Help (A) — Güçlü kanıt. Ayrıntı: [[Footer]].

### Karusel, hero, pop-up ve çerez ([[Hero ve Banner Desenleri]])

54. **Kural:** Hero tek ve statik olmalı: gerçek fotoğraf veya kusursuz render, tam genişlik (masaüstünde 16:7, mobilde 4:5), HTML metin başlık ve tek birincil CTA. Dönen ayakkabı animasyonu korunacaksa 5 sn içinde kendiliğinden durmalı ya da görünür bir "Duraklat" butonu (44×44px) olmalı. `prefers-reduced-motion: reduce` durumunda animasyon tamamen kapatılmalı.
    **Neden:** Otomatik hareket hem kullanılabilirlik hem erişilebilirlik sorunu.
    **Kanıt:** WCAG 2.2.2 (A); NN/g 2013; Baymard'a göre karuseli olan sitelerin %46'sında sorun var (2025) — Güçlü kanıt.
55. **Kural:** Karusel kaçınılmazsa (ör. "Yeni gelenler" ürün şeridi): mobilde otomatik dönme olmamalı, kaydırma ve 44px oklar bulunmalı. Masaüstünde 6 sn'de bir dönmeli, hover'da durmalı ve ilk kullanıcı etkileşiminden sonra kalıcı olarak durmalı. Bir slayt kısmen görünür bırakılmalı (peek, ~%15).
    **Neden:** Kullanıcı kontrolü ve okuma süresi gerekiyor.
    **Kanıt:** Baymard 5–7 sn, mobilde otomatik dönme yok (2025) — Güçlü kanıt.
56. **Kural:** Sayfa açılışında modal pop-up olmamalı. E-bülten veya ilk sipariş teklifi footer'da satır içi blok olarak sunulmalı. Gerekirse ikinci sayfa görüntülemesinden sonra sağ altta 320×120px'lik kapatılabilir bir kart kullanılabilir; mobilde ekran yüksekliğinin %15'ini aşmayan alt bant (öneri). Kapatılan teklif 30 gün tekrar gösterilmemeli.
    **Neden:** Modal en nefret edilen teknik; arama görünürlüğüne de zarar veriyor.
    **Kanıt:** NN/g (2017) en nefret edilen teknikler arasında modal; Google içeriği engelleyen promosyon geçiş ekranlarını önermiyor — Orta/Güçlü kanıt.
57. **Kural:** Çerez bandı alt kenarda (masaüstünde en fazla 120px yükseklik) olmalı. Aynı boyut ve stilde üç buton sunulmalı: "Tümünü kabul et", "Yalnızca zorunlu", "Tercihler". Kabul butonu daha belirgin yapılmamalı. Bant, ATC çubuğu ve sohbet balonuyla üst üste binmemeli; çerez bandı varken diğer katmanlar gösterilmemeli.
    **Neden:** Eşit seçenek güven veriyor; üst üste binen katmanlar içeriği kapatıyor.
    **Kanıt:** NN/g çerez izinleri araştırması (2023) — Orta. KVKK gereklilikleri bu notta doğrulanmadı.

### Ürün fotoğrafçılığı ve AI görselleri ([[Görsel Tasarım ve Trendler 2026]])

58. **Kural:** PDP ve PLP'de ürünü temsil eden görseller gerçek fotoğraf ya da gerçek ürün verisinden üretilmiş doğru render olmalı. AI ile üretilmiş görsel yalnızca atmosfer ve hero amaçlı kullanılmalı. Bu durumda çift kontur, bozuk logo ve anatomik hata kontrolünden geçmeli; gerçeklik izlenimi veriyorsa "Görsel yapay zekâ ile oluşturulmuştur" ibaresi ve görüntü meta verisi eklenmeli.
    **Neden:** AI şüphesi algıyı düşürüyor; temsil hatası beklentiyi bozuyor.
    **Kanıt:** NN/g 2026: kaynak bilinmediğinde fark yok, şüphe edildiğinde puan düşüyor (77 kişi, ürün görseli değil); AB Yapay Zekâ Yasası Madde 50 (2 Ağustos 2026); Baymard: bilgisayar üretimi görseller gerçek fotoğrafı tamamlamalı (2017) — Orta.
59. **Kural:** Tüm katalogda görsel tutarlılığı sağlanmalı: aynı açı sırası (Kural 28), aynı zemin #F3F4F1, ürün kadrajın %80'ini doldurmalı, burun sola bakmalı ve gölge yumuşak olmalı. Bu standarda uymayan tedarikçi görselleri otomatik kırpma ve zemin normalizasyonundan geçirilmeli.
    **Neden:** Tutarsız görseller ızgarada karşılaştırmayı zorlaştırıyor ve kalite algısını düşürüyor.
    **Kanıt:** Liste görsellerinin ürünü doğru yansıtması gerekiyor (Baymard PLP, 2026); karşılaştırma ilkesi `(tahmin: ölçüler)` — Orta.
60. **Kural:** Video, 360° ve AR ancak Kural 28'deki statik set tamamlandıktan sonra eklenmeli; önce en çok satan 20 modelde 6–10 sn'lik sessiz, döngülü ve otomatik oynatılmayan (dokununca oynayan) ayakta videosu ile başlanmalı (öneri). Etki, iade oranı ve dönüşüm üzerinden A/B testiyle ölçülmeli.
    **Neden:** Bağımsız ve güncel kanıt zayıf, maliyet yüksek.
    **Kanıt:** 3D/AR için yalnızca satıcı vakaları var (Shopify 2026, Rebecca Minkoff: AR görüntüleyenlerde satın alma +%65) — Zayıf.

---

## Kaynaklar

**Baymard Institute**
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
- https://baymard.com/research/ecommerce-search
- https://baymard.com/blog/mobile-ux-ecommerce
- https://baymard.com/blog/homepage-carousel
- https://www.smashingmagazine.com/2016/03/pagination-infinite-scrolling-load-more-buttons/ (Baymard araştırması, Smashing Magazine'de yayımlandı)

**Nielsen Norman Group**
- https://www.nngroup.com/articles/mega-menus-work-well/
- https://www.nngroup.com/articles/audience-based-navigation/
- https://www.nngroup.com/articles/hamburger-menus/
- https://www.nngroup.com/articles/mobile-navigation-patterns/
- https://www.nngroup.com/articles/touch-target-size/
- https://www.nngroup.com/articles/auto-forwarding/
- https://www.nngroup.com/articles/most-hated-advertising-techniques/
- https://www.nngroup.com/articles/cookie-permissions/
- https://www.nngroup.com/articles/ai-generated-images/

**Performans**
- https://web.dev/articles/vitals
- https://web.dev/articles/optimize-lcp
- https://almanac.httparchive.org/en/2025/performance
- https://web.dev/case-studies/rakuten
- https://web.dev/case-studies/vodafone
- https://web.dev/case-studies/trendyol-inp
- https://web.dev/case-studies/redbus-inp
- https://web.dev/case-studies/economic-times-inp
- https://web.dev/case-studies/milliseconds-make-millions
- https://www.deloitte.com/ie/en/services/consulting/research/milliseconds-make-millions.html
- https://www.akamai.com/fr/newsroom/press-release/akamai-releases-spring-2017-state-of-online-retail-performance-report
- https://www.portent.com/blog/analytics/research-site-speed-hurting-everyone.htm

**Davranış ve mobil**
- https://contentsquare.com/guides/digital-experience-benchmark/traffic/
- https://contentsquare.com/guides/digital-experience-benchmark/conversions/
- https://contentsquare.com/guides/digital-experience-benchmark/engagement/
- https://www.statista.com/statistics/534123/mobile-share-of-retail-e-commerce-sales/ (içerik bu oturumda doğrudan okunmadı; rakam ikincil aktarım)
- https://www.uxmatters.com/mt/archives/2013/02/how-do-users-really-hold-mobile-devices.php
- https://support.google.com/accessibility/android/answer/7101858
- https://developer.apple.com/design/human-interface-guidelines/accessibility (sayfa metni bu oturumda okunamadı)
- https://spiegel.medill.northwestern.edu/how-online-reviews-influence-sales/
- https://cleancommit.io/ab-tests/sticky-mobile-add-to-cart-button/
- https://cleancommit.io/ab-tests/mobile-bottom-sticky-add-to-cart-button/
- https://www.shopify.com/blog/3d-ecommerce

**Erişilebilirlik ve mevzuat**
- https://www.w3.org/WAI/standards-guidelines/wcag/new-in-22/
- https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html
- https://www.w3.org/TR/WCAG22/
- https://webaim.org/projects/million/
- https://www.who.int/campaigns/international-day-of-persons-with-disabilities/2023
- https://abilitynet.org.uk/news-blogs/research-shows-businesses-lose-17-billion-ignoring-accessibility-needs
- https://www.clickawaypound.com/downloads/CAP2019PR2.pdf
- https://commission.europa.eu/strategy-and-policy/policies/justice-and-fundamental-rights/disability/union-equality-strategy-rights-persons-disabilities-2021-2030/european-accessibility-act_en
- https://eur-lex.europa.eu/eli/dir/2019/882/oj/eng (metin bu oturumda okunamadı)
- https://e-include.eu/web-accessibility/european-accessibility-act/ (ikincil)
- https://www.fudge.ai/blog/european-accessibility-act-shopify/ (ikincil)
- https://www.erdem-erdem.av.tr/bilgi-bankasi/web-siteleri-ve-mobil-uygulamalarin-erisilebilirligi-hakkinda-2025-10-sayili-cumhurbaskanligi-genelgesi-yayimlandi
- https://www.lexpera.com.tr/mevzuat/genelgeler/web-siteleri-ve-mobil-uygulamalarin-erisilebilirligi-ile-ilgili-2025-10-sayili-cumhurbaskanligi-1
- https://ikas.com/tr/blog/e-ticaret-siteleri-icin-yeni-zorunluluk-web-erisilebilirligi
- https://webrazzi.com/2025/06/30/web-siteleri-ve-uygulamalar-icin-erisilebilirlik-zorunlulugu-geliyor/
- https://artificialintelligenceact.eu/article/50/

**Pop-up ve geçiş ekranları**
- https://developers.google.com/search/docs/appearance/avoid-intrusive-interstitials
