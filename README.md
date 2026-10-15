# PDF Düzenleyici

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
