# Pratik Byathnal — Portfolio

A single-page, Apple-inspired personal portfolio. No build step, no dependencies — just static files.

## Files
- `index.html` — the entire site (HTML, CSS, JS inlined)
- `Pratik_Byathnal_Resume.pdf` — résumé download
- `SOC_Alert_Prioritization.pdf`, `Survey_Secure_Boot.pdf` — research papers
- `.nojekyll` — tells GitHub Pages to serve files as-is

## Deploy to GitHub Pages

### Option A — repo named `thecoderpb.github.io` (lives at the root domain)
1. Create a new repo named exactly **`thecoderpb.github.io`**.
2. Copy the contents of this folder into the repo root, then:
   ```bash
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/thecoderpb/thecoderpb.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch → `main` / `root`** → Save.
4. Live at **https://thecoderpb.github.io** within a minute or two.

### Option B — any repo name (e.g. `portfolio`)
Same as above but the site lives at `https://thecoderpb.github.io/<repo-name>/`. Enable Pages the same way (Settings → Pages → branch `main`, folder `/root`).

## Update later
- Swap the résumé by replacing `Pratik_Byathnal_Resume.pdf` (keep the filename).
- Edit text/sections directly in `index.html`.
- Add a profile photo: replace the `PB` `<div class="avatar">` with `<img src="me.jpg" class="avatar" alt="Pratik Byathnal">`.

## Customize the accent
Colors live in the `:root` block at the top of `index.html` — change `--accent` and `--accent-2` to restyle the whole site.
