# Sharon Milone — Personal Landing Page

Built with [Astro](https://astro.build). Deployed to GitHub Pages at `https://sharonhmilone.github.io/about/`.

---

## Local development

**Prerequisites:** Node.js 18+

```bash
# Install dependencies
npm install

# Start dev server (http://localhost:4321/about/)
npm run dev

# Build for production
npm run build

# Preview production build locally
npm run preview
```

---

## Project structure

```
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Header.astro        # Sticky minimal top bar
│   │   ├── Hero.astro          # Name, headline, CTAs, soundbite
│   │   ├── ProofStrip.astro    # Logo row + swipeable chips
│   │   ├── HowIThink.astro     # 4 principle cards + pull quote
│   │   ├── WatchMeThink.astro  # Featured video + grid
│   │   ├── Soundbites.astro    # Large quote section (dark bg)
│   │   ├── WhatIBuild.astro    # 3 capability pillars + examples
│   │   ├── WhatToExpect.astro  # Hiring manager traits
│   │   └── CTAFooter.astro     # Dark CTA + bottom bar
│   ├── data/
│   │   └── content.js          # ← Edit all copy and data here
│   ├── layouts/
│   │   └── Layout.astro        # HTML shell, fonts, meta, scripts
│   ├── pages/
│   │   └── index.astro         # Page composition
│   └── styles/
│       └── global.css          # Design tokens, reset, utilities
├── .github/
│   └── workflows/
│       └── deploy.yml          # Auto-deploy to GitHub Pages
├── astro.config.mjs
└── package.json
```

---

## Updating content

**All copy and data lives in `src/data/content.js`.** You can update:

- `hero` — eyebrow, headline, subhead, CTA labels/links, featured quote
- `proofStrip` — logo names, working-style chips
- `howIThink` — principle cards, pull quote
- `watchMeThink` — featured video, video grid cards (title, context, tag, href)
- `soundbites` — quote text and optional attribution
- `whatIBuild` — pillar labels, descriptions, example bullets
- `whatToExpect` — trait labels and descriptions
- `ctaFooter` — CTA heading, subhead, button labels/links, copyright

---

## GitHub Pages deployment

GitHub Actions deploys automatically on every push to `claude/astro-landing-page-HBXcv`.

**First-time setup:**
1. Go to your repo → **Settings → Pages**
2. Under **Source**, select **GitHub Actions**
3. Push to `claude/astro-landing-page-HBXcv` and the workflow will run

**Live URL:** `https://sharonhmilone.github.io/about/`

---

## Design system

| Token | Value |
|---|---|
| Background | `#F8F5F0` warm off-white |
| Surface | `#FFFFFF` |
| Text | `#1C1A17` warm near-black |
| Text muted | `#6B6460` |
| Accent | `#C96127` warm burnt orange |
| Sans font | Plus Jakarta Sans |
| Serif font | DM Serif Display (quotes only) |

Breakpoints: mobile-first, `640px`, `768px`, `1024px`.
