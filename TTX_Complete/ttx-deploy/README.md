# Think Tank X — Startup Risk Framework

A complete, self-contained risk intelligence platform for startup investors and founders.

**Live platform:** one HTML file, no backend, no dependencies, works offline.

---

## What's inside

| Tab | Feature |
|---|---|
| Home | Landing page, methodology explainer, demo loader |
| Calculator | 22-question risk assessment, dual investor/startup mode |
| Score Card | 1200×630 PNG for LinkedIn and pitch decks |
| Compare | Side-by-side portfolio comparison with radar overlay |
| Benchmark | 7 sectors × 3 stages with source notes |
| Term Sheet | Risk-adjusted deal terms, conditions, tranches |
| History | localStorage persistence, trend chart, session management |

---

## Deploy in 2 minutes

### Option A — Netlify (recommended, free)

1. Go to [netlify.com](https://netlify.com) and sign up / log in
2. Click **"Add new site"** → **"Deploy manually"**
3. Drag the entire `ttx-deploy` folder onto the upload area
4. Done — Netlify gives you a live URL instantly (e.g. `amazing-name-123.netlify.app`)
5. Optional: go to **Site settings → Domain** to set a custom domain

### Option B — Vercel (free)

1. Go to [vercel.com](https://vercel.com) and sign up / log in
2. Click **"Add New Project"** → **"Upload"**
3. Upload the `ttx-deploy` folder
4. Click **Deploy**
5. Live at `your-project.vercel.app` in ~30 seconds

### Option C — GitHub Pages (free)

1. Create a new GitHub repository (public or private)
2. Upload all files from this folder to the repository root
3. Go to **Settings → Pages**
4. Set source to **"Deploy from branch"** → `main` → `/ (root)`
5. Save — GitHub publishes to `yourusername.github.io/repo-name`

### Option D — Cloudflare Pages (free, fastest CDN)

1. Go to [pages.cloudflare.com](https://pages.cloudflare.com)
2. Click **"Create a project"** → **"Direct Upload"**
3. Upload the `ttx-deploy` folder
4. Live at `your-project.pages.dev`

---

## Custom domain (any provider)

After deploying, point your domain's DNS to the hosting provider:

- **Netlify:** Add a CNAME record pointing to `your-site.netlify.app`
- **Vercel:** Add CNAME pointing to `cname.vercel-dns.com`
- **GitHub Pages:** Add CNAME pointing to `yourusername.github.io`
- **Cloudflare Pages:** Managed automatically if domain is on Cloudflare

---

## Local use

Simply open `index.html` in any modern browser. No server required.

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

---

## File structure

```
ttx-deploy/
├── index.html        ← The entire platform (167KB)
├── netlify.toml      ← Netlify config
├── vercel.json       ← Vercel config
├── _headers          ← Cloudflare Pages / Netlify headers
├── .gitignore        ← Git ignore file
└── README.md         ← This file
```

---

## Notes

- **No backend required** — all data stored in browser localStorage
- **Works offline** — only the PNG export feature requires internet (html2canvas CDN), with a graceful fallback
- **No tracking, no analytics, no external calls** — fully private
- **Assessment history** persists in the browser's localStorage per device

---

## Think Tank X

> *Risk before reward.*

thinktankx.com
