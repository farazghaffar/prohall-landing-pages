# Prohall Select One — A/B landing pages

Static A/B landing pages for [Prohall Select One](https://shop.prohall.ai/products/prohall-select-one) on shop.prohall.ai, measured with Split.

**Test: layout.** Both versions use the same headline ("Meet Prohall Select One — the Brazilian smoothing treatment"), copy, photos, price and buttons; only the design differs.

| Version | Path | Layout |
|---|---|---|
| A | `/select-one/v1/a/` | Classic: split hero, card grids, dark ingredients band |
| B | `/select-one/v1/b/` | Editorial: centered arched hero, numbered lists, timeline, dark buy band |

Both load `/select-one/v1/assets/styles.css` (brand tokens + layout A); B also loads `styles-b.css`.

## Live links (GitHub Pages)
Settings → Pages → Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.

- A: https://farazghaffar.github.io/prohall-landing-pages/select-one/v1/a/
- B: https://farazghaffar.github.io/prohall-landing-pages/select-one/v1/b/

Keep the trailing slash.

## Deploy (Vercel, optional)
Import this repo → preset **Other**, no build command. URLs: `https://<project>.vercel.app/select-one/v1/a/` and `/b/`.

## Before starting a Split run
1. Replace the placeholder `<script ... external-landing.js>` tag at the bottom of BOTH pages with the exact tag from Split → New run → Install tracking.
2. The Shopify theme bridge (`split-tracking.js` + `split-tracking.liquid`) must be installed on the live theme.
3. Never put raw page URLs in ads — use Split's generated links.

For a redesign, add `/select-one/v2/...` and start a new run; keep v1 unchanged.
