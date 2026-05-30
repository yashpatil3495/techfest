# CYBORG SYSTEMS // Landing Page v2.084

> *Where Human Meets Machine*

A single-page, immersive **cyborg-themed landing page** built with pure HTML, CSS, and vanilla JavaScript. No frameworks, no build tools, no external JS libraries — just open `index.html` and experience the future.

![Techfest](https://img.shields.io/badge/Techfest-IIT%20Bombay-FF6B00?style=flat-square&labelColor=050810)
![Task](https://img.shields.io/badge/CA%20Program-Web%20Development-00F5FF?style=flat-square&labelColor=050810)
![Tech](https://img.shields.io/badge/Stack-HTML%20%2F%20CSS%20%2F%20JS-FFB800?style=flat-square&labelColor=050810)

---

## 🔬 Overview

This project is a submission for the **Techfest IIT Bombay — Campus Ambassador (CA) Program**, under the **Web Development** domain.

> **Task 1:** Cyborg-Themed Landing Page Development

An atmospheric, dark-themed landing page that visually fuses human biology with machine precision — the **"Organic Machine"** aesthetic. Designed to feel like a neurosurgeon's dashboard meets a military-grade exoskeleton interface.

**Key characteristics:**
- Dark, high-contrast cinematic design
- HUD overlays, circuit traces, and bioluminescent effects
- Clinical, militaristic copywriting tone
- Fully self-contained in a single HTML file (~73KB)
- Zero external dependencies (except Google Fonts CDN)
- Fully responsive across mobile, tablet, and desktop

---

## 📐 Sections

| # | Section | Description |
|---|---------|-------------|
| 1 | **Hero** | Full-viewport canvas particle network, glitch-text headline, HUD reticle, SVG EKG heartbeat |
| 2 | **Stats Bar** | Animated number counters — Neural Sync Rate, Response Latency, Augmented Users, ISO Cert |
| 3 | **Features** | 6 capability cards with inline SVG icons and hover glow effects |
| 4 | **Anatomy** | Detailed SVG human silhouette with circuit overlays, pulsing augmentation points, and scan-line sweep |
| 5 | **Timeline** | 4-phase integration process with animated dashed connector |
| 6 | **Testimonials** | 3 classified dossier cards with hexagonal avatars and signal-strength bars |
| 7 | **CTA** | Terminal-style email input with concentric ring pulse animation |
| 8 | **Footer** | Animated cyan border sweep, navigation, and SVG social icons |

---

## ✨ Animations & Effects

| Effect | Implementation |
|--------|---------------|
| Particle network | `<canvas>` + `requestAnimationFrame` (80 particles desktop, 40 mobile) |
| Glitch headline | CSS `@keyframes` with `clip-path` + `transform: skewX` |
| EKG heartbeat | SVG `stroke-dasharray` / `stroke-dashoffset` animation |
| Number counters | Intersection Observer + eased `requestAnimationFrame` increment |
| Scroll reveal | Intersection Observer toggling CSS class with staggered delays |
| Card hover glow | CSS `box-shadow` + `border-color` transitions |
| Scanline overlay | Fixed pseudo-element with `repeating-linear-gradient` |
| Body breathing | SVG `transform: scale()` keyframe loop |
| Scan-line sweep | CSS `::after` pseudo-element with vertical `translateY` animation |
| Ring pulses | CSS `scale` + `opacity` keyframes with staggered delays |
| Timeline connector | `repeating-linear-gradient` with animated `background-position` |
| Footer border | `linear-gradient` with animated `background-position` sweep |

All animations use `transform` and `opacity` only — zero layout thrashing.

---

## 🎨 Design System

### Color Palette

```
--bg-primary:      #050810     Near-black deep space
--bg-secondary:    #0A0F1E     Dark navy surface
--bg-panel:        #0D1A2A     Panel/card background
--accent-cyan:     #00F5FF     Primary neon — circuitry
--accent-electric: #4D9EFF     Secondary blue — energy
--accent-organic:  #FF4B6E     Organic red — pulse, life
--accent-amber:    #FFB800     Warning amber — data
--text-primary:    #E8F4FF     Near-white body text
--text-secondary:  #7FA8C9     Muted blue-grey labels
--text-faint:      #2A4060     Decorative/dim text
```

### Typography

| Usage | Font | Source |
|-------|------|--------|
| Display / Headlines | `Orbitron` | Google Fonts |
| Body / UI Text | `Share Tech Mono` | Google Fonts |
| Labels / Tags | `Rajdhani` | Google Fonts |

---

## 🚀 Getting Started

### Quick Start

1. Clone or download this repository
2. Open `index.html` in any modern browser

```bash
# Clone
git clone <repo-url>
cd techfest

# Open (Windows)
start index.html

# Open (macOS)
open index.html

# Open (Linux)
xdg-open index.html
```

That's it. No `npm install`, no build step, no server required.

### Development

Since this is a single-file project, just edit `index.html` in your preferred editor. For live-reload during development, you can use any static file server:

```bash
# Using Python
python -m http.server 8080

# Using Node.js (npx)
npx serve .
```

---

## 📱 Responsive Breakpoints

| Breakpoint | Target | Behavior |
|------------|--------|----------|
| `≤ 1024px` | Small desktop | Features → 2-column, anatomy stacks |
| `≤ 768px` | Tablet | Stats → 2×2, testimonials → single column |
| `≤ 480px` | Mobile | Everything single-column, reduced particle count |

Supports `prefers-reduced-motion` — all intensive animations are gracefully disabled.

---

## ♿ Accessibility

- Semantic HTML5 landmarks (`<header>`, `<main>`, `<section>`, `<footer>`)
- `aria-label` on all interactive elements and sections
- `aria-hidden="true"` on decorative elements (canvas, reticle, rings)
- `role="img"` + `aria-label` on the anatomy SVG
- `prefers-reduced-motion` media query support
- Sufficient color contrast ratios against dark backgrounds

---

## 📂 Project Structure

```
techfest/
├── index.html     # Complete landing page (HTML + CSS + JS)
└── README.md      # Project documentation
```

---

## 🛠 Technical Specifications

- **File size:** ~73KB (single file, no external assets except Google Fonts)
- **External dependencies:** Google Fonts CDN only
- **JavaScript:** Vanilla ES6, no libraries
- **CSS:** Custom properties, Grid, Flexbox, `@keyframes`
- **Browser support:** Chrome, Firefox, Edge, Safari (latest 2 versions)
- **Performance:** GPU-composited animations only (`transform`, `opacity`)

---

## 📝 Content Guidelines

The page uses a clinical, militaristic tone consistent with the near-future setting:

- Numbers are specific: `98.7%`, `0.003ms`, `4.2 billion`
- Section labels use `//` prefix or `[ BRACKETS ]`
- Technical jargon encouraged: neural sync, bio-lattice, cortex mesh
- Date references grounded in near-future: `System v2.084`, `Cycle 084`, `EST. 2041`

---

## 🏫 About

This project was built as part of the **Techfest IIT Bombay Campus Ambassador Program** — Asia's largest science and technology festival.

- **Event:** [Techfest, IIT Bombay](https://techfest.org)
- **Domain:** Web Development
- **Task:** Cyborg-Themed Landing Page Development

---

## 📄 License

MIT License — free for personal and commercial use.

```
© 2084 CYBORG SYSTEMS CORP // ALL RIGHTS RESERVED
```
