# E&S Surplus Lines — Stamping Office Interactive Map

An interactive map of stamped excess & surplus lines premium and item counts across
the 15 US stamping office states, 10 lines of business, 2022–2025.

**Live map:** `https://<your-username>.github.io/<repo-name>/`

## What's here

| File | Purpose |
|---|---|
| `index.html` | The entire map — geometry, data, styling and interactivity, all embedded. No build step, no dependencies. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is rather than running them through Jekyll. |

## Publishing it

1. Create a new repository on github.com.
2. Upload `index.html` and `.nojekyll` (drag both into the upload page).
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then Save.
5. Wait a minute or two, then reload the Settings → Pages screen for your live URL.

Anything named `index.html` at the root becomes the page served at the repo's URL.

## Before you publish

GitHub Pages is only free on **public** repositories. Public means anyone with the
URL can view the map, and search engines can index it. Consider whether that suits
this content, which carries Ryan Specialty branding and is structured to accept an
overlay of internal book-of-business data later. Private repositories support Pages
only on paid GitHub plans.

## Updating it

Replace `index.html` in the repo. Pages redeploys automatically within a minute or so.

## Data sources

| Years | Source |
|---|---|
| 2022, 2023 | WSIA / U.S. Surplus Lines Service Offices — *Stamping Office Premium and Transaction Report, 2023 Annual Report* (12 Feb 2024) |
| 2024, 2025 | WSIA — *Stamping Office Premium and Item Report, 2025 Annual Report* (29 Jan 2026) |

2024 figures are WSIA's restated ones. The 2024 Annual Report was deliberately
excluded, as its originally published figures were later restated.

Premium totals reconcile exactly to WSIA's published annual figures in all four
years: $63.39B (2022), $72.66B (2023), $83.81B (2024), $90.33B (2025).

## Known data gaps

- Arizona and Utah have no multi-peril coverage category, so that line reads $0 / 0 items.
- Utah's multi-peril row is absent entirely from the 2025 report for 2024 and 2025.
  These render as "no data" (diagonal hatch), never as zero.
