---
name: midnight-docs-landing
version: 1.0.0
source-study: https://www.fumadocs.dev/
scope: documentation tools, developer SDKs, CLIs, and technical open-source product landing pages
---

# Midnight docs landing design skill

Use this skill for an original developer-tool page that feels nocturnal, crafted, and engineer-credible. Reuse the composition logic, not the reference brand, copy, artwork, testimonials, or product screens.

## Visual thesis

A near-black canvas lit by dithered warm light. The page earns its darkness: thin borders, quiet panels, one cream accent, and halftone dot-raster artwork (orbs, a moon) that gives the darkness texture. Code is the hero's supporting actor, always present, always legible.

## Tokens

```css
--bg: #0a0a09;           /* near-black canvas */
--panel: #131311;        /* cards, nav pills */
--panel-2: #191916;      /* raised controls */
--line: #27271f;         /* warm hairline borders */
--fg: #f3f2e9;           /* warm off-white ink */
--muted: #a09e8d;
--faint: #6f6d60;
--cream: #f5f39d;        /* primary accent: buttons, accent words, labels */
--cream-ink: #191910;    /* text on cream */
--orange: #ff6a3d;       /* single gradient panel accent */
--orange-deep: #e04e22;
--radius-pill: 999px;
--radius-card: 16-18px;
--space: 4, 8, 12, 16, 24, 32, 44, 56, 72, 96px;
```

## Typography

- Display: modern grotesk, 600-650 weight, `clamp(2.6rem, 6.4vw, 4.6rem)`, line-height 1.06, tracking -0.02em.
- Section headings: `clamp(2rem, 4.6vw, 3.2rem)`, often set in the cream accent on black.
- Mono voice: eyebrows, CLI text, and one banner headline in `ui-monospace`, uppercase eyebrows at 12px with 0.2em tracking.
- Body: 15-16px, 1.55-1.6, warm gray, max 56ch.
- Use a system sans if a suitable licensed grotesk is unavailable.

## Layout

- Content max-width 1180px with 24px gutters (20px mobile).
- Sticky blurred nav, 64px. Hero padding 96px top, app mock anchored to hero bottom edge.
- Section padding 96px desktop, 72px mobile.
- Alternating compositions: full-width centered statements, two-column card rows, split code+copy rows.
- Grids collapse to one column under 820px; CTAs stack full-width; sidebars inside product mocks hide.

## Signature components

### Halftone atmosphere
Build orbs and moons from radial gradients (amber to ember to olive) clipped by a repeating dot mask (`mask-image: radial-gradient(circle, #000 1px, transparent 1.35px); mask-size: 4px 4px`). Keep them behind content, never under body copy.

### Hero stack
Outlined cream pill tag, oversized headline with 1-3 accent words in cream, paired pill CTAs (primary cream with dark ink, secondary dark panel with hairline border), then a product-app mock touching the fold.

### Product-app mock
A docs interface with sidebar (search field, grouped nav, active item tinted cream) and content pane (crumb line, mini action buttons, intro copy). It proves the product is real without a screenshot.

### Try-it-out terminal
Mono eyebrow, a copyable `pnpm create` command bar, then a terminal panel floating over a dithered field. Show a CLI prompt flow (project name, framework picker) and a small success toast ("localhost:3000 / app launched").

### Testimonial marquee on orange
One vivid orange gradient panel with a subtle dark dot texture, containing an infinite horizontal marquee of dark quote cards with avatar initials, names, and roles. Duplicate the row for a seamless loop; pause on hover.

### Split code storytelling
Alternate sides: a dark code card (syntax colors: violet keywords, green strings, cream functions, gray comments) against copy with a cream-bulleted feature list or a stack of composable layer rows (`package-name` chip + description + layer tag).

### Moon banner
A mono uppercase headline over a short lowercase mono tagline, with a giant halftone moon rising from the bottom edge of the panel. This is the emotional peak before the close.

### Final promise card
Three icon-led one-line promises (maintained, open-source, fast setup) with square hairline icon tiles, then the same paired pill CTAs as the hero.

## Motion

- Marquee: 30-40s linear infinite, pause on hover.
- Buttons: 1px lift on hover, 150ms.
- Nothing else moves; stillness is part of the tone.

## Responsive rules

- Under 820px: hide nav links and the search pill, show a hamburger; center the hero; stack CTAs; collapse all grids and splits; hide mock sidebars; scale the moon and orbs down, never crop text.

## Build procedure

1. Set the dark token set and hairline borders first; get panels readable on the canvas.
2. Compose the hero stack and app mock; verify the fold at 1280x720 and 390x844.
3. Add the dithered atmosphere last, checking contrast after each orb.
4. Build the terminal and marquee, then the split rows and banners.
5. Finish with the promise card and a quiet footer.

## Quality gates

- Cream accent passes contrast on black; cream buttons use dark ink.
- No horizontal overflow at 390px; the marquee never stretches the page.
- Every code sample is syntactically plausible and fully original.
- All artwork is CSS-generated; no external images, fonts, or brand assets.
- The page reads top to bottom as one story: promise, proof, craft, community, close.
