---
tür: desen
bileşen: plp-filtreler
etiketler: [desen, plp, filtre]
---

# Kategori Sayfası ve Filtreler

> [!summary] Kural özeti
> Filtreler müşterinin dilinde ve **çoklu seçimli** olur: beden ızgarası, renk örnekleri, marka onay kutuları, fiyat aralığı. Masaüstünde seçim anında uygulanır; mobilde alt çekmecede "X ürünü göster" butonuyla. Uygulanan filtreler çip olarak listenin üstünde görünür.

## Sayfa yapısı (yukarıdan aşağı)

1. Breadcrumb (`Ana sayfa / Erkek / Sneaker`).
2. H1 + sonuç sayısı: "Erkek Sneaker · 128 ürün".
3. (Opsiyonel) Alt kategori çipleri, yatay kaydırmalı: `Tümü` `Lifestyle` `Koşu` `Basketbol` `Terlik`.
4. Araç çubuğu (sticky, 48 px): mobilde `[Filtrele (2)]` `[Sırala: Önerilen ▾]`; masaüstünde sağda sıralama açılır menüsü (**seçince otomatik uygulanır, ayrı buton yok**).
5. Uygulanan filtre çipleri: `42 ✕` `Siyah ✕` `Nike ✕` · `Tümünü temizle`.
6. Ürün ızgarası: masaüstü 4 sütun (≥1280 px) / 3 sütun (1024–1279), mobil 2 sütun; 16–24 px boşluk.
7. Sayfalama: "Daha fazla göster" butonu + "48 / 128 ürün gösteriliyor" ilerleme metni; URL'de sayfa durumu korunur (geri tuşu aynı konuma döner).

## Filtre spesifikasyonu

| Filtre | UI | Kural |
|---|---|---|
| Numara | **Beden ızgarası** (44×44 px kutular, 5–6 sütun) | **Tam numara grubu**: "41" seçimi 41, 41⅓ ve 41.5'i getirir (aynı US Erkek 8; Nike'ta EU 41, adidas'ta 41⅓, NB'de 41.5; bu gruplama 12 satırın 11'inde markaları aynı gruba düşürüyor, bkz. [[Ayakkabı Beden ve Kalıp]]); çocuk ve yetişkin ayrı başlıklar; katalogdaki geçersiz değerler (ör. `43 2/3`) temizlenir. Kullanıcının "Numaranla başla"da seçtiği beden hatırlanır ve varsayılan filtre olur. Bkz. [[Ayakkabı Beden ve Kalıp]] |
| Renk | **Renk örnekleri** (28 px daire + etiket) | ~14 renk ailesi: Siyah, Beyaz, Gri, Bej/Krem, Kahverengi, Lacivert, Mavi, Yeşil, Kırmızı, Bordo, Pembe, Mor, Sarı/Turuncu, Çok renkli. Ham tedarikçi renk adı yalnızca PDP'de |
| Marka | Onay kutuları, ürün sayısıyla ("Nike (64)") | 6'dan fazlaysa arama kutulu liste |
| Kategori/Kullanım | Onay kutuları | Yalnızca aktif gruba ait kategoriler (Ayakkabı grubunda Mont, Oyun Kartları çıkmaz) |
| Kitle | Erkek / Kadın / Unisex / Çocuk | Menüden gelindiyse önceden seçili |
| Fiyat | Çift tutamaçlı kaydırıcı + iki sayı kutusu | TL, binlik ayraçlı |
| Stok | "Yalnızca stokta olanlar" anahtarı | Varsayılan açık; beden seçiliyse o bedende stok |
| İndirim | "İndirimli ürünler" anahtarı | Yalnızca gerçek indirim varken |

- Her seçenek yanında sonuç sayısı; 0 sonuç verecek seçenek pasif görünür.
- Masaüstü: sol kolon 260–280 px, sticky; gruplar açılır/kapanır, ilk 3 grup açık.
- Mobil: alt çekmece (bottom sheet), tam yükseklik; altta sticky `[Temizle]` `[128 ürünü göster]`.

## Ürün kartı anatomisi

```
┌───────────────────────┐
│ [Yeni] [−%20]     ♡   │  rozetler sol üst (en fazla 2), favori sağ üst 44×44
│                       │
│     ürün görseli      │  4:5 veya 1:1, tutarlı zemin (#E5E8E3), ürün ortalı, %8 iç boşluk
│                       │  hover: 2. görsel (yan/ayakta)
├───────────────────────┤
│ New Balance           │  marka 13–14 px 700
│ 9060 Sea Salt         │  model + renk adı 14–15 px, en fazla 2 satır
│ ● ● ● +2              │  renk sayısı (varsa)
│ 14.025 TL             │  fiyat 15–16 px 700, tabular-nums; indirimde eski fiyat üstü çizili + yüzde
└───────────────────────┘
```

- Fiyat "TL'den" ise karta "14.025–14.674 TL" aralığı veya "14.025 TL'den" + PDP'de beden bazlı fiyat (bkz. [[Ürün Sayfası]]).
- Kartın tamamı tıklanabilir; favori butonu ayrı hedef.

## Gözlenen örnekler

[[Zalando]] (kalıp uyarısı, filtre), [[Foot Locker]] (beden filtresinde ürün sayısı, EU/UK/US seçici), [[FLO]] ve [[Hepsiburada]] (yatay filtre çipleri, aktif filtre sayısı: Türk alıcının alışkın olduğu düzen), [[Trendyol]], [[New Balance Türkiye]] (filtrelerde ürün sayısı), [[Aimé Leon Dore]] ve [[Stüssy]] (minimal kart: yalnızca ad + fiyat).

İlgili: [[E-ticaret UX Verileri]] · [[Satın Alma Psikolojisi]] (Hick yasası, seçim yükü)
