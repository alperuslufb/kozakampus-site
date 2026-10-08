# kozakampus.com — açılış sayfası

Tek dosyalık statik site. Uygulama deposundan bağımsızdır.

## Yayın (GitHub Pages)

1. GitHub'da yeni, boş bir depo aç: `kozakampus-site` (public).
2. Bu klasörde:
   ```
   git init
   git add .
   git commit -m "Açılış sayfası"
   git branch -M main
   git remote add origin https://github.com/alperuslufb/kozakampus-site.git
   git push -u origin main
   ```
3. Depo → Settings → Pages → Source: **Deploy from a branch** → `main` / `/ (root)` → Save.
4. Aynı sayfada Custom domain `kozakampus.com` görünür (CNAME dosyasından). DNS yayılınca "Enforce HTTPS" işaretle.

## Turhost DNS

- `@` → A → `185.199.108.153`
- `@` → A → `185.199.109.153`
- `@` → A → `185.199.110.153`
- `@` → A → `185.199.111.153`
- `www` → CNAME → `alperuslufb.github.io`

Park sayfasına giden eski A / CNAME kayıtlarını sil.

## Düzenleme

Metinler ve stil `index.html` içinde. Fontlar yereldir (SIL OFL 1.1), dış istek yoktur. Her `git push` siteyi günceller.
