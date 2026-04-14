# Personal site (GitHub Pages)

Static site: open `index.html` locally or deploy this folder to GitHub Pages.

## Deploy

1. Create a new repository on GitHub (e.g. `yourusername.github.io` for a user site, or any name for `https://yourusername.github.io/repo-name/`).
2. From this folder, run:

```bash
git init
git add .
git commit -m "Add personal site"
git branch -M main
git remote add origin https://github.com/YOUR_USER/YOUR_REPO.git
git push -u origin main
```

3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch **main**, folder **/ (root)**.
4. After a minute, the site URL appears on the Pages settings page.

Optional: add PDF resumes under `assets/` and link them from `index.html`.
