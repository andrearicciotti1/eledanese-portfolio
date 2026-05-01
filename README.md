# Eleonora Danese — Portfolio

Static portfolio site. Plain HTML/CSS/JS. Hosted on GitHub Pages.

## Local preview

Just open `index.html` in a browser. No build step.

Or run a local server:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy on GitHub Pages

1. Create a new public repo on GitHub. Recommended names:
   - `eleonoradanese.github.io` — site lives at `https://eleonoradanese.github.io`
   - `portfolio` (or any name) — site lives at `https://<user>.github.io/portfolio/`
2. Push the contents of this folder to the repo:
   ```bash
   git remote add origin git@github.com:<USER>/<REPO>.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment**. Source: **Deploy from a branch**. Branch: `main` / root. Save.
4. Wait ~1 minute. The URL will appear at the top of the Pages settings page.

## Editing content

- Bio, credits, releases, links → `index.html`
- Visual style (colors, fonts, spacing) → `style.css`
- Reveal-on-scroll behavior → `script.js`
- Portrait image → `assets/portrait.jpg` (replace at any time, keep filename)

### Color tokens (in `style.css` `:root`)
- `--bg` — page background
- `--ink` / `--ink-soft` / `--ink-faint` — text shades
- `--accent` — gold accent (currently `#c9a35a`)

### Typography
Cormorant Garamond (serif) and Inter (sans), loaded from Google Fonts.

## Custom domain (optional)

If you buy a domain, add a `CNAME` file at the project root containing the bare domain (e.g. `eleonoradanese.com`), and point the domain's DNS at GitHub Pages.
