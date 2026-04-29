# Interval — Total Experience Design™

Editorial single-page site for Interval, a strategic advisory and design lab.
Static HTML/CSS/JS — designed for Netlify, but works on any static host.

## Structure

```
interval-site/
├── index.html              ← single-file site (HTML + embedded CSS + JS)
├── netlify.toml            ← build, security and cache headers
├── README.md
└── assets/
    ├── interval-logo-black.svg
    ├── interval-logo-white.svg
    ├── fonts/
    │   ├── Inter.woff               ← variable font (opsz + wght)
    │   └── Inter-Italic.woff        ← italic variable
    └── images/
        ├── sculpture-portal.png     ← hero
        ├── amphitheater.jpg         ← photo break 1
        ├── coastal-architecture.jpg ← photo break 2
        ├── architectural-model.jpg  ← "ambition and operation" pair
        ├── curved-monument.jpg      ← gallery: cultural districts
        └── cylinder-forms.jpg       ← gallery: hospitality
```

## Design system

- **Type:** Inter Variable (opsz + wght axes), self-hosted as WOFF.
- **Buttons / CTA:** light tint of Brick (`#F0D9C2`) with black text, 4 px radius.
- **Palette:** Black, Off-White (`#F9F9F3`), Beige (`#F2EDD8`), Mint (`#82FFC0`),
  Electric (`#3D2EB8`), Brick (`#C05000`), Mauve (`#C8B4DC`).

## Deploy to Netlify

### Option A — Drag & drop (fastest)
1. Sign in at https://app.netlify.com.
2. *Add new project → Deploy manually.*
3. Drag the entire `interval-site/` folder (or its zip) onto the upload area.
4. Rename the site under *Site settings → Change site name*.

### Option B — Git-connected (recommended for ongoing work)
1. Push this folder to a GitHub / GitLab / Bitbucket repository.
2. *Add new project → Import an existing project →* connect the repo.
3. `netlify.toml` handles publish dir and headers automatically.

### Custom domain
*Domain management → Add custom domain.*
Either delegate DNS to Netlify nameservers (easiest, gets auto-HTTPS) or
add A / CNAME records to your existing DNS. HTTPS is provisioned automatically.

## Local preview

```bash
cd interval-site
python3 -m http.server 8000
# open http://localhost:8000
```
