# LAT 91 Limited – lat91.co.nz

Static website (HTML/CSS, no build step), hosted on Vercel.

- Pages: `index.html`, `shipping.html`, `tourism.html`, `property.html`, `about.html`, `404.html`
- Styles: `assets/css/styles.css`
- Images, logo and compass: `assets/img/`
- Fonts (Figtree, self-hosted): `assets/fonts/`
- `vercel.json` enables clean URLs (`/shipping` rather than `/shipping.html`)

To edit copy or links, change the HTML files directly. Each push to `main` redeploys.

Hosting: Vercel project `lat91` (lat91.co.nz, www redirects). Linked to this repo, so every push to `main` publishes automatically.

## Parked mode (since 19 Nov 2026)

The site is parked: `index.html` is the "Launching soon" landing page. The full home page is kept as `home-full.html`. `vercel.json` sends /shipping, /tourism, /property and /about back to the landing page with a temporary redirect.

To relaunch the full site:
1. Rename `index.html` to `landing.html`, and `home-full.html` to `index.html`.
2. Delete the `redirects` block from `vercel.json`.
3. Commit and push to `main`. Vercel publishes it automatically.
