# Deploy this portfolio to GitHub Pages

The site is a single static page (`index.html`) + your résumé PDF. For a **user site** at
`https://rahul1996pp.github.io`, the repo must be named exactly `rahul1996pp.github.io`.

## Option A — GitHub CLI (fastest)
```bash
cd portfolio
git init -b main
git add index.html Rahul_P_Resume.pdf
git commit -m "Portfolio site"
gh repo create rahul1996pp.github.io --public --source=. --push
```
GitHub auto-enables Pages for `*.github.io` repos. Live in ~1 minute at **https://rahul1996pp.github.io**.

## Option B — Web UI
1. Create a new **public** repo on github.com named **`rahul1996pp.github.io`**.
2. Upload `index.html` and `Rahul_P_Resume.pdf` to the repo root.
3. Settings → Pages → confirm Source = `main` / root.
4. Visit **https://rahul1996pp.github.io**.

## Updating later
Edit `index.html`, then:
```bash
git add -A && git commit -m "Update" && git push
```

## Notes
- **Custom domain:** add it under Settings → Pages, then a CNAME DNS record. Optional.
- **Fonts:** loaded from Google Fonts (works on Pages; needs internet on first load).
- **Certificates:** edit the `.cert` cards in the Certificates section — duplicate one block per certificate.
