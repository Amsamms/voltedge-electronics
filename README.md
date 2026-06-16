# VoltEdge

A self-contained, fully interactive B2C consumer-electronics marketplace built as a single `index.html` (inline CSS + vanilla JS, Google Fonts only, no backend).

Part of a 10-site set demonstrating Chapter 8 (E-Commerce Systems). This site is the search-management reference: instant search plus faceted, parametric filtering, all client-side.

## Signature feature
- Instant search-as-you-type across name, brand, category and specs with a live result count
- Faceted filters: category, brand, connectivity, price range, minimum rating (AND across groups, OR within a group)
- Parametric sort (price, rating, newest) and removable active-filter chips with an empty state
- Cart, slide-in drawer and a staged checkout

## Run
Open `index.html` in any browser, or serve the folder over HTTP. No build step.

## Deploy
Push to a GitHub repo with Pages enabled (main branch, root). The `.nojekyll` file is included.
