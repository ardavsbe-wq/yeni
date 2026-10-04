---
tür: desen
bileşen: beden-secici
etiketler: [desen, beden, pdp, plp]
---

# Beden ve Kalıp

> [!summary] Kural özeti
> Ayakkabıda en büyük belirsizlik beden. Tüm beden aralığını göster, tükenenleri gizleme, kalıp bilgisini butonun yanında ver, kullanıcının bedenini hatırla. Ayrıntılı araştırma: [[Ayakkabı Beden ve Kalıp]].

## PDP beden seçici

```
Beden seç (EU)                     Beden rehberi →
┌────┐┌────┐┌────┐┌────┐┌────┐┌────┐
│ 38 ││38.5││ 39 ││39.5││ 40 ││40.5│   44×44 px min, 6 sütun (mobil 5)
└────┘└────┘└────┘└────┘└────┘└────┘
  ↑ tükenen: açık gri zemin, soluk metin, çapraz çizgi, tıklanınca "Gelince haber ver"
Kalıp: Normal kalıp. Arada kalırsan yarım numara büyük al.
```

- **Tükenen bedenler gizlenmez.** New Balance TR örneği: tükenen beden açık gri zemin `#F8F8F8` ve soluk metin `#727272`; seçili beden siyah dolgulu (bkz. [[New Balance Türkiye]]). KPT'de: seçili = `--accent` dolgu + beyaz metin; tükenen = `--surface` zemin, `--muted` metin, üstü çizili, `aria-disabled="true"` ama odaklanabilir (haber ver akışı için).
- Beden sistemi seçici (opsiyonel): `EU | US | UK | cm` sekmeleri; marka tablosundan dönüştürülür.
- Bedene göre fiyat farkı varsa kutunun altında küçük yazı (bkz. [[Ürün Sayfası]]).
- "Son 1 çift" gibi stok uyarısı yalnızca **gerçek** stok ≤2 iken ve sayaç olmadan.
- Beden seçilmeden "Sepete ekle"ye basılırsa: beden ızgarasına kaydır, kırmızı çerçeve + "Lütfen bedenini seç." (mevcut metin iyi).

## Kalıp bilgisi

- Ürün verisinde `kalip` alanı: `dar | normal | geniş` + serbest not ("Yarım numara büyük almanı öneririz.").
- Ürün adındaki notlar ("(2 numara büyük alınması tavsiye edilir.)") bu alana taşınır.
- Yorumlarda kalıp oylaması: "Küçük / Tam oldu / Büyük" → PDP'de özet çubuğu (Trendyol/Zalando deseni; bkz. [[Trendyol]], [[Zalando]]).

## Beden rehberi sayfası

1. Ayak ölçme rehberi: 3 adım + çizim (kâğıt, duvar, cetvel), cm cinsinden.
2. Marka bazlı tablolar (New Balance, Nike, adidas, Puma, Vans, Skechers): `cm | EU | US Erkek | US Kadın | UK`.
3. Çocuk beden tablosu ayrı.
4. Kalıp ipuçları (geniş ayak için NB 2E/4E vb.).
5. PDP'den açıldığında ilgili markanın tablosu açık gelir (modal veya yan çekmece).

## Kullanıcının bedenini hatırlama

"Numaranla başla"da veya PDP'de seçilen beden `localStorage`/hesapta saklanır; PLP'de "Bedenin: 42 ✕" çipi varsayılan filtre olur ve kartlarda "Bedeninde stokta" bilgisi gösterilir.

İlgili: [[Kategori Sayfası ve Filtreler]] · [[Sneaker Kültürü ve Alıcı Profili]]
