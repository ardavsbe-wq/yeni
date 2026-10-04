---
tür: desen
bileşen: pdp
etiketler: [desen, pdp]
---

# Ürün Sayfası

> [!summary] Kural özeti
> PDP'nin işi belirsizliği yok etmek: ürün nasıl görünüyor, bana olur mu, kaça gelir, ne zaman gelir, beğenmezsem ne olur. Bu beş sorunun cevabı "Sepete ekle" butonunun 1 ekran yakınında olmalı.

## Düzen

**Masaüstü:** sol 7 sütun galeri (2 sütunlu dikey ızgara veya büyük görsel + küçük resimler), sağ 5 sütun sticky bilgi kolonu.
**Mobil:** galeri (kaydırmalı, nokta/sayaç "1 / 6"), altında bilgi; **sticky alt çubuk**: fiyat + "Sepete ekle" (beden seçilmemişse "Beden seç").

## Bilgi kolonu sırası

1. Marka (link) · rozet (Yeni / İndirim).
2. H1: **Marka + Model + Renk adı**: "New Balance 9060 Sea Salt". Altında kitle/kategori: "Unisex · Lifestyle sneaker".
3. Puan özeti (varsa): "★ 4,6 (128 değerlendirme) · Kalıp: normal" → yorumlara kaydırır.
4. **Fiyat**: seçilen bedenin fiyatı; beden seçilmemişse "14.025 – 14.674 TL". İndirimde eski fiyat üstü çizili + "−%20" + yürürlükteki indirim kuralı (eski fiyat = indirimden önceki son 10 günün en düşük fiyatı; 1 Ağustos 2026 değişikliği, uygulamadan önce doğrula), bkz. [[Türkiye E-ticaret Pazarı]]. Altında taksit satırı: "Peşin fiyatına 3 taksit" / "Aylık 4.675 TL'den başlayan taksitler" (gerçek koşullarla).
5. Renk seçimi: diğer renklerin küçük görselleri (varsa), seçili renk adı yazılı.
6. **Beden seçici**: bkz. [[Beden ve Kalıp]]: tam aralık, tükenen bedenler üstü çizili, beden bazlı fiyat farkı küçük yazı, "Beden rehberi" linki, kalıp notu.
7. **Birincil buton**: "Sepete ekle" (bordo, 52–56 px, tam genişlik). Adet seçici **yok** (sepette değiştirilebilir). Yanında favori (♡) ikon butonu.
8. **Güven bloğu** (3–4 satır, ikonlu, butonun hemen altında): "Tahmini teslim: 7–8 Ekim" · "30 gün ücretsiz iade" · "%100 orijinal ürün" · "Kapıda/mağazada değişim" (gerçek politikalarla). Bkz. [[Güven Sinyalleri]].
9. Akordeonlar: **Ürün açıklaması** (2–3 cümle hikâye + madde liste: üst malzeme, taban, kapanış, renk adı, stil kodu), **Kalıp ve beden** (kalıp notu, model ölçüleri), **Teslimat ve iade**, **Değerlendirmeler**.
10. Altında: "Bu modelle kombinle" / "Benzer modeller" (aynı kategori ve fiyat bandı; alakasız ürün yok) ve "Son baktıkların".

## Galeri

- En az 6 görsel: yan profil (dış), iç yan, üstten, arka, taban, ayakta (on-feet); tutarlı zemin ve 4:5 oran, kare kesme yok.
- Zoom: masaüstünde tıklayınca tam ekran, mobilde iki parmakla yakınlaştırma.
- Video veya 360° opsiyonel, kullanıcı başlatır.

## Beden bazlı fiyat (KPT'ye özgü)

> [!bug] Mevcut hata
> Beden seçilince fiyat güncellenmiyor; sepette farklı fiyat çıkıyor (38.5: 14.674 TL, 39.5: 14.480 TL, 40: 14.025 TL). Bkz. [[KPT Store Denetimi]].

Doğru davranış: beden kutusunda küçük satır fiyat farkı ("+455 TL") veya kutuda doğrudan fiyat (StockX/GOAT deseni, bkz. [[StockX]], [[GOAT]]); seçimde ana fiyat **anında** güncellenir ve `aria-live="polite"` ile duyurulur; sepete eklenen fiyat ekranda görülenle birebir aynıdır. En iyisi: tek fiyat politikası.

## Yapılandırılmış veri

`Product` + `Offer`/`AggregateOffer` (lowPrice/highPrice, priceCurrency TRY, availability), `BreadcrumbList`, Open Graph (`og:image` 1200×630). Canonical URL slug tabanlı.

İlgili: [[E-ticaret UX Verileri]] · [[Dönüşüm Vaka Çalışmaları]] · [[Satın Alma Psikolojisi]]
