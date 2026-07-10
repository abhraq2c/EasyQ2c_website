# EasyQ2C Website Wiki

An LLM-maintained knowledge base for **EasyQ2C** — an Australian IT software & services company focused on Quote-to-Cash (Q2C) workflows.

This wiki captures company identity, products, services, messaging, brand assets, and public web content to support designing and evolving the [EasyQ2C website](https://www.easyq2c.com/).

## What this wiki is for

- Single source of truth for website copy, information architecture, and brand references
- Structured entity and concept pages for products (Debt Collection Systems, Spend Tracker, SubsSpend), services, and Q2C domain expertise
- Cited summaries of ingested sources (web clips, notes, brand guidelines)
- Living synthesis via `wiki/overview.md` as sources accumulate

## Quick start

1. Open this folder in Cursor — `AGENTS.md` loads automatically as the agent schema.
2. Drop sources into `raw/` (web clips, PDFs, notes, logos into `raw/assets/`).
3. Ask the agent to **ingest** a source, **query** the wiki, or run a **lint** health check.
4. Browse pages in `wiki/` — start with [`wiki/index.md`](./wiki/index.md).

## Layout

```
.
├── AGENTS.md           # operating contract (domain, workflows, page formats)
├── README.md           # this file
├── docs/LLM-WIKI.md    # abstract pattern reference (do not modify)
├── raw/                # immutable sources
│   ├── assets/         # logos, diagrams, downloaded images
│   └── …               # web-clips, notes, pdfs (as added)
└── wiki/               # LLM-generated knowledge pages
    ├── index.md        # canonical catalog — read this first
    └── log.md          # append-only operation history
```

## Current status

- **Instantiated:** 2026-07-11
- **Primary tag:** `easyq2c`
- **First ingest complete:** [`wiki/sources/home-welcome-easyq2c.md`](./wiki/sources/home-welcome-easyq2c.md) (homepage, 2026-07-11)
- **Brand assets:** [`raw/logo/logo.jpeg`](./raw/logo/logo.jpeg), [`raw/logo/logo_with_caption.jpeg`](./raw/logo/logo_with_caption.jpeg), [`raw/assets/easyq2c-sdlc-diagram.png`](./raw/assets/easyq2c-sdlc-diagram.png)
- **Start here:** [`wiki/overview.md`](./wiki/overview.md)

## Pattern reference

The wiki implements the [LLM Wiki pattern](./docs/LLM-WIKI.md): raw sources → structured wiki pages → compounding knowledge over time. You curate sources and ask questions; the LLM maintains the wiki.
