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
| `cv.md` | ATS-compatible CV in Markdown |
