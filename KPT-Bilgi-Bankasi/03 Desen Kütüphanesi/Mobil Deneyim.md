---
tür: desen
bileşen: mobil
etiketler: [desen, mobil]
---

# Mobil Deneyim

> [!summary] Kural özeti
> Türkiye'de e-ticaret trafiğinin büyük kısmı mobilden gelir (rakamlar: [[Türkiye E-ticaret Pazarı]]). Tasarım mobil öncelikli yapılır; masaüstü genişletmedir.

## Kurallar

1. **Sticky alt eylem çubuğu (PDP):** 64–72 px, `--paper` zemin, üst çizgi; solda fiyat, sağda "Sepete ekle" (beden seçilmemişse "Beden seç" → beden ızgarasına kaydırır). Nike TR mobilde 62 px'lik sabit "Sepete Ekle" çubuğu kullanıyor (bkz. [[Nike Türkiye]]). `env(safe-area-inset-bottom)` dahil.
2. **Başparmak bölgesi:** birincil eylemler ekranın alt yarısında; filtre ve sıralama sticky araç çubuğunda.
3. **Dokunma hedefleri:** ≥44×44 px, aralarında ≥8 px.
4. **Yazı:** gövde 16 px, meta ≥14 px, input 16 px (iOS yakınlaştırma).
5. **Filtre:** alt çekmece, altta "X ürünü göster".
6. **Galeri:** yatay kaydırma + sayaç; iki parmakla yakınlaştırma.
7. **Hero:** ≤1 ekran; altındaki bölüm görünür olmalı.
8. **Çerez penceresi:** alt şerit, ekranın ≤%30'u.
9. **Performans:** mobil LCP < 2,5 sn (mevcut 5,8 sn); görseller `srcset`/`sizes` ile, mobilde 800 px'i aşmayan sürümler.
10. **Hamburger menü** tek mantıkla, gerçek cihazda test (mevcut hata: [[KPT Store Denetimi]]).
11. Klavye türleri: telefon `inputmode="tel"`, e-posta `type="email"`, posta kodu `inputmode="numeric"`; `autocomplete` öznitelikleri.

İlgili: [[Ürün Sayfası]] · [[Header ve Navigasyon]] · [[E-ticaret UX Verileri]]
