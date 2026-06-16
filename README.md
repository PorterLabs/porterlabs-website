# porterlabs-website

Marketing website for [PorterLabs](https://porterlabs.ai) — deployed via Cloudflare Pages.

## Stack

- Pure HTML/CSS/JS — no build step required
- Hosted on Cloudflare Pages (auto-deploy on push to `main`)
- Custom domain: `porterlabs.ai`

## Structure

```
porterlabs-website/
├── public/                  ← Cloudflare Pages root (serve from here)
│   ├── index.html           ← Main site (single-page, anchor-linked sections)
│   └── assets/
│       └── logos/           ← Transparent PNG logos (mark, full, horizontal)
├── .github/
│   └── workflows/           ← CI hooks (future use)
├── .gitignore
└── README.md
```

## Sections (V1)

1. Hero
2. MTP — Massively Transformative Purpose
3. Thesis — The Porter Equation
4. The Architecture — Recursive system flow
5. Founding Principles
6. Portfolio — Clout, Triplebolt, Kairix, BarberStack
7. Selection Criteria — The Areopagus filter
8. Contact CTA
9. Footer

## Roadmap

| Phase | Status | Description |
|-------|--------|-------------|
| P0 | ✅ Complete | Design + Build V1 |
| P1 | 🔵 Next | Deploy to porterlabs.ai via Cloudflare Pages |
| P2 | ⬜ Backlog | Content expansion — About, team, Areopagus teaser |
| P3 | ⬜ Backlog | SEO + Meta — OG tags, sitemap, Cloudflare Analytics |
| P4 | ⬜ Backlog | Multi-page expansion — /companies, /atrium, /blog |

## Deploy

Connected to Cloudflare Pages. Push to `main` → auto-deploy in ~30s.

Cloudflare Pages settings:
- **Build command:** *(none — static site)*
- **Output directory:** `public`
- **Root directory:** `/`
