# İnsan Kaynakları Standartları — Ders Notları

BSI ve ISO/TC 260 İnsan Sermayesi Yönetimi ve Gelişimi (HCMD) çerçevesine dayalı
yüksek lisans dersinin izlencesi ve haftalık ders notlarının statik web sürümü.

## İçerik

| Dosya | İçerik |
|---|---|
| `index.html` | Ders izlencesi (syllabus) + tüm haftalara bağlantı veren giriş sayfası |
| `hafta-01.html` … `hafta-14.html` | Haftalık ders notları; `hafta-07.html` ara değerlendirme haftasıdır (vize kapsamı, 1.–6. hafta tekrar rehberi ve proje ara raporu yönergesi) |
| `donem-projesi.html` | Dönem projesi örneği — Marmara Lojistik A.Ş. (ISO 30414:2025 uyumlu HCRD taslağı) |
| `assets/style.css` | Tek stil dosyası |
| `.nojekyll` | GitHub Pages'in dosyaları olduğu gibi yayımlaması için |

Sayfalar birbirine üç yoldan bağlıdır: üst çubuktaki **Haftalar** menüsü, giriş
sayfasındaki hafta kartları ve her sayfanın altındaki **önceki / sonraki** gezinimi.
Her ders notunun solunda o sayfaya ait içindekiler listesi vardır (mobilde açılır-kapanır).

## GitHub Pages'te yayımlama

1. GitHub'da yeni bir depo açın (ör. `ik-standartlari`).
2. Bu klasördeki tüm dosyaları deponun köküne yükleyin:

   ```bash
   git init
   git add .
   git commit -m "İK Standartları ders notları"
   git branch -M main
   git remote add origin https://github.com/<kullanici>/<depo>.git
   git push -u origin main
   ```

3. Depoda **Settings → Pages** yolunu izleyin; **Source** olarak `Deploy from a branch`,
   **Branch** olarak `main` ve klasör olarak `/ (root)` seçin.
4. Birkaç dakika içinde site `https://<kullanici>.github.io/<depo>/` adresinde yayına girer.

Alt klasörde yayımlamak isterseniz (ör. `docs/`), dosyaları `docs/` içine koyup
Pages ayarında klasör olarak `/docs` seçmeniz yeterlidir; tüm bağlantılar görelidir.

## Notlar

- Yazı tipleri (Public Sans, Inter) Google Fonts'tan çekilir; çevrimdışı kullanımda
  sistem yazı tiplerine düşer.
- Sayfalar yazdırmaya uygundur (gezinim öğeleri baskıda gizlenir).
- ISO ve BSI standart metinleri telife tabidir; burada yalnızca öğretim amaçlı
  kavramsal çerçeve ve özetler yer alır.
