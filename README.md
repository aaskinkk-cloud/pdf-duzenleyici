# PDF Düzenleyici

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
