# Prohall landing pages

Static A/B landing pages for shop.prohall.ai, measured with Split.

| Version | Path | Headline |
|---|---|---|
| A | `/select-one/v1/a` | Meet Prohall Select One — the Brazilian smoothing treatment |
| B | `/select-one/v1/b` | How to use Prohall Select One for smooth, frizz-free hair |

Both pages share `/select-one/v1/assets/styles.css`; only the `<title>` and `<h1>` differ.

## Deploy (Vercel)
Import this repo in Vercel → Framework preset **Other**, no build command, output directory `.` (root).
Public URLs will be `https://<project>.vercel.app/select-one/v1/a` and `/select-one/v1/b`.

## Before starting a Split run
1. Replace the placeholder `<script ... external-landing.js>` tag at the bottom of BOTH pages with the exact tag from Split → New run → Install tracking.
2. Install the Shopify theme bridge (`split-tracking.js` + `split-tracking.liquid`) on the live theme.
3. Never put raw page URLs in ads — use Split's generated links.

For a redesign, add `/select-one/v2/...` and start a new run; keep v1 unchanged.
