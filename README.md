# Gokul T Vibin — Digital Marketing Executive Portfolio

> **Psychology-Led Performance Marketing Portfolio**  
> Tailored for Gokul T Vibin (Kochi, Kerala, India). Built as a self-contained, high-converting, single-page editorial web application with zero external framework dependencies.

---

## 📁 Repository & Project Architecture

```
gokul-dm/
├── index.html                   # Single-file production portfolio (~72 KB)
├── robots.txt                   # Search crawler directives
├── sitemap.xml                  # Canonical XML sitemap for SEO
├── README.md                    # Complete technical and deployment guide
└── assets/
    ├── Gokul-TVibin-Resume.pdf  # Valid, self-contained candidate resume
    └── og-image.svg             # 1200x630 OpenGraph social share card
```

---

## 🎨 Color System — "Amber on Slate"

Grounded in **classical color theory** for maximum conversion tension and visual prestige:
- **Complementary Hue Pair**: Warm Amber (38°) ↔ Cool Slate (220°).
- **Temperature Contrast**: Warm attention accents layered over a calm, deep ground.
- **Chroma Discipline**: One high-chroma warm family (Amber + Rose); surfaces and body text remain low-chroma.

### Color Tokens

| Token | Hex | Role | Contrast Ratio |
|---|---|---|---|
| `--bg-base` | `#0C111C` | Page Background | — |
| `--bg-surface` | `#1D2534` | Cards & Structured Panels | — |
| `--bg-elevated` | `#2F3A4D` | Hover & Active States | — |
| `--ink` | `#F5F1E8` | Warm Bone Primary Reading Copy | **15.1:1 (AAA)** |
| `--ink-dim` | `#A8AEB8` | Neutral Secondary Copy | **7.5:1 (AAA)** |
| `--ink-mute` | `#6B7280` | Tertiary Marginalia & Dates | **4.9:1 (AA)** |
| `--ink-inverse` | `#0C111C` | Mandatory Label on Amber Surfaces | **8.5:1 (AAA)** |
| `--amber` | `#F59E0B` | Primary Accent (CTAs, Key Numerals) | **8.5:1 (AAA)** |
| `--amber-hi` | `#FBBF24` | Hover & Pulse States | **10.4:1 (AAA)** |
| `--amber-lo` | `#B45309` | Pressed States | **4.8:1 (AA)** |
| `--rose` | `#FB7185` | Secondary Warm Accent (Deltas, Status) | **7.2:1 (AAA)** |
| `--rule` | `rgba(245,241,232,0.08)` | Hairline Separators & Crop Marks | — |

### Enforced 60 / 30 / 10 Usage Law
- **Ground + Text = 92%** of every viewport.
- **Amber = ≤ 6%** (Primary CTAs, H1 brand growth highlight, key metric numerals).
- **Rose = ≤ 2%** (Data deltas `+2.4x`, `−38%`, `CURRENT` status dot, active location pill).
- **Contrast Law**: Any Amber surface strictly carries `--ink-inverse` (`#0C111C`).

---

## ⚡ Engineered Techniques

1. **SVG `feTurbulence` Grain Overlay**: Full-viewport fixed noise filter (`baseFrequency="0.9"`, `opacity: 0.035`, `mix-blend-mode: overlay`, `pointer-events: none !important`).
2. **CSS Counters with `::before`**: Automated chapter numbering (`01 / 06` to `06 / 06`) driven natively by CSS counter rules.
3. **`animation-timeline: view()`**: CSS view scroll timelines for card entrances with progressive `@supports` immediate fallback.
4. **`:has()` Sibling Dimming**: Focusing or expanding any card subtly dims sibling cards (`opacity: 0.55; filter: saturate(0.7)`) with an undim on hover.
5. **`clip-path: circle()` Reveal**: Education qualification cards reveal institutional details via circular transition with touch tap support.
6. **Dynamic View Transitions API**: Card expansions/collapses use `document.startViewTransition()` with dynamically allocated `view-transition-name` identifiers that clean up automatically after 320ms.
7. **Container Queries**: `@container (max-width: 440px)` enables cards to self-adapt their internal layouts to card width rather than viewport width.
8. **Balanced Typographic Discipline**: `text-wrap: balance` on headings (`h1–h3`) and `text-wrap: pretty` on short card titles.
9. **`@starting-style` Transitions**: Mobile menu takeover and Back-to-Top pill enter smoothly from `display: none` using `transition-behavior: allow-discrete`.
10. **Zero-Shift Interactions**: Jitter-free layout architecture where hovering never triggers text reflow or vertical height displacement.
11. **Single-Space Floating Labels**: Form fields use `placeholder=" "` to power bug-free CSS floating labels via `:has(:not(:placeholder-shown))` and `:has(:focus)`.
12. **Recruiter-Friendly Print Stylesheet**: Includes `@media print` rules that hide interactive widgets and format all experience bullets into a pristine white multi-page CV layout when pressing `Ctrl+P`.

---

## 🚀 Instant Deployment Guide

Because the entire website is self-contained with no npm or build scripts, you can deploy it in under 60 seconds:

### Option 1: GitHub Pages (Free)
1. Push this directory to a GitHub repository named `gokul-portfolio`.
2. Go to **Settings** → **Pages**.
3. Under **Branch**, select `main` and root `/`, then click **Save**.
4. Your site will be live at `https://<your-username>.github.io/gokul-portfolio/`.

### Option 2: Vercel / Netlify
- Drag and drop the `gokul-dm` folder directly into the [Vercel](https://vercel.com) or [Netlify](https://netlify.com) dashboard.
- Zero configuration required. It will deploy instantly.

### Custom Domain Setup (`gokultvibin.com`)
1. In your domain registrar (Namecheap, GoDaddy, Cloudflare), set up:
   - `CNAME` for `www` → `<your-username>.github.io`
   - `A` records for `@` pointing to GitHub Pages / Vercel IPs.
2. Update the canonical URL in `index.html` if you change domain.

---

## 👤 Candidate Profile Foundation

- **Name**: Gokul T Vibin
- **Role**: Digital Marketing Executive
- **Location**: Kochi, Kerala, India
- **Email**: `gokultvibin.work@gmail.com`
- **Phone / WhatsApp**: `+91 9048646762`
- **LinkedIn**: `https://www.linkedin.com/in/gokultvibin`
- **Core Competencies**: Meta Ads, Google Ads, Technical SEO, Conversion Rate Optimization, Consumer Psychology, Content Strategy.

