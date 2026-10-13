# ShopNest — E-commerce Accounting Close (July 2026)

A single-file, browser-based **month-end close workbook** for an e-commerce business (ShopNest).
Everything — layout, styling, data and interactivity — lives in one `index.html`. No build step, no
server, no dependencies to install: open the file and it runs.

## Live demo

Once GitHub Pages is enabled: <https://palakpeshwani69428-del.github.io/ecommerce-accounting/>

## What's inside

- **Overview** — KPI cards (invoiced / collected / spent), an expenses **donut** chart with a
  category legend, and an invoiced-vs-collected-vs-spent **bar** chart. Charts are rendered with
  Chart.js.
- **Raw data** — tabbed ledgers with live in-table filtering:
  - Bank statement
  - Credit card statement
  - Invoices (AR)
  - Bills (AP)
  - Expenses & categories
- **Reconciliation** — reconciles the ledgers against the bank/credit-card records.
- **Issues** — a log of review items surfaced during the close.
- **Closing** — the month-end close summary.

The UI ships with a **light/dark theme toggle** and a responsive sidebar navigation.

## Usage

1. Download or clone the repository.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari).

That's it — 100% static, client-side only.

## Tech

- One self-contained `index.html`.
- [Chart.js](https://www.chartjs.org/) 4.4.0, loaded from the jsDelivr CDN (the only runtime
  external dependency, needed for the charts).
- Google Fonts: **Hanken Grotesk** + **IBM Plex Mono**.

## Notes on this push

The `index.html` committed here is the **authentic, unmodified deliverable**. The hosting layer
serves a copy with an injected `data-tmly-media-guard` script; that wrapper has been stripped so
the repository contains exactly the file as authored.
