# Reference notes — woblo.in (studied 2026-09-19)

Source: https://woblo.in/ — marketing page for Woblo, a Chrome extension that extracts colors, fonts, icons and CSS from any live page and exports them to Tailwind, shadcn, or an AI prompt.

This folder's `index.html` is an original study ("Spectra") that borrows the source's layout logic and visual grammar. No copy, branding, logos, screenshots, fonts or code were taken from the source.

## Observed visual system

Measured live via computed styles (desktop, 1280px):

- **Surface:** near-white `#fbfbfb` page, white cards, hairline borders (`#e9e9ee` range), light gray `#f4f4f6` inset areas and footer band.
- **Ink:** `#101013` headings and body; muted gray-blue `#5f6470`-range secondary text; faint `#8a8f9c` micro-labels.
- **Accent:** blue `#0f7fff` family. Primary CTA is a *light* vertical blue gradient (`#edf4ff → #d6e7ff → #a2c7ff → #99cbf8 → #a2d2f7`) with black text, full pill radius (`999px`), weight 500.
- **Type:** Inter everywhere; H1 56px / weight 500 / letter-spacing -0.03em / line-height 1.1; mono micro-labels in Geist Mono (proof line, "hover to open", dimension chips).
- **Signature device:** a hand-drawn blue scribble circling one word of the H1 ("design").
- **Radius:** cards ~20px, insets ~14px, pills fully round.

## Page structure (top to bottom)

1. Sticky translucent nav: logo mark + name, center-left links (Features / Pricing / FAQs), right blue icon-link "Get Woblo".
2. Centered hero: mono proof line (`5 stars · 30,000+ developers`), huge two-line H1 with scribbled word, gray 18px lede, paired pill CTAs (gradient "add to chrome" with Chrome icon, outlined "try it live" with cursor icon).
3. Browser-chrome hero mock: dark window with blue gradient top edge, toolbar icons, page content on the left, dark extension panel on the right with tabs (Styles / Assets / Inspect / Design) and asset rows. Floating inspector chip (`img · 894 × 447 / hero-poster.png …`) overlapping the top-left of the mock.
4. Feature grid `Everything a page is made of.` — 3×2 white cards; each card is a gray inset **mini-mock of the feature itself** (inspector chip, swatches + contrast grade, type scale, asset chips, CSS var list, markdown snippet) above a bold title and gray one-liner.
5. Two wide "hover to open" cards with mono label and chip clouds: `Everything it reads` (asset types), `Everywhere it exports` (Tailwind v4, shadcn/ui, DTCG, CSS vars, SCSS, JSON, DESIGN.md, .zip).
6. Pricing `Inspecting is free. Forever.` — 3 white cards; the popular middle card has a gradient border glow and the gradient pill button; black tier chips; big `$N / month`; circle-check feature lists.
7. Testimonials `What people actually say.` — masonry of review cards (initial avatar, name, date, orange stars) mixed with dark social-embed cards, then a full-width blue-outlined pill bar: avatar stack + `5 ★★★★★ 42 reviews on the Chrome Web Store` + `Read them all ↗`.
8. FAQ `Questions? Answers.` — white accordion cards with circled `+`, closing line `Still stuck? Email us and a person will reply.`
9. Footer: gray band with logo/links/`© 2026`/"Get Woblo", then a giant **block-color wordmark** (each letter on a different saturated block: black, orange, green, pink, purple).
10. Persistent bottom-center floating pill `try woblo on this page`; fake multiplayer "guest" cursor label near the top.

## Behavior notes

- Sections reveal on scroll (fade/rise). Screenshots taken before a section enters the viewport render blank — scroll, wait ~3s, then capture.
- FAQ is a native accordion; only plus→x rotation animates.

## Substitutions in this study

| Source | Study ("Spectra") |
| --- | --- |
| Woblo brand, logo, Chrome Web Store links | Original "Spectra" name, CSS cursor-arrow logo mark, in-page anchors |
| Real copy, reviews, reviewer names, prices ($0/$7/$12) | Original copy, fictional reviewers, original prices ($0/$6/$10) |
| hero-poster video + product screenshots | Pure HTML/CSS browser mock with original placeholder content |
| Real Chrome Web Store rating (5 · 42 reviews) | Fictional 4.9 · 38 reviews |
| DESIGN.md export feature | Renamed SPEC.md with original snippet values |
| Inter + Geist Mono webfonts | System Inter/ui-sans and ui-monospace stacks |
| Blue scribble asset on "design" | Original inline SVG stroke circle |
| Block-color "woblo" footer wordmark | Block-color "spectra" footer wordmark |

## Comparison checklist

- [x] Sticky nav with blue icon CTA
- [x] Mono proof line over huge tight-tracked H1
- [x] Blue scribble on one headline word
- [x] Light-blue gradient pill + outlined pill CTAs
- [x] Dark browser-chrome hero mock with side panel and floating inspector chip
- [x] 3×2 feature cards with self-demonstrating gray insets
- [x] Two wide hover-to-open chip-cloud cards
- [x] 3-tier pricing with gradient-bordered popular plan
- [x] Testimonial masonry + avatar-stack rating bar
- [x] FAQ accordion cards + "Email us" closer
- [x] Gray footer band + giant block-color wordmark
- [x] Floating bottom-center pill CTA
