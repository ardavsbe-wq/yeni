---
tür: uygulama
konu: tasarım-tokenları
etiketler: [uygulama, token, renk, tipografi]
---

# Tasarım Token Önerisi

> [!summary] Karar
> Mevcut üç token katmanı (`:root` kiremit/Anton, `.theme-atelier` krem/bordo/Cormorant, footwear adaçayı) **tek sisteme** indirilir. Nötr sıcaklık: **adaçayı** (ürünleri en iyi taşıyan, mevcut ana sayfanın çoğunluğu). Tek vurgu: **bordo**. Tek font ailesi: **Manrope** (logo Archivo Black kalır). Gerekçe ve kanıtlar: [[Renk ve Tipografi]], [[KPT Store Denetimi]].

## Renk

```css
:root {
  /* Nötrler (adaçayı eğilimli) */
  --ink:        #171B1C;  /* ana metin, koyu yüzey */
  --ink-2:      #3A4240;  /* ikincil metin (paper üstünde 9,4:1) */
  --muted:      #56605E;  /* yardımcı metin (paper üstünde 5,9:1) */
  --line:       #D2D8D2;  /* çizgiler, kutu kenarları */
  --surface:    #E5E8E3;  /* ürün görsel zemini, kart, hero */
  --surface-2:  #EDEFEA;  /* hover/ikincil yüzey */
  --paper:      #F3F4F1;  /* sayfa zemini */
  --white:      #FFFFFF;

  /* Vurgu: yalnızca birincil satın alma eylemleri ve seçili durum */
  --accent:       #741E32;  /* beyaz metin 10,6:1 */
  --accent-hover: #5E1828;
  --accent-soft:  #F1E4E8;  /* seçili filtre çipi zemini */

  /* Anlamsal (vurgudan ayrı) */
  --success: #2F6B4F;  --success-bg: #E4F2EA;
  --warning: #8A5A00;  --warning-bg: #FBF0D9;
  --danger:  #B42318;  --danger-bg:  #FDECEA;   /* hata, tükendi değil */
  --sale:    #B42318;                           /* indirim fiyatı ve rozeti */
}
```

- **Kaldırılacaklar:** `#BD3525` (kiremit), `#F3EFE7`/`#E9E2D7`/`#D8CFC3` krem-kum seti, `#2B211D` kahve buton, `#6A5D54` taupe (kum üstünde AA'yı geçmiyor).
- **Buton hiyerarşisi:** Birincil = `--accent` dolgu + beyaz; İkincil = `--ink` 1 px çerçeve + `--ink` metin; Üçüncül = altı çizili metin linki. İkincil eylemler (Sırala, Uygula, Filtre) **asla** bordo değil.
- **Durumlar:** odak halkası `2px solid var(--accent)` + 2 px ofset; tükendi = `--surface` zemin + `--muted` metin + üstü çizili.
- Koyu mod: e-ticarette zorunlu değil; yapılacaksa token düzeyinde.

## Tipografi

```css
:root {
  --font-sans: 'Manrope', system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif;
  --font-logo: 'Archivo Black', var(--font-sans);
  /* Ölçek (mobil → masaüstü, clamp) */
  --fs-display: clamp(40px, 6vw, 72px);  /* hero başlık, 800, -0.03em */
  --fs-h1:      clamp(30px, 4vw, 44px);  /* sayfa başlığı, 800, -0.02em */
  --fs-h2:      clamp(24px, 3vw, 32px);  /* bölüm başlığı, 700 */
  --fs-h3:      20px;                    /* kart/blok başlığı, 700 */
  --fs-body:    16px;                    /* gövde, 400, satır yüksekliği 1.6 */
  --fs-ui:      15px;                    /* ürün adı, buton, menü, 600 */
  --fs-meta:    14px;                    /* meta, fiyat yanı bilgi; ALT SINIR */
  --fs-eyebrow: 13px;                    /* büyük harf etiket, 700, 0.08em */
}
```

- 12–13 px gövde/meta metni kaldırılır; en küçük metin 13 px ve yalnızca büyük harf etiketlerde.
- Fiyatlar `font-variant-numeric: tabular-nums`.
- Türkçe: `<html lang="tr">` (mevcut doğru). `text-transform: uppercase` Türkçe "i → İ" dönüşümünü doğru yapar, ancak **`capitalize` kullanma**: Chromium testinde "indirim" → "Indirim" oluyor (bkz. [[Renk ve Tipografi]]). Baş harf büyütme metnin kendisinde yapılır.
- Archivo Black fontunda **₺ işareti yok**: logo fontu fiyatlarda kullanılmaz; fiyatlar Manrope ile "TL" veya ₺ olarak yazılır.
- Arama kutusu dahil tüm input'lar 16 px (mevcut arama kutusu 12 px, iOS'ta sayfa yakınlaşıyor). Sunucu tarafında İngilizce verilerde yerel ayardan bağımsız küçük harf (mevcut "whıte" hatası).
- Cormorant Garamond kaldırılır (yalnızca 4 öğede kullanılıyordu). Editoryal vurgu gerekiyorsa tek bir yerde (ör. kampanya başlıkları) ve sistem olarak.
- Font yükleme: Manrope değişken font (tek woff2, 400–800), `font-display: swap`, ana ağırlık preload.

## Boşluk, ızgara, şekil

```css
:root {
  --space-1: 4px; --space-2: 8px; --space-3: 12px; --space-4: 16px;
  --space-5: 24px; --space-6: 32px; --space-7: 48px; --space-8: 64px; --space-9: 96px;
  --gutter: clamp(16px, 3.6vw, 56px);
  --container: 1440px;
  --radius-0: 0;      /* butonlar, kutular, beden kutuları (mevcut keskin dil korunur) */
  --radius-pill: 999px; /* arama kutusu, filtre çipleri */
  --radius-full: 50%;   /* favori butonu */
  --shadow-drawer: 0 8px 32px rgb(23 27 28 / .16);
  --ease: cubic-bezier(.16, 1, .3, 1);
  --dur-fast: 150ms; --dur: 250ms;
}
```

- Izgara: 12 sütun, masaüstü 24 px, mobil 16 px aralık.
- Ürün görsel oranı: **4:5** her yerde (kart, PDP, karolar).
- Bölümler arası dikey boşluk: mobil 48 px, masaüstü 96 px.
- Hareket: yalnızca durum geçişleri (≤250 ms); `prefers-reduced-motion: reduce` ile kapatılır.

İlgili: [[AI Geliştirici Brief'i]] · [[Renk ve Tipografi]] · [[Görsel Tasarım ve Trendler 2026]]

## Doğrulanmış kontrastlar

| Çift | Oran |
|---|---|
| `--ink` / `--paper` | 15,72 |
| `--ink-2` / `--paper` | 9,36 |
| `--muted` / `--paper` | 5,89 |
| `--muted` / `--surface` | 5,26 |
| beyaz / `--accent` | 10,64 |
| beyaz / `--accent-hover` | 12,83 |
| `--accent` / `--accent-soft` | 8,61 |
| `--sale` / `--paper` | 5,95 |
| `--success` / `--success-bg` | 5,45 |
| `--warning` / `--warning-bg` | 5,24 |
| `--danger` / `--danger-bg` | 5,75 |

Hepsi küçük metin için WCAG AA (4,5:1) üstünde.
