---
name: handdrawn-illustration-pack-landing
version: 1.0.0
source-study: https://www.notioly.com/
scope: illustration packs, icon libraries, font or asset shops, and other single-product creative marketplaces
---

# Hand-drawn illustration pack landing design skill

Use this skill for an original single-product page that sells a visual asset library. The design works because it gets out of the way: the artwork carries the page, and everything else is quiet monochrome type. Reuse the composition logic, never the reference brand, artwork, copy, or assets.

## Visual thesis

A gallery wearing a landing page. Keep the entire page black-on-white with zero decorative color so the line art reads as the product. Confidence comes from restraint: one heavy headline, one grid of artwork, one dark panel at the end.

## Tokens

```css
--paper: #fafafa;
--card: #ffffff;
--ink: #09090b;
--ink-soft: #18181b;
--muted: #585860;
--faint: #8b8b93;
--line: #e7e7e4;
--wash: #f4f4f3;
--dark: #0a0a0b;
--dark-pill: #26262b;
--radius-card: 16-18px;
--radius-panel: 24-26px;
--radius-pill: 999px;
--space: 4, 8, 12, 16, 24, 32, 48, 64, 88, 110px;
```

## Typography

- Display: extra-heavy grotesk (800-900), `clamp(2.6rem, 5.4vw, 3.5rem)`, line-height ~1.08, slight negative tracking. Archivo Black / Arial Black system fallbacks are acceptable.
- Section heading: same face, `clamp(1.9rem, 3.6vw, 2.5rem)`.
- Body: 15.5-18px system sans, mid-gray, hero lede capped near 56ch.
- Byline accent: one script or italic face for the maker's name only. Never use script anywhere else.
- No uppercase eyebrow labels on this pattern; the announcement chip carries the news.

## Layout

- Content max-width ~1200px with 32px desktop and 22px mobile gutters.
- Header is a single quiet row (~84px): brand mark left, links and purchase pill right.
- Hero is centered and compact: chip, headline (~15ch max), one-line lede, maker byline. Total under ~460px tall.
- The gallery follows immediately; it is the hero's proof, not a later section.
- Generous vertical rhythm: ~110px between major sections.
- Footer is one row: copyright left, links right.

## Signature components

### Announcement chip
Small white pill with a 1px border, 13-14px text, one emoji or sparkle. It announces freshness (new additions this month), which is the library's main promise.

### Maker byline
Tiny round avatar plus a script-font name. This personalizes the pack and signals hand-made origin. Keep it under the lede, centered.

### Artwork grid
4 columns desktop, 2 tablet, 1 mobile; 20-24px gaps. Cards are white with a hairline border, 16-18px radius, ~4/3.4 aspect, artwork centered with ~26px padding. No captions, prices, or buttons on cards. A subtle 4px hover lift is the only motion.

### Full-width ghost button
One light-gray pill spanning the grid's width directly below it, labeled with the full library size. It behaves as "view all", not as the sales CTA.

### Text-only feature trio
Three columns: small line icon, bold 18px title, two-line gray paragraph. Themes: always growing, works everywhere, fully editable. A single small sparkle mark above the section heading.

### Inset dark panel
The only dark surface on the page: 24-26px radius, ~90px vertical padding, small line flourish, white heavy headline, paired pills (white primary with price, dark-gray secondary for the free sample), one quiet social-proof line with a tiny badge.

## Art direction for substitute artwork

- Draw original inline SVG: 2.5-3px round-capped black strokes on white, minimal fills.
- Everyday, warm subjects (bicycle, plant, coffee, pet, letter) over abstract tech shapes.
- One consistent stroke width across the whole set; tiny motion dashes or sparkles as accents.
- Never trace, recreate, or closely imitate the source pack's actual drawings.

## Motion

- Hover lift only: 4px over ~200ms on cards and buttons.
- No marquees, parallax, autoplay, or scroll-triggered animation.
- Respect `prefers-reduced-motion`.

## Responsive rules

Below 640px: hide nav links behind a hamburger affordance, recompose the headline to ~40px, single-column gallery, stack features, make CTA buttons full width, stack the footer centered. Nothing may exceed 390px without horizontal scrolling.

## Build procedure

1. Draft 6-8 original SVG drawings first; the grid quality decides the page.
2. Build header, hero, grid, ghost button, features, dark panel, footer in that order.
3. Keep every asset inline; the study must be a single self-contained HTML file.
4. Verify at 1280px and 390px: grid columns, CTA button stacking, footer stacking, no overflow.

## Quality gates

- [ ] Page reads black-on-white; the only dark surface is the final panel.
- [ ] Headline weight 800+ and centered hero with chip and script byline.
- [ ] Grid is caption-free; artwork is original inline SVG with one stroke width.
- [ ] Purchase pill includes the price in its label; free-sample pill sits beside it.
- [ ] 390px: hamburger header, one-column grid, full-width CTA pair, no horizontal scroll.
