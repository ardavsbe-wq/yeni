---
tür: araştırma
konu: Renk psikolojisi, kontrast ve tipografi (kanıt/mit ayrımı + KPT token önerisi)
güncellik: 2026-10-04
etiketler: [araştırma, renk, tipografi, kontrast, erişilebilirlik, tasarım-tokenları, türkçe-tipografi]
ilgili: ["[[Görsel Tasarım ve Trendler 2026]]", "[[Satın Alma Psikolojisi]]", "[[E-ticaret UX Verileri]]", "[[KPT Store Denetimi]]"]
---

# Renk ve Tipografi

> [!summary] En önemli 12 bulgu
> 1. "Kırmızı buton kazanır" bir mittir. Bilinen HubSpot/Performable testinde (2011, ~2.000 ziyaret) kırmızı, yeşil ağırlıklı bir sayfada tek kırmızı öğe olduğu için kazanmıştır. Bu bir **izolasyon/kontrast etkisidir**. **Güçlü (mit olduğu konusunda)**
> 2. "Yargının %62–90'ı renge dayanır" iddiası (Singh, 2006) bir derlemenin aralığıdır. Tek bir ölçüm değildir ve bağlamından koparılmıştır. **Zayıf**
> 3. Renk ile marka kişiliği arasındaki ilişki deneysel olarak gösterilmiştir: siyah, mor ve pembe → sofistike; kırmızı → heyecan; mavi → yetkinlik; kahverengi → sağlamlık; beyaz ve pembe → samimiyet. Satın alma niyeti, renk markanın iddia ettiği kişilikle uyumlu olduğunda en yüksektir (Labrecque & Milne, 2012). **Orta**
> 4. Renk–duygu eşleşmeleri 30 ülkede büyük ölçüde ortaktır (r = .88), ancak ülkeye özgü sapmalar da vardır (Jonauskaite vd., 2020). Bu yüzden "evrensel renk anlamı" tablolarına güvenilmez. **Güçlü**
> 5. Fiyatı kırmızı yazmak erkeklerde algılanan indirimi artırır. İlgi düzeyi yüksek olduğunda bu etki kaybolur (Puccinelli vd., 2013). **Orta**
> 6. WebAIM Million 2026 raporuna göre ana sayfaların **%83,9'unda** düşük kontrastlı metin var (2025'te %79,1'di). Rapor, AI destekli kodlamayı gerilemenin olası nedenlerinden biri olarak anıyor. **Güçlü**
> 7. Bugün yasal ölçüt WCAG 2.2 AA'dır (metinde 4.5:1, büyük metin ve UI öğelerinde 3:1). APCA, WCAG 3 taslağından çıkarıldı ve WCAG 3 en erken ~2030'da bekleniyor. **Güçlü**
> 8. Açık zemin (pozitif polarite) görme keskinliği ve düzeltme okumasında daha iyi sonuç veriyor. Fark, punto küçüldükçe büyüyor (Piepenbrock vd., 2013; NN/g). **Güçlü**
> 9. Okuma hızı ve anlama 18 pt'ye kadar puntoyla birlikte artıyor (Rello vd., 2016, n=104). iOS Safari, 16px'ten küçük input'larda odaklanınca sayfayı yakınlaştırıyor. **Güçlü**
> 10. Serif ile sans arasında ekranda tutarlı bir okunabilirlik farkı yok (Arditi & Cho, 2005; NN/g). Kişiden kişiye fontlar arası hız farkı %35'e kadar çıkabiliyor (Wallace vd., 2022). **Güçlü**
> 11. Chromium testinde `text-transform: uppercase` yalnızca `lang="tr"` ile doğru çalıştı (i → İ). **`capitalize` ise lang="tr" ile bile "İndirim" yerine "Indirim" üretti.** JS `toUpperCase()` da hatalı sonuç veriyor. **Güçlü (kendi testimiz)**
> 12. KPT'nin CSS'inde 72 farklı font-size, 71 farklı hex ve 6 font ailesi var. px cinsinden font-size bildirimlerinin 116/254'ü ≤13px. Arama input'u 12px olduğu için iOS'ta zoom tetikleniyor. Manrope'un varsayılan rakamları orantılı, bu yüzden fiyatlarda `tabular-nums` gerekiyor. **Gözlem**

## 1. Renk psikolojisi: kanıt mi, mit mi?

| İddia | Durum | Kanıt |
|---|---|---|
| "Kırmızı/turuncu CTA her zaman kazanır" | **Mit** | Performable testi, yeşil bir sayfada kırmızının öne çıkmasını ölçtü. Rengin kendisini değil, çevresinden ayrışmasını (Von Restorff) gösterdi. |
| "Renkler evrensel anlam taşır" | **Kısmen yanlış** | Ortak örüntü güçlü (r=.88), ancak ülke ve dil yakınlığı sonuçları değiştiriyor (Jonauskaite vd., 2020). Türkiye'nin örneklemde olup olmadığını doğrulayamadım. |
| "Kararların %90'ı renkle verilir" | **Abartı** | Singh (2006) bir derlemedir. Aralık, tek bir sayıya indirgenerek yayıldı. |
| Renk marka kişiliğini etkiler | **Orta** | Labrecque & Milne (2012) bunu 4 çalışmayla test etti. Düşük doygunluk + yüksek açıklık → sofistike; yüksek doygunluk → heyecan/sağlamlık. |
| Mavi/yeşil logo "çevreci" algılanır | **Orta** | Sundar & Kellaris (2017) bunu gösterdi. Mavi, yeşilden "daha yeşil" algılandı. |
| Kırmızı çekicilik/romantizm etkisi | **Zayıf** | Meta-analizde küçük bir etki bulundu (d=0,26 ve 0,13) ve yayın yanlılığı işaretleri var (Lehmann, Elliot, Calin-Jageman, 2018). |
| Doygun ürün görseli daha büyük algılanır | **Orta** | Hagtvedt & Brasel (2017, JCR). Sneaker görsellerinde doygunluğu yapay olarak artırmak beden ve hacim beklentisini bozabilir (tahmin). |

**CTA renginin gerçekte gösterdiği:** Kazanan renk, sayfadaki diğer her şeyden ayrışan renktir. KPT'de vurgu rengi tek (bordo #741E32). Bu yüzden bordo yalnızca birincil eyleme (Sepete Ekle, Ödemeye Geç) ve indirimli fiyata ayrılmalı. Dekoratif çizgi, ikon ya da başlıkta kullanıldıkça ayırt ediciliği azalır (izolasyon ilkesi, NN/g 2017 göstergeç çalışmasıyla uyumlu).

**Nötr palet ve premium algı:** Labrecque & Milne'a göre siyah ve koyu tonlar sofistike algısıyla ilişkili. Bu durum lüks moda sitelerinde gözlenen siyah-beyaz ağırlıklı paletlerle uyumlu, ancak "nötr palet dönüşümü artırır" diyen doğrudan bir deney bulamadım. **Zayıf.**

### KPT tonlarının çağrışımları

| Ton | Hex | Çağrışım | Kanıt |
|---|---|---|---|
| Kömür/siyah | #171B1C | Sofistike, premium | Orta (Labrecque & Milne) |
| Adaçayı / kırık beyaz | #E5E8E3, #F3F4F1 | Sakin, doğal, çevreci | Zayıf–Orta. Doğrudan "adaçayı" çalışması yok, yeşil/mavi → çevreci için bkz. Sundar & Kellaris. #F3F4F1, Pantone 2026 "Cloud Dancer" (11-4201, kırık beyaz) eğilimiyle örtüşüyor, ancak bu dönüşüm kanıtı değil. |
| Bordo | #741E32 | Kırmızının heyecanı ile koyu tonun sofistikeliği arasında | Zayıf (çıkarım). **Türkiye bağlamı:** bordo, umuma mahsus pasaportun ("bordo pasaport") ve Trabzonspor'un ("bordo-mavi") rengi. Bordo + mavi kombinasyonundan kaçınılmalı, yoksa kulüp ürünü gibi okunabilir. |
| Espresso | #2B211D | Toprak, deri, sağlamlık (kahverengi → ruggedness) | Orta |
| Kum/krem | #D8CFC3 | Sıcak nötr, "quiet luxury" | Zayıf (trend gözlemi) |

Türkiye'de kırmızı-beyaz ulusal bayrakla güçlü biçimde ilişkilidir. Kırmızı-sarı (Galatasaray) ve sarı-lacivert (Fenerbahçe) gibi kulüp renk çiftleri de yerel çağrışım taşır (gözlem; dikkat edilecek nokta, kanıt değil). Yeşilin dinî çağrışımı ile ilgili kültürlerarası derleme için bkz. Aslam (2006).

## 2. Kontrast

- **WCAG 2.2 AA:** normal metin 4.5:1; büyük metin (≥24px ya da ≥18.66px kalın) 3:1; UI bileşen sınırları ve odak göstergesi 3:1 (1.4.11); dokunma hedefi en az 24×24 CSS px (2.5.8). Kullanıcı satır yüksekliğini 1.5, paragraf aralığını 2em'e çıkardığında içerik bozulmamalı (1.4.12).
- **APCA (deneysel):** Lc 90 tercih edilen gövde metni; Lc 75, 18px/400 ya da 16px/500 gövde için minimum; Lc 60, 24px/400 ya da 16px/700 içerik metni; Lc 45 başlıklar; Lc 30 placeholder ve devre dışı metin. **Bir yasal ölçüt değil.** Önce WCAG 2'yi geçin, APCA'yı ikinci kontrol olarak kullanın (Roselli, 2026).
- **Karanlık mod:** Kullanıcıların yaklaşık üçte biri karanlık, üçte biri açık, üçte biri ikisini birlikte kullanıyor ve kullanıcılar karanlık mod eksikliğini pek fark etmiyor (NN/g, 2023). Saf #000 zemin ve doygun vurgu renklerinden kaçının. Beyaz zeminli ürün fotoğrafları karanlık temada "kutu" gibi görünür. Chrome Android'in otomatik koyulaştırmasını kapatmak için `<meta name="color-scheme" content="only light">` kullanılır (Chrome, 2021).

### KPT paleti kontrast matrisi (kendi hesabım: WCAG oranı / APCA Lc)

| Metin \ Zemin | #FFFFFF | #F3F4F1 | #E5E8E3 | #D8CFC3 | #171B1C | #741E32 |
|---|---|---|---|---|---|---|
| #171B1C | 17.36 / 104 | 15.72 / 97 | 14.04 / 90 | 11.27 / 77 | – | **1.63 ✗** |
| #56605E | 6.50 / 82 | 5.89 / 75 | 5.26 / 68 | **4.22 ✗** | **2.67 ✗** | ✗ |
| #741E32 | 10.64 / 94 | 9.63 / 87 | 8.60 / 80 | 6.90 / 66 | ✗ | – |
| #FFFFFF | – | ✗ | ✗ | ✗ | 17.36 | 10.64 |

Sonuçlar:
- (a) Gri metin (#56605E) kum zeminde AA'yı geçemiyor.
- (b) Adaçayı zeminde APCA Lc 68, yani 18px/400 gövde metni için sınırın altında.
- (c) #2B211D ile #171B1C arasındaki fark yalnızca 1.11:1. İkisi birbirinden ayrıştırıcı olarak kullanılamaz.
- (d) Mevcut ayırıcı çizgi #D2D8D3, kâğıt zeminde 1.31:1. Yalnızca dekoratif çizgi için uygundur. Input ve beden çipi sınırları için 3:1 gerekir.

## 3. Tipografi

**Satır uzunluğu:** Gövde metni için 50–75 karakter önerilir, ideal 66. Uzun satırlar korkutucu algılanıyor ve okunmadan atlanıyor (Baymard, 2022). WCAG 1.4.8 (AAA) üst sınırı 80 karakter olarak koyar. Dyson & Haselgrove'a (2001) göre ~55 karakter normal okumada anlama ile hız arasında iyi bir denge sağlıyor. **Güçlü.** Uygulama: `max-width: 65ch`.

**Punto ve satır yüksekliği:** Rello vd. (2016) 18 pt'ye kadar artışın okunabilirliği iyileştirdiğini, satır aralığının ise belirgin bir etkisi olmadığını buldu. Apple HIG'de iOS için varsayılan 17pt, minimum 11pt; ince ağırlıklardan (Ultralight, Thin, Light) kaçınılmalı. Material 3 ölçeğinde Body Large 16/24, Body Medium 14/20, Label Small 11/16. Mobilde gövde metni ≥16px, form alanları **≥16px** olmalı (iOS zoom). `maximum-scale=1` ile yakınlaştırmayı kapatmak erişilebilirliği bozar (WCAG 1.4.4).

**Serif ve sans:** Ekranda anlamlı bir okunabilirlik farkı yok. Seçimi marka belirler (NN/g, 2012; Arditi & Cho, 2005). Ancak x-yüksekliği önemli: **Cormorant Garamond'un x-yüksekliği 0,386 em, Manrope'unki 0,540 em** (fontTools ile ölçtüm). Aynı px değerinde Cormorant'ın küçük harfleri ~%29 daha küçük görünür. 24px Cormorant ≈ 17px Manrope. **Cormorant'ı 32px altında kullanmayın.**

**Font eşleştirme:** Bu konuda kontrollü bir çalışma bulamadım (**Zayıf**). Uzman pratiği şudur: tek bir değişken sans gövde fontu, en fazla bir kontrast ailesi (serif display) ve logo fontu yerine SVG logo. Gözlem: New Balance TR, Proxima Nova + EB Garamond (serif vurgu) kullanıyor, yani KPT'nin sans+serif yaklaşımı sektörde var.

**Değişken fontlar:** Sitelerin %39–41'i değişken font kullanıyor. Medyan font dosyası ~35 KB (Web Almanac, 2025). KPT, Manrope'u 5 statik dosya olarak yüklüyor (≈84 KB). Google Fonts'un Manrope değişken sürümü (200–800) latin (24 KB) + latin-ext (14 KB) = **38 KB** tutuyor.

**Türkçe karakterler (kendi testlerim):**
- Ğ, ğ, Ş, ş ve İ Google'ın **latin-ext** alt kümesinde, ı ise **latin** alt kümesinde. Türkçe sayfada iki alt küme de her zaman indirilir, ikisi de preload edilmeli.
- Manrope, Cormorant Garamond ve Archivo Black'te Türkçe glifler var. **Archivo Black'te ₺ (U+20BA) glifi yok.** Manrope ve Cormorant'ta var.
- Manrope'un `locl` özelliği TRK dil sistemini içeriyor. `lang="tr"` olduğunda "fi" bağlı harfi Türkçe kurallarla bastırılır (Glyphs).
- Chromium 141 testi:

| Girdi | Sonuç |
|---|---|
| `lang="tr"` + uppercase: "istanbul iğne çizgi" | "İSTANBUL İĞNE ÇİZGİ" ✓ |
| `lang="en"` ya da lang yok + uppercase | "ISTANBUL IĞNE ÇIZGI" ✗ |
| `lang="tr"` + **capitalize**: "indirim ıhlamur" | "**Indirim** Ihlamur" ✗ |
| `lang="en"` + lowercase: "İSTANBUL" | "i̇stanbul" (birleşik nokta) ✗ |
| JS `toUpperCase()` / `toLocaleUpperCase('tr-TR')` | "ISTANBUL" ✗ / "İSTANBUL" ✓ |

KPT `<html lang="tr">` kullanıyor, bu doğru. Ancak dinamik olarak eklenen ya da `lang` değeri farklı bileşenlerde sorun çıkabilir.

**Sayısal tipografi:** Manrope'un varsayılan rakamları **orantılı** (font biriminde "1" = 780, "0" = 1220). Fiyat, beden ızgarası, sepet tutarı ve sayaçlarda `font-variant-numeric: tabular-nums` zorunlu (KPT CSS'te 9 yerde zaten var). Fiyat biçimi gözlemleri: KPT "14.999,00 TL", Nike TR "8.699₺", `Intl.NumberFormat('tr-TR', {style: 'currency', currency: 'TRY'})` çıktısı "₺1.299,90". Virgül ve kuruş içeren fiyatlar daha "büyük" algılanıyor (Coulter, Choi, Monroe, 2012, ABD örneklemi, **Orta**). Kuruş sıfırsa "14.999 TL" biçimi önerilir.

## 4. Sneaker/moda e-ticaretinde tipografi sistemleri (gözlem, 2026-10-04 ajan taramaları)

| Site | Aileler | Boyut/renk | Buton |
|---|---|---|---|
| Nike TR | Helvetica Now Text Medium (500), display: Nike Futura ND | Hero 76px masaüstü / 40px mobil; gövde 16px; metin #111111, ikincil #707072; görsel zemini #F5F5F5; indirim/rozet #D33918 | Hap biçimli, 30px radius |
| END. | Proxima Nova 400/600 | 14px masaüstü, 16px mobil; #1A1A1A | Büyük harf, 16px/600, 46px yükseklik, 2px radius |
| Foot Locker UK | Maven Pro + FL Classic | Hero 48px masaüstü / 40px mobil; #0E1111; indirim #D12E20 | 4px radius |
| New Balance TR | Proxima Nova Semibold + EB Garamond Medium | İndirim #CF0A2C | – |
| SNS | SNSInter (özel Inter) | #F5F5F5 zemin, vurgu #60FF7A | – |
| Aimé Leon Dore | Söhne | Büyük harf 10px, harf aralıklı (okunması zor) | – |

Ortak örüntü: tek bir grotesk gövde fontu, 2–3 gri tonu, tek bir indirim rengi ve görsellerde açık gri zemin.

## 5. KPT için önerilen token sistemi

```css
:root{
  /* Zeminler */
  --bg:#F3F4F1; --surface:#FFFFFF; --surface-alt:#E5E8E3;
  --surface-warm:#D8CFC3;          /* yalnızca dekoratif blok; üzerinde yalnızca --text */
  --surface-inverse:#2B211D;       /* footer/duyuru şeridi; üzerinde #F3F4F1 (14.22:1) */
  /* Metin */
  --text:#171B1C; --text-muted:#56605E;   /* muted: yalnız --bg/--surface üstünde */
  --text-muted-strong:#4A5351;            /* --surface-alt 6.42:1, --surface-warm 5.15:1 */
  /* Vurgu: yalnızca birincil CTA + indirimli fiyat + aktif durum */
  --accent:#741E32; --accent-hover:#5E1828; --accent-tint:#F2E6E9; --on-accent:#FFFFFF;
  /* Çizgiler */
  --border:#D2D8D3;                /* dekoratif */
  --border-strong:#7D8783;         /* input, beden çipi: 3.36:1 bg / 3.00:1 surface-alt */
  /* Durum */
  --success:#256246; --error:#B42318; --warning:#7A4F00;
  --focus:#741E32;                 /* outline 2px, offset 2px */
  /* Tipografi */
  --font-sans:'Manrope',system-ui,sans-serif;   /* değişken 200–800 */
  --font-serif:'Cormorant Garamond',Georgia,serif; /* yalnız ≥32px editoryal */
  --fs-xs:.75rem;   /* 12/16 rozet, yasal; büyük harf +.06em */
  --fs-sm:.875rem;  /* 14/20 meta, kart marka satırı */
  --fs-md:1rem;     /* 16/24 gövde, input, kart ürün adı */
  --fs-lg:1.125rem; /* 18/28 PDP açıklama */
  --fs-xl:1.25rem;  /* 20/28 fiyat (PDP mobil), 700, tabular */
  --fs-2xl:1.5rem;  /* 24/32 H3, PDP fiyat masaüstü */
  --fs-3xl:clamp(1.75rem,1.4rem + 1.2vw,2rem);  /* 28→32 H2 */
  --fs-4xl:clamp(2rem,1.5rem + 2vw,2.5rem);     /* 32→40 H1 */
  --fs-display:clamp(2.5rem,1.5rem + 4vw,4.5rem); /* 40→72 hero, lh 1.05, 800, -.02em */
}
```

Karanlık mod sonraya bırakılmalı ve kullanılırsa şu değerlerle: zemin #121615, yüzey #1E2324, metin #ECEDEA (15.52:1), ikincil #B4BCB7 (8.94:1), vurgu metni #E6A9B6 (8.86:1). Birincil buton #F3F4F1 zemin üzerine #171B1C metin. Bordo, koyu zeminde yalnızca 1.63:1 veriyor.

## KPT için uygulama kuralları

1. **Kural:** Bordo (#741E32) yalnızca birincil CTA, indirimli fiyat ve aktif sekme/çip için kullanılsın. **Neden:** Vurgu, ancak tek ve seyrek olduğunda öne çıkar. **Kanıt:** Performable 2011 (izolasyon), NN/g 2017. Orta.
2. **Kural:** #56605E yalnızca #F3F4F1 ya da #FFFFFF üzerinde ve ≥14px kullanılsın. Adaçayı ve kum zeminde #4A5351 kullanılsın. **Neden:** Kum zeminde 4.22:1 ile AA'dan kalıyor, adaçayında Lc 68. **Kanıt:** WCAG 1.4.3, APCA hesabı. Güçlü.
3. **Kural:** Input, beden çipi ve checkbox sınırı #7D8783 olsun, #D2D8D3 yalnızca ayırıcı çizgide kullanılsın. **Neden:** UI sınırları 3:1 gerektirir. **Kanıt:** WCAG 1.4.11. Güçlü.
4. **Kural:** Tüm input/select/textarea `font-size: 16px` olsun (arama kutusundaki mevcut 12px düzeltilsin). Yakınlaştırma kapatılmasın. **Neden:** iOS'ta odaklanınca zoom tetikleniyor. **Kanıt:** iOS Safari davranışı, WCAG 1.4.4. Güçlü.
5. **Kural:** Font aileleri 3'e indirilsin: Manrope (değişken, latin + latin-ext preload), Cormorant Garamond (tek ağırlık, ≥32px), SVG logo. Space Grotesk, Phudu, Anton ve Archivo Black kaldırılsın. **Neden:** Archivo Black'te ₺ yok, Manrope değişken sürümü 84 KB yerine 38 KB, aile sayısı tutarlılığı bozuyor. **Kanıt:** fontTools ölçümü, Web Almanac 2025. Güçlü.
6. **Kural:** CSS'te yalnızca 9 basamaklı tip ölçeği (`--fs-*`) kullanılsın. Gövde ≥16px olsun, 12px yalnızca rozet ve yasal metinde. 10–11px tamamen kaldırılsın. **Neden:** 72 farklı boyut var ve bildirimlerin yarıya yakını ≤13px. **Kanıt:** Rello 2016, Apple HIG (11pt minimum). Güçlü.
7. **Kural:** Negatif harf aralığı yalnızca ≥24px başlıklarda olsun (−.01/−.02em). Gövde 0, küçük büyük-harf etiketleri +.06em. **Neden:** −.04em değeri 12–14px metinde harfleri sıkıştırıyor (KPT ekran görüntüsünde düzensiz aralık gözlendi). **Kanıt:** Gözlem + uzman pratiği. Zayıf–Orta.
8. **Kural:** Metinlerde `text-transform: capitalize` kullanılmasın, doğru yazım kaynakta yapılsın. Büyük harf yalnızca CSS uppercase + `lang="tr"` ile ya da JS'te `toLocaleUpperCase('tr-TR')` ile üretilsin. **Neden:** Chromium'da capitalize "İndirim"i "Indirim" yapıyor. **Kanıt:** Kendi testim. Güçlü.
9. **Kural:** Fiyat, beden ve tutarlarda `tabular-nums` kullanılsın. Biçim "14.999 TL" (kuruş sıfırsa gösterilmesin). İndirimde yeni fiyat bordo 700, eski fiyat #56605E üstü çizili ve 14px. **Neden:** Manrope'un rakamları orantılı; virgül ve kuruş fiyatı daha büyük gösteriyor. **Kanıt:** fontTools, Coulter 2012, Puccinelli 2013. Orta.
10. **Kural:** Açıklama ve blog metni `max-width: 65ch`, `line-height: 1.5–1.6` olsun. **Neden:** 50–75 karakter okunmayı artırıyor. **Kanıt:** Baymard 2022, Dyson & Haselgrove 2001. Güçlü.
11. **Kural:** Odak göstergesi: `outline: 2px solid #741E32; outline-offset: 2px`. **Neden:** Bordo butonun üzerinde koyu halka 1.63:1 kalıyor, offset ile kâğıt zemin üzerinde 9.63:1 elde ediliyor. **Kanıt:** WCAG 2.4.7/2.4.13. Güçlü.
12. **Kural:** Sitede yalnızca açık tema olsun ve `color-scheme: only light` tanımlansın. Karanlık mod tokenları hazırda tutulsun. **Neden:** Açık mod okunabilirlik açısından daha iyi; beyaz zeminli ürün görselleri koyu temada bozuluyor. **Kanıt:** Piepenbrock 2013, NN/g 2020/2023. Orta.

## Kaynaklar

- Labrecque & Milne (2012), Exciting red and competent blue: https://doi.org/10.1007/s11747-010-0245-y
- Auburn tezi (Labrecque & Milne bulgularının özeti): https://etd.auburn.edu/bitstream/handle/10415/3683/clarethesis__gradschool.pdf?sequence=2
- Jonauskaite vd. (2020): https://doi.org/10.1177/0956797620948810
- Singh (2006): https://doi.org/10.1108/00251740610673332
- Puccinelli vd. (2013): https://doi.org/10.1016/j.jretai.2013.01.002
- Sundar & Kellaris (2017): https://doi.org/10.1007/s10551-015-2918-4
- Lehmann, Elliot, Calin-Jageman (2018): https://doi.org/10.1177/1474704918802412
- Hagtvedt & Brasel (2017): https://doi.org/10.1093/jcr/ucx039
- Aslam (2006): https://doi.org/10.1080/13527260500247827
- Coulter, Choi, Monroe (2012): https://doi.org/10.1016/j.jcps.2011.11.005
- CTA testinin bağlamı: https://atticusli.com/blog/posts/cta-button-ab-tests-why-button-color-tests-are-worthless/
- WebAIM Million 2026: https://webaim.org/projects/million/
- WCAG 2.2 Contrast Minimum: https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html
- WCAG 2.2 Non-text Contrast: https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html
- WCAG 2.2 Target Size: https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html
- WCAG 2.2 Text Spacing: https://www.w3.org/WAI/WCAG22/Understanding/text-spacing.html
- APCA in a Nutshell: https://git.apcacontrast.com/documentation/APCA_in_a_Nutshell
- Roselli, WCAG3 Contrast as of April 2026: https://adrianroselli.com/2026/04/wcag3-contrast-as-of-april-2026.html
- NN/g Dark Mode vs Light Mode: https://www.nngroup.com/articles/dark-mode/
- NN/g Dark Mode issues (2023): https://www.nngroup.com/articles/dark-mode-users-issues/
- Piepenbrock vd. (2013): https://doi.org/10.1080/00140139.2013.790485
- Chrome Auto Dark Theme: https://developer.chrome.com/blog/auto-dark-theme
- NN/g Flat UI (2017): https://www.nngroup.com/articles/flat-ui-less-attention-cause-uncertainty/
- Baymard satır uzunluğu: https://baymard.com/blog/line-length-readability
- Dyson & Haselgrove (2001): https://doi.org/10.1006/ijhc.2001.0458
- Rello, Pielot, Marcos (2016): https://doi.org/10.1145/2858036.2858204
- Wallace vd. (2022): https://doi.org/10.1145/3502222
- Arditi & Cho (2005): https://doi.org/10.1016/j.visres.2005.06.013
- NN/g Serif vs Sans HD: https://www.nngroup.com/articles/serif-vs-sans-serif-fonts-hd-screens/
- Apple HIG Typography: https://developer.apple.com/design/human-interface-guidelines/typography
- Material 3 type scale (Flutter TextTheme): https://api.flutter.dev/flutter/material/TextTheme-class.html
- iOS input zoom: https://css-tricks.com/?p=339455 ve https://specification.website/spec/accessibility/mobile-form-inputs/
- Web Almanac 2025 Fonts: https://almanac.httparchive.org/en/2025/fonts
- Turkish locl / fi bağı: https://glyphsapp.com/learn/localize-your-font-turkish
- Google Fonts CSS API (alt küme ölçümü): https://fonts.googleapis.com/css2?family=Manrope:wght@200..800
- Pantone 2026 Cloud Dancer: https://www.pantone.com/color-of-the-year/2026
- Trabzonspor renkleri: https://en.wikipedia.org/wiki/Trabzonspor
- Türk pasaportu: https://en.wikipedia.org/wiki/Turkish_passport
- Gözlem: KPT CSS/Lighthouse ve rakip ajan taramaları (scratchpad, 2026-10-04). Ayrıca bkz. [[KPT Store Denetimi]]
