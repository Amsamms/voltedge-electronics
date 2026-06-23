# VoltEdge

A self-contained, fully interactive B2C consumer-electronics marketplace built as a single `index.html` (inline CSS + vanilla JS, Google Fonts only, no backend).

Part of a 10-site set demonstrating Chapter 8 (E-Commerce Systems). This site is the search-management reference: instant search plus faceted, parametric filtering, all client-side.

## Signature feature
- Instant search-as-you-type across name, brand, category and specs with a live result count
- Faceted filters: category, brand, connectivity, price range, minimum rating (AND across groups, OR within a group)
- Parametric sort (price, rating, newest) and removable active-filter chips with an empty state
- Cart, slide-in drawer and a staged checkout

## Pages (hash router, no build step)
- Every product opens its own page: `#/product/<id>` (specs, description, related items, Add to cart / Buy now)
- Separate Support pages: `#/shipping`, `#/returns`, `#/warranty`, `#/contact`
- Separate Company pages: `#/about`, `#/careers`, `#/press`, `#/privacy`
- All pages are fully bilingual (English + Arabic, with RTL)

## Built-in assistant
- A bilingual chat assistant (bottom-right) answers product, shipping, returns and warranty questions.
- It calls Mistral AI directly from the browser. NOTE: the API key is visible in the page source by design (static site, no backend).

## Secret strategy presentation
- Type `strategy` in the search bar, or open `#/strategy`.
- Launches a full-screen, bilingual, interactive deck answering the Chapter 8 "E-Commerce Strategy Checklist" (7 questions), grounded in this store's real catalog and features. Arrow keys / dots to navigate, Esc to exit.

## Run
Open `index.html` in any browser, or serve the folder over HTTP. No build step.

## Deploy
Push to a GitHub repo with Pages enabled (main branch, root). The `.nojekyll` file is included.
