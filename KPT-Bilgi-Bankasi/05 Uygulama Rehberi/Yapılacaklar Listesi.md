---
tür: uygulama
konu: yapılacaklar
etiketler: [uygulama, yol-haritası]
---

# Yapılacaklar Listesi

Öncelik: etki × efor. Her madde ilgili notla bağlantılı. Kabul kriterleri [[AI Geliştirici Brief'i]] içinde.

## P0: Kritik hatalar ve hızlı kazanımlar

- [ ] **Beden seçilince fiyatı güncelle**; seçimden önce fiyat aralığı göster; sepet fiyatı = ekrandaki fiyat → [[Ürün Sayfası]]
- [ ] **Hero'yu yeniden kur**: gerçek fotoğraf, ≤1 ekran, otomatik geçiş yok, `<img fetchpriority="high">`, WebP/AVIF ≤250 KB → [[Hero ve Banner Desenleri]]
- [ ] **Renk verisini temizle**: ~14 renk ailesi + swatch; I→ı küçük harf hatasını düzelt → [[Kategori Sayfası ve Filtreler]]
- [ ] **PDP'de tüm bedenleri göster**, tükenenler soluk + "Gelince haber ver" → [[Beden ve Kalıp]]
- [ ] **Mobil menü**: tek açma/kapama mantığı, gerçek cihazda test → [[Header ve Navigasyon]]
- [ ] **PDP güven bloğu**: teslim tarihi, iade, taksit, orijinallik → [[Güven Sinyalleri]]
- [ ] **Duyuru şeridi**: tarih/şehir yerine değer önerisi → [[Hero ve Banner Desenleri]]
- [ ] **Tek birincil buton rengi**: bordo yalnızca birincil eylemlerde → [[Tasarım Token Önerisi]]
- [ ] **Çerez penceresi**: alt şerit, seçim sayfayı yenilemesin → [[Güven Sinyalleri]]

## P1: Yapısal iyileştirmeler

- [ ] Menüye `Yeni gelenler · Erkek · Kadın · Çocuk · Markalar` + mega menü → [[Header ve Navigasyon]]
- [ ] PLP filtrelerini yeniden kur: çoklu seçim, beden ızgarası, renk örnekleri, anında uygulama, otomatik sıralama, filtre çipleri → [[Kategori Sayfası ve Filtreler]]
- [ ] Ürün adı standardı: Marka + Model + Renk; kalıp notları ve kodlar ayrı alanlara → [[Ürün Sayfası]]
- [ ] Ürün açıklaması şablonu: hikâye + künye (malzeme, taban, renk adı, stil kodu) → [[Ürün Sayfası]]
- [ ] Ürün görselleri: aynı zemin, 4:5, en az 6 açı → [[Ürün Sayfası]]
- [ ] Token sistemini teke indir, Cormorant ve kiremit/krem setini kaldır → [[Tasarım Token Önerisi]]
- [ ] Yazı boyutu tabanı: gövde 16 px, meta ≥14 px → [[Tasarım Token Önerisi]]
- [ ] Mobil sticky "Sepete ekle" çubuğu; adet seçiciyi kaldır → [[Mobil Deneyim]]
- [ ] Mini sepet çekmecesi, sepette otomatik adet güncelleme, alakalı çapraz satış → [[Sepet ve Ödeme]]
- [ ] Beden rehberi: marka bazlı tablolar + ölçüm çizimi → [[Ayakkabı Beden ve Kalıp]]
- [ ] Kullanıcının bedenini hatırla, PLP'de varsayılan filtre → [[Beden ve Kalıp]]
- [ ] Arama: Türkçe karakter eşdeğerliği, yazım toleransı, sıfır sonuç sayfası, sonuç görsellerini panel açılınca yükle → [[Arama]]
- [ ] Performans: CSS birleştirme + kritik CSS, görsel `srcset`, mobil LCP < 2,5 sn → [[E-ticaret UX Verileri]]
- [ ] Erişilebilirlik: `ol` yapısı, aria-label uyuşmazlığı, odak yönetimi → [[KPT Store Denetimi]]

## P2: Yayın öncesi zorunlular ve büyüme

- [ ] Yasal içerik: mesafeli satış sözleşmesi, ön bilgilendirme formu, KVKK, çerez politikası, ETBİS, iletişim bilgileri → [[Türkiye E-ticaret Pazarı]], [[Footer]]
- [ ] İndirim gösterimi: son 10 gün en düşük fiyat kuralı (1 Ağustos 2026), AI içerik etiketi, yalnızca alıcı yorumu → [[Türkiye E-ticaret Pazarı]]
- [ ] Slug URL, canonical, `Product`/`BreadcrumbList` JSON-LD, Open Graph; `noindex` kaldır → [[Ürün Sayfası]]
- [ ] Yorum ve kalıp geri bildirimi sistemi → [[Beden ve Kalıp]], [[Dönüşüm Vaka Çalışmaları]]
- [ ] Ödeme: taksit tablosu, misafir ödeme, kısa form → [[Sepet ve Ödeme]]
- [ ] Markalar sayfası: marka başına logo, kısa hikâye, öne çıkan modeller → [[KPT Store Denetimi]]
- [ ] E-bülten + İYS uyumlu onay; "Gelince haber ver" e-postaları → [[Footer]]
- [ ] Gerçek fotoğraf çekimi (ayakta ve yaşam tarzı) → [[Görsel Tasarım ve Trendler 2026]]
- [ ] Gerçek sunucuda performans ölçümü (TTFB < 200 ms önbellekli)
