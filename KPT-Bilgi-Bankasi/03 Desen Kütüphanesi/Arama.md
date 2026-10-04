---
tür: desen
bileşen: arama
etiketler: [desen, arama]
---

# Arama

> [!summary] Kural özeti
> Mevcut KPT arama paneli iyi bir temel (canlı sonuç, sonuç sayısı, öneriler). Geliştirilecekler: yazım hatası toleransı, Türkçe karakter eşdeğerliği, beden/renk anlama, sıfır sonuç sayfası, performans.

## Spesifikasyon

- Masaüstünde header'da görünür arama kutusu (≥280 px); mobilde ikon → tam ekran panel, klavye otomatik açılır.
- Boş durumda: "Popüler aramalar" (Samba, 9060, Mind 001...), "Son aramaların", kategori kısayolları.
- Yazarken (≥2 karakter, 150–250 ms debounce): öneri kelimeler (vurgulu eşleşme) + ilk 4–6 ürün (görsel, marka, model, fiyat) + "Tüm sonuçları gör (9)".
- **Eşdeğerlik:** `ı/i`, `ş/s`, `ğ/g`, `ü/u`, `ö/o`, `ç/c` eşleşir; "samba", "Samba OG", "sambA" aynı; "nb 9060" → New Balance 9060; yaygın yazım hataları ("adiddas", "nıke").
- **Niyet anlama:** "siyah 42 nike" → Nike + Siyah + 42 filtreli PLP.
- **Sıfır sonuç:** "‘xyz’ için sonuç bulamadık" + yazım önerisi + popüler kategoriler + iletişim linki; asla boş sayfa.
- Sonuç görselleri yalnızca panel açıldığında yüklenir (mevcut sitede 343 gizli `<img>` var, bkz. [[KPT Store Denetimi]]).
- Erişilebilirlik: `role="combobox"`, `aria-expanded`, `aria-activedescendant`, ok tuşlarıyla gezinme, sonuç sayısı `aria-live`.

İlgili: [[Header ve Navigasyon]] · [[E-ticaret UX Verileri]]
