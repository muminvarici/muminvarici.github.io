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
| `index.html` | Portfolio site (single file, no dependencies) |
| `cv.md` | ATS-compatible CV in Markdown (excluded from the published site) |
| `robots.txt` / `sitemap.xml` | Crawler rules and sitemap for search engines |
| `favicon.svg` / `apple-touch-icon.png` | Site icons |
| `og-image.png` | 1200×630 social share preview (LinkedIn, X, WhatsApp…) |
| `404.html` | Custom not-found page (`noindex`) |
| `_config.yml` | GitHub Pages build config (excludes repo docs from the site) |

## SEO & Google Search Console

The page ships with a canonical URL, Open Graph / Twitter meta tags and
`schema.org` JSON-LD (`WebSite` + `ProfilePage` + `Person`).

To register the site in Google Search Console:

1. Open https://search.google.com/search-console → **Add property** → **URL prefix** →
   `https://muminvarici.github.io/` (a *Domain* property is not possible on `github.io`).
2. Choose **HTML tag** verification, copy the `content` value, and paste it into the
   commented-out `google-site-verification` meta tag in `index.html`. Push and wait for Pages to deploy.
3. Click **Verify**.
4. **Sitemaps** → submit `sitemap.xml`.
5. **URL inspection** → `https://muminvarici.github.io/` → **Request indexing**.

When content changes, update `<lastmod>` in `sitemap.xml`.
