# html-scss-lab

A comprehensive learning laboratory for HTML, CSS, SCSS, and Tailwind CSS — progressing from semantic markup fundamentals through component architecture to full production-grade websites.

## Repository Structure

```
html-scss-lab/
├── html-css/
│   ├── semantics/       # Semantic HTML & attribute/pseudo selectors
│   ├── design/          # Product landing page with design-system thinking
│   ├── components/      # Standalone UI component catalogue
│   ├── theater/         # Interactive HTML/CSS playground
│   └── frontend/        # Omnifood — full production-like website
├── tailwind/
│   ├── init/            # Minimal Tailwind bootstrap
│   ├── theater/         # 18 step-by-step Tailwind lessons
│   ├── components/      # Tailwind UI component library
│   └── frontends/       # Complete Tailwind landing pages
├── css-scss/            # SCSS experimentation (reserved)
└── pwa/                 # Progressive Web App exploration (reserved)
```

## HTML-CSS Modules

### Semantics

A resume page and form submission page built entirely with semantic HTML5 elements.

**Concepts:** `<nav>`, `<menu>`, `<main>`, `<article>`, `<aside>`, `<section>`, `<address>`, `<dl>`/`<dt>`/`<dd>`, `<fieldset>`, attribute selectors, pseudo-selectors (`:where`, `:hover`).

### Design

A chair-shop product landing page that exercises design-system fundamentals.

**Concepts:** CSS Grid (`repeat(3, 1fr)`), Flexbox, a spacing scale (2/4/8/12/16/24/32 px), a font-size scale (10–44 px), SVG icon colouring, box shadows, border radius, link pseudo-class ordering (`:link` → `:visited` → `:hover` → `:active`), `<figure>` for product cards.

### Components

Six isolated UI components, each in its own HTML file:

| File | What it demonstrates |
|------|---------------------|
| `hero.html` | Background-image gradient overlay, centred CTA buttons |
| `accordion.html` | CSS-only FAQ toggle with numbered grid items |
| `pagination.html` | Circular page-number buttons with icon navigation |
| `carousel.html` | Testimonial carousel with dot indicators |
| `table.html` | `<thead>`/`<tbody>` with alternating-row colour |
| `app-layout.html` | Email-client layout using CSS Grid (nav, toolbar, list, content, sidebar) |

### Theater

An interactive playground built around "The Code Magazine" — a fictional blog.

**Pages:** `index.html` (main article), `blog.html` (simple post listing), `flexbox.html`, `css-grid.html`, plus a product-card challenge (Converse shoe layout).

**Concepts:** `display: flex`, `align-self`, `order`, `grid-template-columns`/`-rows`, `grid-column`/`grid-row`, `gap`, `justify-content`, `align-items`, pseudo-elements (`::first-letter`, `::after`), the box model.

### Frontend — Omnifood

A complete, production-like AI meal-delivery landing page.

**Sections:** Sticky nav with mobile hamburger toggle, hero with dual CTAs, "How it works" steps, meal showcase, testimonials, pricing tiers with feature comparison, call-to-action form, multi-column footer.

**CSS architecture:** Modular `style.css` (~2 000 lines), `queries.css` (responsive breakpoints), `utility.css` (reusable spacing/text helpers). Uses rem units throughout.

**JavaScript (`js/script.js`):** Footer year auto-update, mobile nav toggle, smooth anchor scrolling, Intersection Observer sticky nav, Safari flexbox-gap polyfill.

**Assets:** WebP hero with `<picture>` fallback, customer photos, meal images, gallery (12 images), press logos (Forbes, TechCrunch, NYT, USA Today, Business Insider), iOS/Android icons, favicon, PWA `manifest.webmanifest`.

## Tailwind Modules

### Init

Bare-minimum Tailwind project — a single `h1` with utility classes plus the standard `package.json`/`tailwind.config.js` scaffold.

### Theater — 18 Lessons

Progressive walkthroughs of the entire Tailwind utility API:

| # | Topic | # | Topic |
|---|-------|---|-------|
| 01 | Utility-first approach | 10 | Interactivity (cursor, selection) |
| 02 | Colour palette | 11 | Responsive breakpoints |
| 03 | Container & spacing | 12 | Multi-column layouts |
| 04 | Typography | 13 | Flexbox utilities |
| 05 | Sizing (width/height) | 14 | Grid utilities |
| 06 | Layout & position | 15 | Transform & transition |
| 07 | Backgrounds & shadows | 16 | Animation (keyframes) |
| 08 | Borders & radius | 17 | Theme customisation |
| 09 | Filters (blur, brightness) | 18 | Dark mode |

### Components

Six reusable Tailwind components:

| Component | Highlights |
|-----------|-----------|
| **Directives** | `@layer base/components/utilities`, custom `.btn-teal`, media-query decorators |
| **Email** | Responsive flex card (column → row), gradient background, hover-scale image |
| **Gallery** | Flex nav, group-hover border animation, search input with icon |
| **Login** | Two-column modal (form + image), social login (Facebook, Google) |
| **Modal** | Product card with strikethrough pricing, ping-animation stock indicator |
| **Pricing** | Three-tier pricing table with checkmark feature lists |

Each component ships with its own `package.json`, `tailwind.config.js`, source `styles.css` with `@tailwind` directives, and compiled `css/main.css`.

### Frontends — Clipboard

A multi-section landing page for a clipboard utility app. Custom colour theme (`strongCyan`, `lightBlue`, `grayishBlue`), sponsor logo grid, advanced responsive layout.

## Technologies

- **HTML5** — semantic elements, `<picture>`, forms, accessibility attributes
- **CSS3** — Grid, Flexbox, custom properties, pseudo-elements/classes, media queries, transitions, box-shadow, design-system scales
- **JavaScript** — DOM manipulation, Intersection Observer, event listeners, classList, feature detection
- **Tailwind CSS** — utility-first workflow, responsive prefixes, dark mode, custom themes, `@layer` organisation, group hover
- **PWA** — `manifest.webmanifest` for installability

## Getting Started

Static HTML/CSS files can be opened directly in a browser. For Tailwind projects:

```bash
cd tailwind/<project>
npm install
npm run watch   # rebuilds on file changes
```
