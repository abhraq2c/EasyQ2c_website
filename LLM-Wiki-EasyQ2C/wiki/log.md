# Wiki Log

Append-only timeline of wiki operations. Newest entries at the bottom.

Entry header format (mandatory, parseable by `grep "^## \[" wiki/log.md`):
`## [YYYY-MM-DD] <operation> | <short title>`

Allowed operations:
- `ingest` — a raw source was processed into wiki content.
- `query` — an answer was generated from wiki pages.
- `lint` — a health-check pass over wiki structure/content.
- `meta` — schema/index/log/structure maintenance.

---

## [2026-07-11] meta | Instantiate template for EasyQ2C website wiki

- Filled `AGENTS.md` §1 Domain: EasyQ2C IT software & services company; website knowledge base; primary tag `easyq2c`.
- Defined entity categories: company, product, service, location, contact-channel, brand-asset, team-member.
- Defined concept categories: Q2C domain, revenue/collection themes, value propositions, messaging, delivery patterns.
- Removed template callout from `AGENTS.md`; marked §10 checklist complete.
- Rewrote `README.md` for the EasyQ2C domain.
- Updated `wiki/index.md` Domain line, website URL, and raw assets table.
- Downloaded homepage SDLC diagram to `raw/assets/easyq2c-sdlc-diagram.png` (from `https://www.easyq2c.com/spd.png`).
- Files touched: `AGENTS.md`, `README.md`, `wiki/index.md`, `wiki/log.md`, `raw/assets/easyq2c-sdlc-diagram.png`.
- Next step: ingest `raw/Home - Welcome to EasyQ2C.md` (homepage web clip already present).

## [2026-07-11] ingest | Homepage web clip + logo assets

- Ingested [`raw/Home - Welcome to EasyQ2C.md`](../raw/Home%20-%20Welcome%20to%20EasyQ2C.md) → [`wiki/sources/home-welcome-easyq2c.md`](./sources/home-welcome-easyq2c.md).
- Referenced brand logos from [`raw/logo/`](../raw/logo/): `logo.jpeg`, `logo_with_caption.jpeg`.
- Created 14 entity pages: company, 3 products, 4 services, location, contact, 3 brand assets.
- Created 5 concept pages: Q2C, product-first org, revenue leakage, value propositions, tagline.
- Created [`wiki/overview.md`](./overview.md) as first synthesis.
- Updated [`wiki/index.md`](./index.md).
- Open gaps flagged: redacted phone, SubsSpend undefined, brand hex values, clip vs. live site hero mismatch.
- Files touched: 1 source, 14 entities, 5 concepts, 1 overview, index, log.

## [2026-07-11] meta | Logo SVG/PNG transparent variants

- Created transparent PNG variants from `logo.jpeg` and `logo_with_caption.jpeg` (full-res + 512px + 256px wordmark).
- Created vector SVG variants: `logo.svg`, `logo-with-caption.svg` (Poppins, colors `#2B365C` / `#3B86F4`).
- Updated brand-asset entity pages and `wiki/index.md` raw assets table.
- Files added under [`raw/logo/`](../raw/logo/): 7 new files (2 SVG, 5 PNG).
- Files touched: `wiki/entities/logo-easyq2c-wordmark.md`, `wiki/entities/logo-easyq2c-with-caption.md`, `wiki/index.md`, `wiki/log.md`.

## [2026-07-11] meta | Address change → Auburn (supersedes Girraween)

- Curator-provided update: EasyQ2C Pty Ltd address changed to Unit 132, 15A Mary Street, Auburn NSW 2144 (no web source; supersedes the homepage's Girraween address).
- Created [`wiki/entities/auburn-office.md`](./entities/auburn-office.md); archived old page to [`wiki/_archive/girraween-office.md`](./_archive/girraween-office.md) with `status: superseded`.
- Updated address + `Located at` link in [`easyq2c-pty-ltd.md`](./entities/easyq2c-pty-ltd.md), address in [`overview.md`](./overview.md), catalog line in [`index.md`](./index.md), and `location` example in `AGENTS.md`.
- Updated the website contact block in `index.html`.
- Note: `raw/Home - Welcome to EasyQ2C.md` left unchanged (immutable source; still shows original Girraween address).
- Files touched: `index.html`, `AGENTS.md`, `wiki/entities/auburn-office.md`, `wiki/_archive/girraween-office.md`, `wiki/entities/easyq2c-pty-ltd.md`, `wiki/overview.md`, `wiki/index.md`, `wiki/log.md`.
