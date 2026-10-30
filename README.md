# PDF Düzenleyici

## 2.2 (30.10.2026) — Satır / Kelime düzenleme seçimi
- Sağ panelin üstünde (Metni düzenle aracı) **Düzenleme: ▤ Satır · ▭ Kelime** düğmeleri; seçim hatırlanır.
  **Satır:** satırın tamamı tek kutuda. **Kelime:** yalnız dokunulan kelime (sürüklenirse kelime aralığı) düzenlenir, diğerleri olduğu gibi kalır — normal ve taranmış PDF'te. Normal PDF'te yazı tipi/punto/taban çizgisi PDF'in kendisinden; taranmışta görünen harflerden. Yeni yazı yandaki kelimeye taşarsa uyarır.

## 2.1 (30.10.2026) — Taranmış belgede yine satırın tamamı
- Taranmış (OCR katmanlı) sayfada da tıklanan **görünen satırın tamamı** düzenlenir (kelime kelime değil). Yazı tipi/punto/kalınlık görünen harflerden bulunmaya devam eder; OCR kelime sayısı görünen kelimelerle aynıysa kalın kısımlar korunur. Satır metni gizli OCR katmanından gelir, hatalı harfler düzeltilir. Aynı görsel satıra ikinci tıklama yeni düzenleme açmaz.

## 2.0 (30.10.2026) — Yazı tipi görünen harflerden; taranmış belgede kelime düzenleme
- **Yazı tipi, punto, kalınlık görünen harflerden bulunur:** satırın çizgi kontrastı (Times'ta ince yatay / kalın dikey çizgiler), gövde kalınlığı ve x-yüksekliği Times / Arial / Courier × düz / kalın örnekleriyle karşılaştırılır. Taranmış belgelerdeki gizli OCR katmanı çoğu zaman "Arial" adı taşır; artık bu ada bakılmaz. Normal PDF'te yazı tipi adı belirsizse de aynı yöntem kullanılır.
- **Taranmış (OCR katmanlı) sayfa:** görünen yazı resimdir, altındaki OCR metni hatalı olabilir (İlçemiz → Ilgemiz). Bu yüzden satırın tamamı değil, **yalnız dokunulan kelime** (sürüklenirse kelime aralığı) düzenlenir; diğer kelimeler orijinal resim olarak kalır. Kelime sınırları resimdeki boşluklardan, satır yüksekliği görünen satırdan bulunur; örtü satırın tam yüksekliğinde ve kağıt dokusuyla.
- Yeni yazı yandaki kelimeye taşarsa uyarı verir (kelimeleri sürükleyerek birlikte seçin).

## 1.9 (30.10.2026) — Orijinal kağıt dokusu, kalınlık korunur, yeni üst çubuk
- Eski yazıyı örten kutu artık **düz renk değil, kağıdın kendisi**: bölge sayfadan yüksek çözünürlükte alınır, yazı silinip çevredeki kağıt tonu ve kumlamasıyla doldurulur (taranmış, renk tonu değişen belgelerde leke kalmaz). Zemin bölümünde "Orijinal kağıt dokusu" kutusu; renk seçilirse düz renge döner.
- Satırda kalın ve normal parçalar karışıksa (ör. "İlçemiz **Ardıç Mahallesi**, …") düzenlemede kalınlık korunur.
- Üst çubuk (Geri · İleri · Çizgiler · Önizleme · Ekle · Kaydet) alt araç çubuğuyla aynı görünümde: simge üstte, yazı altta; telefonda sığar.

## 1.8 (30.10.2026) — Kısmen kalın yazı
- Düzenlenen satırda **yalnız seçilen kelime(ler) kalın** olur: kelimeyi seçip sağ paneldeki **K** ya da **Ctrl+B**. Seçim yoksa K tüm satırı kalın yapar (eskisi gibi). PDF'e, önizlemeye ve tozlu yazıya aynen yansır.
- Açılış ekranındaki **Dosya seç** düğmesinde simge görünür, simge ve yazı ortalı.

## 1.7 (27.10.2026) — Metin düzenleme araçları, baskı önizleme, BelgeNet uyumu
- Düzenlenen/eklenen metinde **tutamaklar** (köşeler orantılı büyütür-küçültür, ✥ taşır), **yön tuşlarıyla taşıma** (0,5 pt; Shift 5 pt; yazarken Alt+yön; panelde ◀▲▼▶).
- **Yoğunluk** sürgüsü (sola soluk/şeffaf, sağa koyu; PDF'e de yazılır) ve **taranmış (tozlu) yazı** seçeneği (toz miktarı ayarlanır; PDF'te görsel olarak).
- **Zemin rengi**: renk kutusu veya 💧 sayfadan seç. Eski yazıyı örten kutu **tablo çizgilerine binmez**; aynı satırdaki hücreler dikey çizgiden ayrılır; zemin rengi ince hücrede griye kaymaz.
- **Geri al / İleri al** yazılı düğmeler; Ctrl+Z / Ctrl+Y metin yazarken de çalışır. **Çizgiler** düğmesi düzenleme çerçevelerini gizler.
- **Baskı önizleme**: kaydedilecek PDF kağıt görünümünde; yalnız bu sayfa, yakınlaştırma, PDF olarak kaydet, Yazdır.
- Sağ panel açılır-kapanır **bölümler** (Yazı · Görünüm · Zemin · Çizgi · Konum · Seçili nesne · Sayfa), durum hatırlanır.
- Kaydedilen PDF **klasik xref** ile (nesne akışı yok) — BelgeNet önizlemesi için. Cloudflare Pages'te de çevrimdışı.

## 1.6 (23.10.2026) — Tam ekran düğmesi geri
- Kurulu uygulamada gizlenen tam ekran düğmesi yeniden görünür ve çalışır. Düğmeye basınca Chrome kendi "Tam ekrandan çıkmak için…" uyarısını bir kez gösterir (tarayıcı kuralı). Dokununca kendiliğinden tam ekran isteği gönderilmez.

## 1.5 (22.10.2026) — Kurulu uygulamada tam ekran düğmesi
- Ana ekrandan yüklenen uygulama baştan tam ekran açıldığı için tam ekran düğmesi gizlendi ve basılsa da tam ekran isteği gönderilmez. Önceden düğmeye basınca uyarı çıkıyor, sayfa yeniden diziliyor, yazılar kayboluyor / sayfa değişiyordu.

## 1.4 (22.10.2026) — Tam ekran uyarısı kesin çözüm
- Sayfanın kendiliğinden tam ekrana geçme istekleri (ilk dokunuşta, açılışta, dosya seçiciden dönünce) **tamamen kaldırıldı**; Chrome'un "Tam ekrandan çıkmak için…" uyarısı ekrana dokununca artık çıkmaz. Tam ekran isteği yalnız tam ekran düğmesine basınca gönderilir. Ana ekrandan yüklenen uygulama zaten tam ekran açılır.

## 1.3 (22.10.2026) — Açılışta tam ekran
- Ana ekrandan açılınca uygulama **doğrudan tam ekran** gelir (`manifest.webmanifest`: `"display": "fullscreen"`). Tarayıcı içinden tam ekran isteği gönderilmediği için Chrome'un "Tam ekrandan çıkmak için…" uyarısı da çıkmaz.
- Daha önce yüklenmiş simge eski ayarla açılabilir: simgeyi kaldırıp Chrome › ⋮ › **Uygulamayı yükle** ile yeniden yükle.

## 1.2 (22.10.2026) — Sessiz ekran
- **Tam ekran uyarısı:** Ana ekrandan açılan (kurulu, tam ekran) uygulamada içeriden tam ekran isteği gönderilmez → Chrome'un "Tam ekrandan çıkmak için yukarıdan sürükleyip…" uyarısı çıkmaz. Chrome sekmesinde tam ekrana her girişte bu uyarıyı tarayıcı kendisi gösterir; sayfa kapatamaz.
- **Kelimeye dokununca Google paneli:** Chrome'un "Dokunarak ara" paneli açılmasın diye sayfa (ve içindeki çerçeveler) dokunuşu kendisi karşılar. Uzun basıp seçme çalışır.
- Blok `/* SESSİZ EKRAN */` adıyla `index.html`'in başındadır; tüm uygulamalarda aynıdır.

PDF birleştirme, ayırma, sıkıştırma, sayfa döndürme/silme/çoğaltma, imza, filigran, parola, görselden PDF ve JPG/PNG çıkarma — telefonda, dosyalar cihazdan çıkmaz.

**Uygulamayı aç:** https://aaskinkk-cloud.github.io/pdf-duzenleyici/

Milli Emlak uygulamasının **PDF Düzenleyici** modülü de buradan gelir: Milli Emlak açılışta bu sayfanın sürümünü (`sw.js`) okur, değişmişse yeni sürümü kendiliğinden indirir. Drive'a modül yüklemek gerekmez.

## Kurulum

Chrome'da adresi aç → menü → **Ana ekrana ekle**. İnternetsiz de çalışır.

## Gizlilik

Dosyalar yalnız cihazında işlenir; hiçbir sunucuya gönderilmez.

## Dosyalar

| Dosya | Açıklama |
|---|---|
| `index.html` | Uygulamanın tamamı (tek dosya) |
| `sw.js` | Çevrimdışı önbellek ve sürüm (`V=P+'…'` — Milli Emlak buradan okur) |
| `manifest.webmanifest`, `icon.svg` | Ana ekran simgesi ve uygulama bilgileri |

## Sürüm

**1.1** — Metin düzenleme Okur'un PDF metin motoruyla: satıra **dokununca** (tıklayınca) düzenleme açılır (telefonda klavye ve odak daha güvenilir); yazı tipi, punto, kalın/italik (",B"/"-Bold" gibi adlar dahil), yazı ve zemin rengi otomatik algılanır; **hiç değiştirilmeyen satır kaydedilmez** — dokunulan ama değiştirilmeyen satır özgün hâliyle kalır, yerine benzer yazı tipiyle yeniden yazılmaz; ekrandaki satır aralığı kaydedilen PDF ile aynı.  
1.0 — GitHub'a taşındı (Milli Emlak 124 ile birlikte).
