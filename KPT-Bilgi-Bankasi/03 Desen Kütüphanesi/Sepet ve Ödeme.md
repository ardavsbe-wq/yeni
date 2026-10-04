---
tür: desen
bileşen: sepet-odeme
etiketler: [desen, sepet, checkout]
---

# Sepet ve Ödeme

> [!summary] Kural özeti
> Sürpriz yok: ürün sayfasında görülen fiyat, kargo ve toplam sepette aynen görünür. Misafir ödeme serbest, form kısa, ödeme yöntemleri ve taksit baştan belli. Ayrıntı ve veriler: [[E-ticaret UX Verileri]], [[Dönüşüm Vaka Çalışmaları]], [[Türkiye E-ticaret Pazarı]].

## Sepete ekleme geri bildirimi

Mevcut KPT davranışı iyi (satır içi mesaj + toast "Sepeti gör" + rozet). Önerilen yükseltme: **sağdan açılan mini sepet çekmecesi** (masaüstü 400 px, mobilde alttan): eklenen ürün görseli, ad, beden, fiyat; ara toplam; ücretsiz kargo ilerleme çubuğu; `[Sepete git]` `[Ödemeye geç]`; "Bununla iyi gider" 2–3 ürün.

## Sepet sayfası

- Satır: görsel · Marka + Model + Renk · "Beden: 39.5" (değiştirilebilir açılır menü) · adet (değişince **otomatik** güncellenir, "Güncelle" butonu yok) · fiyat · "Kaldır" ve "Favorilere taşı".
- Özet kutusu (masaüstünde sticky sağ kolon, mobilde altta): Ara toplam · Kargo (tutar veya "Ücretsiz") · İndirim kodu (katlanmış link "İndirim kodun var mı?") · **Toplam (KDV dahil)** · bordo "Ödemeye geç" · ödeme logoları (Visa, Mastercard, Troy, banka kartları) · taksit notu · güven satırı ("Güvenli ödeme · 30 gün iade").
- Ücretsiz kargo ilerleme çubuğu: "Ücretsiz kargoya 320 TL kaldı" (yalnızca gerçek eşik varsa).
- Çapraz satış: yalnızca alakalı (aynı kitle, tamamlayıcı ürün: çorap, bakım ürünü); mevcut sitedeki Panini albümü önerisi gibi alakasız öneri yok.
- Boş sepet: mevcut metin korunur ("Sepetin yeni keşiflere açık.") + "Son baktıkların".

## Ödeme (checkout)

- Tek sayfa veya en fazla 3 adım (Teslimat → Ödeme → Onay), ilerleme göstergesi.
- **Misafir ödeme** varsayılan seçenek; hesap oluşturma sipariş sonrası tek tıkla.
- Form: ad soyad, telefon, e-posta, il/ilçe (açılır menü), açık adres; fatura adresi "teslimat adresiyle aynı" varsayılan işaretli. `autocomplete` öznitelikleri, mobilde doğru klavye (`inputmode="tel"`, `type="email"`), 16 px input.
- Ödeme: kart (taksit tablosu banka bazlı, kart numarası girilince otomatik), dijital cüzdanlar, varsa kapıda ödeme. 3D Secure akışı.
- Yasal: ön bilgilendirme formu ve mesafeli satış sözleşmesi onayı, sipariş butonunda ödeme yükümlülüğünü belirten metin (bkz. [[Türkiye E-ticaret Pazarı]]).
- Sipariş özeti her adımda görünür; ürün görselleriyle.

İlgili: [[Güven Sinyalleri]] · [[Satın Alma Psikolojisi]]
