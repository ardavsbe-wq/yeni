---
tür: rakip-analizi
site: Türkiye çok markalı sneaker mağazaları (Sneaks Up, Superstep, Sportive, Korayspor, Lescon, Instreet)
url: [https://www.sneaksup.com/, https://www.superstep.com.tr/, https://www.sportive.com.tr/, https://www.korayspor.com/, https://www.lescon.com.tr/, https://www.instreet.com.tr/]
ülke: TR
segment: çok markalı sneaker / spor perakendesi (doğrudan rakip)
erişim: kısmi
erişim-ayrıntı: "Superstep: kısmi (sunucu HTML'i, JS'siz render) · Sportive: kısmi (sunucu HTML'i + RSC verisi) · Sneaks Up: tarayıcı engellendi (Cloudflare 403), metin WebFetch ile · Korayspor: tarayıcı engellendi (Cloudflare 403), metin WebFetch ile · Lescon: tarayıcı engellendi (Cloudflare 403), metin WebFetch ile · Instreet: engellendi (reCAPTCHA, WebFetch dahil)"
incelenme: 2026-10-04
incelenen-sayfalar: [https://www.superstep.com.tr/erkek-ayakkabi/, https://www.superstep.com.tr/urun/adidas-x-superstep-samba-og-unisex-krem-spor-ayakkabi/ki8459-2/, https://www.sportive.com.tr/erkek-spor-ayakkabi/, https://www.sportive.com.tr/nike-court-vision-lo-erkek-siyah-sneaker-ayakkabi-ib2998-004-1/, https://www.sneaksup.com/erkek-ayakkabi-sneaker, https://www.korayspor.com/gunluk-erkek-spor-ayakkabilari/, https://www.lescon.com.tr/erkek-sneakers/]
etiketler: [rakip, tr-sneaker, cok-markali]
---

# Türkiye Sneaker Mağazaları

> [!summary] Özet
> KPT'nin doğrudan rakipleri olan altı çok markalı Türk mağazası. Ortak mekanikler şunlar: ücretsiz kargo eşiği (1.500–5.000 TL), mağazadan teslim, vade farksız taksit ve uygulamaya özel kupon (APP15). Sneaks Up çekiliş, lansman takvimi ve token tabanlı sadakat programıyla öne çıkıyor. Superstep ve Sportive ise beden önerisi, "Son 10 Günün En Düşük Fiyatı" etiketi ve sepette ek indirim gösteriyor. KPT için en değerli ders: güven bilgisini (kargo eşiği, iade süresi, taksit) ürün sayfasında butonun hemen yanına koymak ve beden ızgarasında kalıp tavsiyesi vermek.

> [!warning] Erişim ve yöntem
> Superstep ve Sportive (Akinon / Next.js) kendi JS dosyalarına 500 döndüğü için "Application error" ile çöküyor. Bu yüzden sayfalar JS kapalı alındı ve sunucu HTML'i ile RSC verisinden okundu; bazı görseller ve menü yüklenmedi. Sneaks Up, Korayspor ve Lescon iki denemede de Cloudflare 403 verdi. Bu üç sitenin metni WebFetch özetleyicisinden geliyor: ekran görüntüsü yok ve özet kayıplı olabilir. Instreet her denemede reCAPTCHA gösterdi. Hiçbir engel atlatılmaya çalışılmadı.

## Karşılaştırma tablosu (mekanikler)

| Site | Ücretsiz kargo | İade | Mağazadan teslim | Taksit | Çekiliş / lansman | Uygulama kuponu |
|---|---|---|---|---|---|---|
| Sneaks Up | 5.000 TL üzeri (WebFetch) | 30 gün, kargo veya mağaza (SSS) | Var, ücretsiz; 2–5 iş günü, 7 gün içinde alınmalı | 9 taksite kadar (Bonus, World, Maximum, CardFinans, Paraf, Axess, Advantage) | **Raffle + "LANSMAN TAKVİMİ \| DROP & RELEASE"** | — |
| Superstep | Meta açıklamada "ücretsiz kargo" var, eşik görülmedi | "Kolay İade / Yurtiçi Kargo ile ücretsiz iade." | Durum metni var ("Teslim Almaya Hazır") | "Bonus kartlara özel vade farksız taksit seçenekleri!" | Geri sayımlı lansman banner bileşeni var (şu an test içeriği) | "APP15" (%15) |
| Sportive | "3.500 TL Üzerine Ücretsiz Kargo" | "Kolay İade" | **"Mağazadan Ücretsiz Teslimat"**, ertesi gün | "Vade Farksız Taksit Seçenekleri", Maximum ile 6 taksit | Yok | "APP15" (%15) |
| Korayspor | "1500 TL ve üzeri alişverişlerde ücretsiz kargo" (yazım hatası sitede) | Üst şeritte 14 gün, iade sayfasında "14 iş günü"; DHL kodu 4434 | Görülmedi | Görülmedi | Yok | Uygulama var |
| Lescon | "3500 TL ve Üzeri Alışverişlerde Ücretsiz Kargo!📦" | 14 gün; mağazada değişim 30 gün | "Mağazadan teslim alma" | Vade farklı; World ile 5.000 TL'ye 2, 10.000 TL'ye 3 taksit | Yok | Var |
| Instreet | incelenemedi | incelenemedi | incelenemedi | incelenemedi | incelenemedi | Play Store: 5 Mn+ indirme, 4,7 puan |

## Superstep (erişim: kısmi)

**Görsel dil:** Montserrat. Metin #1D1D1B, ikincil metin #4A4A49, indirim kırmızısı #CF152D / #E30613, kart zemini #F4F4F4. Köşeler: hap 9999px, CTA 30px, beden kutusu 4px. Gövde 14px, fiyat 18px kalın, H1 28px.

**Header:** #1D1D1B zemin üzerinde 12px beyaz dönen üst şerit: "Siparişin 2-5 iş günü içerisinde kargoya verilecektir.", "APP'e Özel Seçili Ürünlerde %15 İndirim! Kupon Kodu: APP15", "Bonus kartlara özel vade farksız taksit seçenekleri!". Mega menüde İNDİRİM sekmesi #cf152d renginde.

**Ana sayfa (RSC sırası):** indirim video bandı (1296×214 / mobil 343×200) → 3 sütunlu hero (mobilde 492px, 10px köşeli kaydırıcı; "Yeni Sezon Tarzını Yansıt / UGG", "Retro Tarz, Modern Dokunuş / adidas", beyaz "Keşfet" butonu) → kampanya bantları ("SEÇİLİ ÜRÜNLERDE %25 İNDİRİME EK SEPETTE %10 İNDİRİM") → "Kategorilere Göz At" → "Kombinlerle Tarzını Yarat" → "Sezonun Öne Çıkan Modelleri" → geri sayımlı lansman banner'ı ("Kalan Süre: Gün / Saat / Dakika / Saniye") → güven rozetleri ("Kolay İade", "Teslimat", "Güvenli Ödeme"). Banner görsellerinin köşesinde **"Yapay zeka ile oluşturulmuştur"** etiketi var.

**PLP** (/erkek-ayakkabi/):
- Üstte #F9F9F9 giriş kutusu: "Favori Erkek Ayakkabıları ile Adımlarına Hava Kat" + 3 altı çizili hızlı link. Ardından H1 "Erkek AYAKKABI (2137)", "Filtrele" (çekmece) ve "Sırala: Önerilenler".
- Hap şeklinde model çipleri: "New Balance 9060", "adidas gazelle", "Puma Palermo" (48px yükseklik, 1px çerçeve).
- 4 sütun ızgara. Kartta kalp, 32px siyah daire "+" (hızlı ekleme), renk sayısı ("6"), marka (16px kalın), ad (14px), puan ("5.0 ★★★★★ (1)"), fiyat (18px kalın) var.
- İndirim gösterimi: kırmızı "▼%40" → üstü çizili "7.399 TL" → "4.439 TL", altında kırmızı **"↘ Son 10 Günün En Düşük Fiyatı"**. Varyant: kırmızı fiyat ve **"↘ Avantajlı Fiyat"**. Sayfa başına 48 veya 96 ürün seçilebiliyor.

![[superstep-plp-kart.jpg]]
*Superstep PLP kartları: "Avantajlı Fiyat" ve "%40 · üstü çizili · Son 10 Günün En Düşük Fiyatı" etiketleri (görseller JS'siz yüklenmedi).*

**PDP** (adidas x SuperStep Samba OG, 6.499 TL):
- Galeri: solda dikey küçük görsel şeridi (oklu), sağda #F4F4F4 zeminli tek büyük görsel.
- Sağ sütun sırasıyla: breadcrumb, marka (kalın), ad, fiyat (18px kalın), paylaş ve favori ikonları, "RENK(1) • Krem" küçük görsel swatch, sağda "MODEL NUMARASI : KI8459".
- Ardından "BEDEN" başlığı, sağında "Beden Tablosu" linki. Altında kalıp tavsiyesi: **"Yarım beden büyük almanı tavsiye ederiz."**
- Beden ızgarası 6 sütunlu. Her kutu 72×40px, 1px #E8E8E8 çerçeveli, 4px köşeli. Bedenler 36–45 arası, yarım numaralar dahil ("36,5", "42,5").
- Stok etiketleri sözlükte "Tükendi" ve "Son 1 Ürün" olarak geçiyor. Stokta olmayan beden için "Gelince Haber Ver" (e-posta) var.
- CTA "Sepete Ekle": 190×48px, #1D1D1B zemin, beyaz metin, 30px köşe.
- Açıklama: "Neden … Tercih Etmelisin?", "Sana Sağlayacağı Avantajlar" (kırmızı noktalı liste), "Ürün Özellikleri", "Kombin Önerileri", "Bakım Önerileri". Çapraz satış: "Bunları da Beğenebilirsin" (ilk kart editoryal: "adidas Samba / Keşfet").
- Mobilde kırmızı **"SUPERSTEP ÖZEL"** rozeti ve **sabit alt çubuk** var (solda fiyat, sağda "Sepete Ekle").
- Sözlükte görülen diğer özellikler: "Mağazada bul", "Sanal Deneme Kabini" (AI), "TAKSİT SEÇENEKLERİ" tablosu, "Ürün sepetine eklendi / Sepete Git / Alışverişe Devam Et" çekmecesi, ücretsiz kargo ilerleme metni ("… Daha eklersen Kargo Bedava!"), "Misafir Olarak Ödeme".

![[superstep-pdp.jpg]]
*Superstep PDP: kalıp tavsiyesi, 6 sütunlu yarım numaralı beden ızgarası, 48px hap "Sepete Ekle".*

![[superstep-pdp-mobil.jpg]]
*Mobil PDP: "SUPERSTEP ÖZEL" rozeti ve fiyat ile "Sepete Ekle" içeren sabit alt çubuk.*

## Sportive (erişim: kısmi)

- **Görsel dil:** Poppins font. Ana renk lacivert #243746, logodaki "V" harfinde lime vurgu. İskelet zemin #F6F7F8. PDP bilgi kartı 24px köşeli (`rounded-3xl`). İskeletteki CTA **eğik paralelkenar** şeklinde (marka imzası).
- **Header:** logo; geniş hap arama kutusu ("Ürün veya kategori arayın"); ikonlar sırasıyla bildirim zili, favori, hesap, sepet. Menü (büyük harf): SPORLAR, KADIN, ERKEK, ÇOCUK, MARKALAR, KOLEKSİYONLAR, İNDİRİM, TAKIM SPORLARI. Mega menüde "Koşu Rehberi", "Krampon Rehberi", "Bra Rehberi" ve "Yüzücü Rehberi" var.
- **Ana sayfa (RSC sırası):** video hero kaydırıcı (başlık 48px / mobil 32px; "PUMA / Suede Daima Bir Klasik / Alışverişe Başla") → 26 markalı daire logo şeridi → Kadın / Erkek / Çocuk 3'lü tam genişlik görseller → 3'lü kampanya ızgarası (oran 1,28 / mobil 0,67, 6px boşluk; gradyan üzerine 25px başlık + 18px alt metin + 40px beyaz hap "KEŞFET"; "APP'e Özel %15 İndirim", "Seçili ürünlerde 3 al 2 öde") → spor kategorileri → uygulama QR bloğu → değer şeridi "Mağazadan Ücretsiz Teslimat · 3.500 TL Üzerine Ücretsiz Kargo · Vade Farksız Taksit Seçenekleri".
- **PLP:** 1162 ürün, sayfa başına 48. 20 çoklu seçimli filtre var ("Renkler" swatch). Aralarında **teknik filtreler** de var: Ayak Formu, Bilek Desteği, Yastıklama Seviyesi, Zemin Tutuşu, Parmak Hareket Alanı. Çekmecede "Seçili Filtreler", "Tümünü Temizle", "Sonuçları Göster" bulunuyor.
- **PDP:** Stokta olmayan beden (41) listede kalıyor ama seçilemiyor. Etiketler: "Beden Seçiniz", "Son Ürün", "STOK GELİNCE HABER VER", "Mağazada Bul". Fiyat örneği: 4.299 TL → 3.439,90 TL, ayrıca **"Online Özel"** sepet teklifiyle 3.267,91 TL. "Çok Seveceksin Çünkü" bloğu 5 fayda maddesinden oluşuyor.
- **Mağazadan teslim:** "Pazar günleri hariç siparişini takip eden gün seçtiğin mağazadan teslim almaya gelebilirsin". Tutarsızlık: ödeme sözlüğünde eski "400 TL Üzerine Ücretsiz Kargo" metni kalmış.

## Sneaks Up (erişim: tarayıcı engellendi, metin WebFetch)

- **Menü ve banner:** YENİLER, ÇOK SATANLAR, "İNDİRİM sale up", "STİL ÖNERİLERİ shop the look". Bannerlar: "MEET ME IN THE CITY", "SALE UP – Kampanya 1 - 15 Ekim tarihleri arasında geçerlidir."
- **Lansman takvimi:** Ana sayfada **"LANSMAN TAKVİMİ | DROP & RELEASE"** bölümü var. Kartlarda ay etiketi ("Ocak 2026"), durum ("Satışta", "Tükendi") ve buton ("Ürüne Git" / "Gelince Haber Ver") bulunuyor (WebFetch).
- **Raffle (SSS):**
  - "her ayakkabı numarası için ayrı çekiliş", stok sayısı kadar kazanan.
  - "Her ürün için tek katılım hakkı"; birden fazla beden girilirse tüm katılımlar geçersiz sayılıyor.
  - Ürün kimlik ibrazıyla mağazadan ya da kimliği e-postayla gönderip online teslim alınıyor.
  - Tarihler site ve Instagram'dan duyuruluyor.
- **SNEAKS UP FRIENDS:**
  - 3 seviye: Friend, Best Friend, BFF.
  - Kazanım: harcamanın %2'si token; Click & Collect +40 token, ürün değerlendirmesi +30 token. PDP'de kazanılacak token gösteriliyor: "148 Token" (7.399 TL ürün).
  - Ayrıcalıklar: tüm siparişlerde ücretsiz kargo, **raffle'a öncelikli katılım, lansman ön siparişi**, yılda 1 ücretsiz sneaker bakımı, mağazada kişiselleştirme.
- **PLP:** "1449 ürün listeleniyor", fiyat formatı "7.399,00 TL", "Yeni" rozeti, "DAHA FAZLA GÖSTER" butonu. Mağazalar sayfasında 9 öne çıkan mağaza (Kanyon, Nişantaşı, Galata Port vb.) ve il/ilçe filtresi var. Kapıda ödeme yok.

## Korayspor (erişim: tarayıcı engellendi, metin WebFetch)

- **Üst şerit:** "Güvenle alışveriş yapın. 14 gün içinde kullanılmayan ürünleri ücretsiz iade edebilirsiniz."
- **Değer blokları:** "Kargoyu düşünmeyin" / "Ücretsiz iade – Şimdi çok kolay" / "Kafanızda soru işareti kalmasın – Online Destek'ten bize sorun".
- **PLP:** 3639 ürün, "Load More" ile yükleme. Kart rozetleri: "Yeni", "Ücretsiz Kargo", "-%40", "Fırsat Köşesi", "Premium Koleksiyon" (210 ürünlük seçki).

## Lescon (erişim: tarayıcı engellendi, metin WebFetch)

- **Üst şeritler:** "Yeni Sezonda 2.Ürüne %30 - 3.Ürüne %50 İndirim!⚡", "Seçili Ürünlerde Aynı Gün Kargo 🚚" (koşul: "saat 12:00'a kadar verilen siparişlerde").
- **PLP:** filtreler KATEGORİLER, Beden, Fiyat, Renk, Cinsiyet. Sıralama: En Yeni / Fiyata Göre Artan-Azalan / İndirime Göre Artan-Azalan / Çok Satan. Kart rozetleri: "Yeni", "2. Ürüne %30", "Aynı Gün Kargo". İndirim örneği: "1.999,99 TL", üstü çizili "2.399,99 TL", "%17".

## Instreet (erişim: engellendi)

Ana sayfa normal ziyaretçiye bile "Tarayıcınız kontrol ediliyor - reCAPTCHA" sayfası ve resim seçme testi ("Bisiklet içeren tüm kareleri seçin") gösteriyor. Bu bir dönüşüm kaybı riski. Tek ikincil veri Google Play'den geliyor: uygulama "Instreet", geliştirici "Flo Mağazacılık ve Pazarlama A.Ş.", 4,7 puan, 11,8 B yorum, 5 Mn+ indirme. Başka bölümler incelenemedi (WebSearch kotası doldu, şikâyet sitesi 403 verdi).

## Güven ve ikna teknikleri

| Teknik | Nerede | İlke | KPT'ye uyarlanabilir mi? |
|---|---|---|---|
| "Son 10 Günün En Düşük Fiyatı" | Superstep PLP | Referans fiyat / çapa, güven | Evet, fiyat geçmişi tutulursa (Omnibus tarzı) |
| "Yarım beden büyük almanı tavsiye ederiz." | Superstep PDP | Belirsizliği azaltma | Evet, model bazlı kalıp notu |
| Raffle + lansman takvimi | Sneaks Up | Kıtlık, adalet | İleride, sınırlı modellerde |
| PDP'de "148 Token" | Sneaks Up | Kazanç çerçevesi | Sadakat programı gelirse |
| Ücretsiz kargo ilerleme metni | Superstep sepet | Hedef gradyanı | Evet, hemen |
| "SUPERSTEP ÖZEL" rozeti | Superstep | Ayrıcalık | "KPT'de" seçkisi rozeti |

## KPT için çıkarımlar

**Uygula:**
1. PDP'de "Sepete Ekle"nin hemen altına 3 satırlık bir güven bloğu koy, metni şöyle olsun: "X TL üzeri ücretsiz kargo · 14 gün ücretsiz iade · Vade farksız 3 taksit". Rakiplerin hepsinde bu üçlü var; eşik olarak 3.500 TL piyasa ortalamasına yakın.
2. Beden ızgarasını şöyle kur: 6 sütun, 72×40px kutu, 1px #E8E8E8 çerçeve, 4px köşe, yarım numaralar ("42,5"). Stokta olmayan bedenleri gizleme; üstü çizili göster ve "Gelince Haber Ver" sun. Izgaranın üstüne model bazlı kalıp notu ekle ("Yarım beden büyük almanı tavsiye ederiz.").
3. Mobil PDP'ye sabit alt çubuk ekle: solda fiyat (18px kalın), sağda 48px hap "Sepete Ekle" (KPT'de bordo #741E32).
4. İndirim gösterimi şu sırayla olsun: yüzde → üstü çizili eski fiyat → yeni fiyat. Altına küçük açıklayıcı etiket ekle ("Son 30 Günün En Düşük Fiyatı" gibi, ancak yalnızca veri gerçekse).
5. PLP'nin üstüne hap şeklinde model çipleri koy ("New Balance 9060", "Samba", "Palermo"). Kategori filtresini çoklu seçimli çekmeceye çevir ve "Seçili Filtreler", "Tümünü Temizle", "Sonuçları Göster" ekle.
6. Sepete eklemede çekmece aç ("Ürün sepetine eklendi / Sepete Git / Alışverişe Devam Et"). Çekmecede ücretsiz kargo ilerleme metni olsun: "Sepetine X TL daha eklersen Kargo Bedava!".
7. AI ile üretilen hero görseline küçük bir "Yapay zeka ile oluşturulmuştur" etiketi ekle (Superstep deseni).

**Uyarla:**
- Sportive'deki "Çok Seveceksin Çünkü" 5 maddelik fayda bloğu, KPT'nin boş açıklama sorununa şablon olabilir.
- Sneaks Up'taki "LANSMAN TAKVİMİ" kart yapısı (ay etiketi, durum, "Gelince Haber Ver") "Yakında gelecekler" bölümü olarak kullanılabilir.
- Erkek / Kadın / Çocuk 3'lü tam genişlik görsel giriş (Sportive) eksik cinsiyet menüsünü tamamlar.

**Kaçın:** ana sayfada resimli CAPTCHA (Instreet); çelişen iade ve kargo metinleri (Korayspor'da "14 gün" ve "14 iş günü", Sportive'de "400 TL" ve "3.500 TL"); JS hatasında tüm sayfanın çökmesi (Superstep, Sportive); emoji dolu üst şerit metinleri (Lescon).

İlgili: [[Ürün Sayfası]], [[Beden ve Kalıp]], [[Güven Sinyalleri]], [[Sepet ve Ödeme]], [[Kategori Sayfası ve Filtreler]], [[Mobil Deneyim]], [[Türkiye E-ticaret Pazarı]], [[KPT Store Denetimi]]

## Kaynaklar
- https://www.superstep.com.tr/ , /erkek-ayakkabi/ , /urun/adidas-x-superstep-samba-og-unisex-krem-spor-ayakkabi/ki8459-2/ (sunucu HTML'i, 2026-10-04)
- https://www.sportive.com.tr/ , /erkek-spor-ayakkabi/ , /nike-court-vision-lo-erkek-siyah-sneaker-ayakkabi-ib2998-004-1/ (sunucu HTML'i, 2026-10-04)
- https://www.sneaksup.com/ , /erkek-ayakkabi-sneaker , /puma-speedcat-dress-up-406998-03-sneaker-p-256609 , /sss , /friends-landing , /magazalar (WebFetch, 2026-10-04)
- https://www.korayspor.com/ , /gunluk-erkek-spor-ayakkabilari/ , /new-balance-ayakkabi-gunluk-1906-gri-modeli-koleksiyonu-m1906reh/ , /iade/ , /sss/ , /premium-koleksiyon/ (WebFetch, 2026-10-04)
- https://www.lescon.com.tr/ , /erkek-sneakers/ , /beyaz-riva-2-erkek-sneaker-ayakkabi/ , /sikca-sorulan-sorular/ (WebFetch, 2026-10-04)
- https://play.google.com/store/search?q=instreet&c=apps&hl=tr&gl=TR (2026-10-04)
