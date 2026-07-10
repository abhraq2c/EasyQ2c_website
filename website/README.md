# EasyQ2C Website

Modern single-page marketing site for **EasyQ2C Pty Ltd** — Australian IT software & services company specializing in Quote-to-Cash (Q2C) workflows.

## Preview locally

Open `index.html` directly in a browser, or serve with any static file server:

```powershell
# Python (if installed)
python -m http.server 8080 --directory .

# Node.js
npx serve .
```

Then visit `http://localhost:8080`.

## Structure

```
website/
├── index.html          # Single-page site
├── css/styles.css      # Brand styles (navy #2B365C, blue #3B86F4)
├── js/main.js          # Nav, scroll reveal, contact form
└── assets/             # Logos, SDLC diagram, favicon
```

## Sections

- **Hero** — tagline, CTAs, SDLC diagram
- **About** — company story and mission
- **Services** — Enterprise, Mobile, Custom Engineering, API Integration
- **Products** — Debt Collection Systems, Spend Tracker, SubsSpend
- **Why EasyQ2C** — value propositions
- **Process** — SDLC lifecycle
- **Contact** — address, email, inquiry form

## Deploy

Upload the `website/` folder contents to any static host (Netlify, Vercel, GitHub Pages, S3, or your web server).

## Brand assets source

Original assets live in `../LLM-Wiki-EasyQ2C/raw/logo/` and `../LLM-Wiki-EasyQ2C/raw/assets/`.
