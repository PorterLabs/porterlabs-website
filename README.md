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
| P1 | ✅ Complete | Deploy to pocolabs.ai via Cloudflare Pages |
| P1.5 | ✅ Complete | Favicon (PL mark) + email obfuscation fix |
| P2 | 🔵 Next | Content expansion — Areopagus teaser page (`/areopagus`). About/team deferred (not ready to name council publicly). |
| P3 | ⬜ Backlog | SEO + Meta — OG tags, sitemap, Cloudflare Analytics |
| P4 | ⬜ Backlog | System deep-dives — one scroll section per layer (Aurelius → Polaris → Nodes → Thundr → Deployment → Analytics) with real examples |
| P5 | ⬜ Backlog | Multi-page expansion — /companies, /atrium, /blog |
| P6 | ⬜ Backlog | Mobile polish pass (Stu to flag when ready) |
| — | 🟡 Ongoing | Domain acquisition — porterlabs.ai (currently owned, Stu reaching out) |

## Deploy

Connected to Cloudflare Pages. Push to `main` → auto-deploy in ~30s.

Cloudflare Pages settings:
- **Build command:** *(none — static site)*
- **Output directory:** `public`
- **Root directory:** `/`
