# muminvarici.github.io

Personal portfolio site for Mümin Kadir Varıcı — Software Architect.

## Deploy to GitHub Pages

1. Create a new repository on GitHub named exactly: `muminvarici.github.io`
2. Push this project to that repo:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/muminvarici/muminvarici.github.io.git
   git push -u origin main
   ```
3. Go to **Settings → Pages → Source**: set branch to `main`, folder to `/ (root)` → Save
4. Your site will be live at **https://muminvarici.github.io** within a few minutes.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Portfolio site – English (default, `x-default`) |
| `tr/index.html` | Portfolio site – Turkish |
| `assets/css/site.css`, `assets/js/site.js` | Shared styles and scripts used by both language pages |
| `cv.md` | ATS-compatible CV in Markdown (excluded from the published site) |
| `robots.txt` / `sitemap.xml` | Crawler rules and sitemap for search engines |
| `favicon.svg` / `apple-touch-icon.png` | Site icons |
| `og-image.png` | 1200×630 social share preview (LinkedIn, X, WhatsApp…) |
| `404.html` | Custom not-found page (`noindex`) |
| `googleff89007e00027af1.html` | Google Search Console ownership verification – do not delete |
| `_config.yml` | GitHub Pages build config (excludes repo docs from the site) |

## SEO & Google Search Console

The page ships with a canonical URL, Open Graph / Twitter meta tags and
`schema.org` JSON-LD (`WebSite` + `ProfilePage` + `Person`).

Both language pages link to each other with `hreflang` (also declared in `sitemap.xml`).
Page-specific text – including the typewriter phrases (`data-phrases`) – lives in each HTML file;
layout and behaviour live in `assets/`. When you change content, update **both** pages.

Google Search Console (URL-prefix property `https://muminvarici.github.io/`) is verified
with the HTML file method (`googleff89007e00027af1.html`). After deploy:

1. Search Console → **Verify**.
2. **Sitemaps** → submit `sitemap.xml`.
3. **URL inspection** → request indexing for `/` and `/tr/`.

When content changes, update `<lastmod>` in `sitemap.xml`.
