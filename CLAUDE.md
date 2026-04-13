# 2017 Portfolio Site

Pete Thomas's original 2017 portfolio, converted from plain HTML/CSS/JS to Astro. Design, layout and content are intentionally preserved exactly as-is.

## Stack
- Astro v6 (static output)
- Tachyons CSS (utility classes, loaded from `public/css/`)
- Custom CSS in `public/css/main.css` (and `main.scss` source)
- jQuery + plugins in `public/js/`
- No framework components — pure HTML in `.astro` files

## Local development
```bash
npm run dev
```

## Build
```bash
npm run build
```

Output goes to `dist/`.

## Structure
- `src/layouts/Layout.astro` — shared layout with header, nav, footer, and all scripts
- `src/pages/` — one `.astro` file per page, content only (no header/footer)
- `public/css/` — tachyons.min.css + main.css/scss
- `public/js/` — main.js, plugins.js, vendor/
- `public/img/` — all images and videos for case studies

## Pages
- `/` — homepage with 3 case study cards
- `/work` — full work listing (Geckoboard, Huddle, Miscellaneous Adventures, Cloth and Notions)
- `/about` — bio page
- `/building-widgets` — Geckoboard widget builder case study
- `/clicker` — Geckoboard hack week case study
- `/data-visualization` — data visualization overview
- `/data-visualisation` — redirects to `/data-visualization` (British spelling)
- `/404` — 404 page

## Deploy
Not yet deployed. Plan is GitHub repo + GitHub Actions + Cloudflare Workers (same pattern as the new portfolio site).

## Important
- Do not change the design, layout or content without being asked — the goal is to preserve the 2017 site faithfully
- Scripts use `is:inline` directive to prevent Astro bundling public JS files
- Original HTML files are preserved in `/Users/peterthomas/Projects/2017 portfolio/` (note the space in the folder name)
