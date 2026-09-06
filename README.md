# CocoFert — Organic Fertilizer Website

Marketing website for CocoFert Enterprise (Navrongo, Ghana), built by BeyondURL.

## Structure

- `public/index.html` — the full site (single-file HTML/CSS/JS, no build step)
- `wrangler.jsonc` — Cloudflare Workers static assets config

## Deploy (Cloudflare Workers)

This repo deploys as a static site via **Workers Static Assets** — Cloudflare's
current recommended path (not Pages).

**One-time setup (dashboard):**
1. Cloudflare dashboard → Workers & Pages → Create → Import a Git repository
2. Select this repo, keep default build settings (no build command needed —
   it's static HTML)
3. Deploy. Every push to `main` auto-deploys via Workers Builds.

**Manual deploy (if needed):**
```
npx wrangler deploy
```

## Pending

- [ ] Contact form + partner inquiry modal: wire to Web3Forms
- [ ] Custom domain connection (to be added later)
