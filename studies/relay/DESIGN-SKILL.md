---
name: dark-developer-infrastructure-landing
description: "Build a premium dark landing page for a developer tool or API product: black canvas, giant serif display hero paired with grotesk section headings, 3D-look CSS visuals, framework-tabbed code windows, product-UI mockups as feature proof, tinted status pills, and a cropped giant wordmark above the footer. Use when a dev-tool, API, SaaS-infrastructure, or B2D product needs a marketing page in this style."
---

# Dark developer-infrastructure landing

A design system distilled from studying a best-in-class email-API landing page. The
pattern: restraint everywhere, spectacle in exactly three places (hero visual, gradient
accents, product mockups).

## When to use

- Marketing site for a developer tool, API, SDK, CLI, or infrastructure product.
- The audience is engineers: proof beats adjectives — show the code, show the UI.

## Non-negotiables

1. **Pure black canvas** (`#000`), not dark gray. All elevation comes from hairline
   borders (white at 5-8%) and barely-lifted panels (#0a0a0b-#141416), never from
   shadows on the background itself.
2. **Two-typeface tension**: a sharp serif for the hero + final CTA display only
   (96px desktop / 64px mobile, tight -1% tracking, weight 400), a neutral grotesk for
   everything else. Section H2: 56px/67px, -2.8px tracking, weight 400 — never bold.
   Code always in a mono face at ~13.5px with line numbers.
3. **One accent system**: a violet→blue→teal gradient used ONLY for: one phrase in a
   section heading, thin gradient borders on announcement pills/icon tiles, small glows.
   Status colors (green/red/amber) only as 12%-alpha tinted pills with full-strength text.
4. **Restrained chrome**: 48px pill buttons, radius 16px, dark fill + 2px 5%-white border,
   600-weight 16px label. One white button max per page (inside a mockup).
5. **Product UI as content**: feature sections show believable interface mockups (code
   editor with framework tabs, email editor, dashboard with sidebar + metric cards +
   line chart) — hand-built in HTML/CSS, denser and darker than the page around them.
6. **The white canvas beat**: place one stark white surface inside the dark UI (the email
   body being composed, the rendered email preview). It photographs the product instantly.
7. **Ending ritual**: giant serif two-line CTA, single dark pill, then an oversized
   near-black wordmark (#0d0d0f) cropped by the footer top edge. Footer carries address,
   social icon circles, a live status pill (green dot, pulse), and 4-5 link columns.

## Layout grammar

- Container ~1152px, sections breathe (100-140px vertical padding).
- Hero: text left / 3D visual right on desktop; visual stacks above centered copy on mobile.
- Pair feature cards at 2-up, visuals on top (300px) + text below; grids of small features
  go 3x3 inside one bordered container.
- Every visual block gets a reveal-on-scroll (24px rise, 700ms, cubic-bezier(.2,.6,.2,1)).
- Mobile: hamburger nav, horizontal scroll strips (SDK icons, testimonial cards) with a
  thin 4px scrollbar, sidebars collapse to icon rails.

## Implementation notes

- Fake the 3D hero object with CSS `preserve-3d`: three faces of a 3x3 tile grid
  (rotateX(-28deg) rotateY(42deg)), glossy inset gradients, slow float keyframes, and a
  blurred radial "floor" reflection. No WebGL needed.
- Gradient border pill: `border:1px solid transparent; background-clip:padding-box` plus a
  conic-gradient pseudo-element masked to the border ring.
- Line-numbered code: CSS counter on block-level spans, not a table.
- Dashboard chart: inline SVG path + `linearGradient` area fill + one dashed gridline.
- Keep every mockup's data internally consistent (the "Delivered 29,486" rows should match
  the chart's headline number) — engineers notice.
- Fonts: Inter (sans) + Instrument Serif (display) + JetBrains Mono (code) are free
  stand-ins for the commercial ABC Favorit / Domaine / Commit Mono stack.

## Anti-patterns

- No colored backgrounds, no light mode, no big border-radius blobs.
- No emoji or stock photos. Icons are 1.5-1.8px-stroke inline SVGs.
- No bold display type; weight 400 with tight tracking does the work.
- Don't stack multiple gradient accents in one viewport — one per section.
