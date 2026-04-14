# Personal site (GitHub Pages)

Static site: open `index.html` locally or deploy this folder to GitHub Pages.

**Do not share GitHub passwords or tokens in chat.** Sign in on your own machine (browser or `gh auth login`).

## Deploy (GitHub CLI — recommended)

[GitHub CLI](https://cli.github.com/) (`gh`) should be available. From this folder:

```bash
cd /Users/khangmle/Downloads/Website
gh auth login
```

Choose GitHub.com → HTTPS → authenticate via browser (or your preferred method). Then create the repo and push (pick one):

**User site** (URL `https://YOUR_USERNAME.github.io/` — repo name must be `YOUR_USERNAME.github.io`):

```bash
gh repo create YOUR_USERNAME.github.io --public --source=. --remote=origin --push
```

**Project site** (URL `https://YOUR_USERNAME.github.io/REPO_NAME/`):

```bash
gh repo create REPO_NAME --public --source=. --remote=origin --push
```

Enable Pages: **Settings → Pages →** branch **main**, folder **/ (root)**. The site URL appears on that page after a short wait.

## Deploy (manual)

1. Create an empty repository on GitHub (website UI).
2. Add the remote and push:

```bash
git remote add origin https://github.com/YOUR_USER/YOUR_REPO.git
git push -u origin main
```

3. Enable Pages as above.

Optional: add PDF resumes under `assets/` and link them from `index.html`.
