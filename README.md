# The Corner Bean

The Corner Bean is a responsive café dashboard prototype built as a single-page web application. It presents fictional sales and stock information for an independent café, with interactive views for daily performance, item sales, product details, and inventory levels.

## Features

- **Overview dashboard** for today's sales, order count, busiest hour, yesterday's best seller, and low-stock warnings
- **Sales by item** with Today, Yesterday, and Last 7 days periods
- **Sorting** by units sold, revenue, or item name
- **Item detail view** with a seven-day sales table and sales progress chart
- **Stock management view** with search, low-stock filtering, status badges, and reorder actions
- **Mobile-friendly navigation** and accessible modal, form, table, and skip-link behaviour
- **Reset prototype** control to restore default view and filters

## Technology

- HTML5
- CSS and Bulma 1.0.2, loaded from cdnjs
- Vanilla JavaScript
- In-memory fictional data; no backend or database

## Getting Started

Open `index.html` directly in a modern browser. An internet connection is needed to load the Bulma stylesheet from the CDN.

To serve the project locally, run:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Prototype Navigation

The main navigation provides four working areas:

- Overview
- Sales by item
- Stock levels
- Item details, reached by selecting an item in the sales table

Reports and Settings are placeholders that open an out-of-scope modal. Reorder actions and the reset control demonstrate prototype interactions but do not persist changes.

## Data

The dashboard contains 20 menu items across Coffee, Tea, Cake, and Sandwich categories. Values are generated in `index.html` from fictional price, typical daily unit, stock, and reorder-level data.

Search and filter state is held only in the current browser session. Reloading or resetting the page restores the original dataset.