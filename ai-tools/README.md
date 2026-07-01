# AI Tools Research — Top 1,000 (in progress)

A structured, categorized database of the most-used AI tools, with pricing, release dates, ratings,
descriptions, and hidden features. Built and verified in **batches** to keep the data accurate.

## Files

| File | What it is |
|------|------------|
| [`AI-Tools-Master.csv`](./AI-Tools-Master.csv) | The spreadsheet. One row per tool with all structured columns. Open in Excel / Google Sheets. |
| [`Tool-Profiles.md`](./Tool-Profiles.md) | Deep profiles: description, main features, **hidden features**, release date, pricing. |
| [`Filtered-Lists.md`](./Filtered-Lists.md) | Ready-made views: free-tier, business/enterprise, coding-only. |
| [`AI-Tool-Directories.md`](./AI-Tool-Directories.md) | Source websites/directories used to build and refresh the list. |

## Spreadsheet columns
`No · Tool · Category · Release · Pricing Model · Free Tier / Trial · Paid Plans (USD/mo) · G2 Rating (approx) · Est. Monthly Web Visits · Est. Mobile MAU · Origin`

## Categories (17)
LLM Assistants · Search & Answer Engines · Writing & Grammar · Image Generation & Editing ·
Video Generation & Editing · Audio, Music & Voice · Coding & Development · Productivity & Knowledge ·
Presentations & Design · Marketing, Sales & SEO · Automation, Agents & No-code · Translation & Language ·
Meetings & Transcription · Education & Research · Detection & Integrity · Companion & Character · Model & Dev Hubs

## Roadmap to 1,000
The catalog is being expanded from the current flagship set toward 1,000 tools, in batches of ~100.
Each batch: no duplicate tools, category-balanced, with pricing/release verified from official or reputable sources.

- [x] **Batch 1 — Top ~100 by usage** (this commit): full schema + deep profiles for flagships.
- [ ] Batch 2–3: next ~200 (broader per-category depth).
- [ ] Batch 4–7: long tail to 1,000 (niche + vertical tools).
- [ ] Ongoing: monthly refresh of pricing, ratings, and rankings.

## Important data caveats
- **Traffic ≠ usage.** Web-visit figures miss mobile-app and API usage.
- **Mobile MAU** is rarely disclosed publicly, so most rows show `—` rather than a guess.
- **G2 ratings are approximate** (rounded) and should be verified at g2.com.
- **Pricing changes frequently.** Figures are 2026 snapshots; confirm on the vendor page before relying on them.
- Adult "companion" apps that rank on some raw-traffic charts are intentionally excluded.

## How to refresh
1. Pull the latest monthly rankings (see `AI-Tool-Directories.md`).
2. Add new rows to `AI-Tools-Master.csv` (check for duplicates first).
3. Write profiles for any new flagship-level tools.
4. Regenerate the views in `Filtered-Lists.md`.
