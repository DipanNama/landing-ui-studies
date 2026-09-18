# Component-Library Storefront Landing

Use this skill for a component-library or design-system product page that must prove breadth (many components) and trust (pricing, testimonials, docs) on one long white page.

## Core recipe

1. Keep a white canvas, hairline borders, and one violet/purple accent that carries eyebrows, primary buttons, checks, and inline highlights. Do not add a second accent.
2. Sticky slim header: gradient square mark + wordmark left, short text nav, ghost + primary buttons right; hamburger only on mobile.
3. Hero on a faint dot grid: small black glyph tile, purple eyebrow, 56-64px tight headline, two-line gray sub, three-button row (two ghost with icons, one primary). Proof is two overlapping app windows with a negative-margin stack and a small accent name-tag chip.
4. Prove breadth with a 4-column card grid: light preview panel with a tiny CSS-drawn component mock on top, bold name + muted variant count below. Close with one centered ghost button.
5. Break the page rhythm with large rounded panels (24px radius, #f9fafb) for the video section and the FAQ accordion.
6. Include a 2x2 feature grid (icon tile, title, paragraph, text link) and a "built with" hairline divider followed by 4 stack cards; repeat the hero CTA trio after them.
7. Show the CLI as real mono terminal boxes (command box + interactive-prompt box) beside a starter-kit card grid.
8. Show theming with a side-by-side light/dark panel pair rendering identical mini widgets.
9. Pricing tiers: big price figure, small-caps tag, muted description, circled-check feature list (gray minus rows for excluded items), full-width button; accent border + shadow on the featured tier.
10. Wall of love: amber star row, quote with one accent-highlighted phrase, avatar + name + role.
11. Footer: sitemap columns with accent-colored column heads, badge chips, legal row, and a giant ultra-light wordmark cropped at the bottom.

## Tokens

- Canvas: `#ffffff`; panels: `#f9fafb`; hairlines: `#eaecf0`
- Text: `#101828`; secondary: `#667085`; faint: `#98a2b3`
- Accent: `#6c4cf6` (hover `#5a3ee0`; soft chip `#f4f1ff`)
- Stars: `#f79009`
- Radius: 12px cards, 16px panels/pricing, 24px feature panels, 9px buttons
- Type: tight sans stack ("Inter", system); display 60px desktop / 38px mobile at -0.03em
- Mono: ui-monospace stack for terminal blocks
- Hero texture: `radial-gradient(#e9e9f2 1.15px, transparent 1.15px)` at 22px size

## Responsive rules

- Collapse nav to a hamburger and stack hero CTAs full width below 768px.
- 4-col grids go to 2 at 1024px and 1 at 520px; pricing and testimonials go single column at 1024px.
- Hide decorative overlaps that get cramped (name-tag chip, long breadcrumbs) on small screens; shorten the negative hero overlap to about -40px.
- Keep side gutters at 24px and section padding near 88px desktop / 64px mobile.
- The giant footer wordmark needs `overflow:hidden` and `max-width:100%` so it never creates horizontal scroll.

## Avoid

- Copying a real library's name, logo, component screenshots, testimonials, prices, or version claims.
- More than one accent color; gradients across large surfaces.
- Image-heavy previews: draw component mocks in CSS/SVG so the page stays self-contained.
- Carousels, autoplay video, or animation-heavy sections; this layout wins on density and calm.
