# DESIGN SKILL — Light Tool-SaaS Landing ("self-demonstrating product page")

Reusable system for landing pages of small browser tools, extensions and dev utilities, derived from studying woblo.in. The core idea: **the page demonstrates the product instead of describing it** — every feature card contains a tiny working mock of the feature, and the hero shows the product UI inside a browser frame.

## When to use

- Browser extensions, DevTools-adjacent utilities, inspectors, exporters, CLI-with-GUI products.
- Products whose value is "see exactly what you'll get" — the page itself becomes the demo.
- Light, friendly, craft-forward tone (not enterprise, not dark/glowy).

## Tokens

```css
--bg: #fbfbfb;          /* near-white page */
--ink: #101013;         /* headings + body */
--muted: #5f6470;       /* secondary text */
--faint: #8a8f9c;       /* micro-labels */
--line: #e9e9ee;        /* hairline borders */
--card: #ffffff;
--inset: #f4f4f7;       /* gray demo areas inside cards */
--accent: #0f7fff;      /* blue; links, icon CTAs, scribble */
--radius-card: 20px;
--radius-inset: 14px;
/* pills: border-radius: 999px */
```

Primary CTA gradient (light, glossy, black text — never white text on dark blue here):

```css
background: linear-gradient(#edf4ff 0%, #d6e7ff 18%, #a2c7ff 50%, #99cbf8 80%, #a2d2f7 100%);
border: 1px solid #b9d6fb;
box-shadow: 0 1px 2px rgba(15,127,255,.25), inset 0 1px 0 rgba(255,255,255,.7);
```

Popular-plan border (gradient border trick):

```css
border: 1.5px solid transparent;
background: linear-gradient(#fff,#fff) padding-box,
            linear-gradient(120deg,#2f6bff,#8a5cf6,#ff7a59) border-box;
```

## Typography

- Sans: Inter or the system-ui stack. Mono: Geist Mono or ui-monospace stack.
- H1: `clamp(38px, 6.2vw, 64px)`, weight **500** (not bold), letter-spacing **-0.03em**, line-height 1.1, max-width ~14ch, centered.
- Section H2: `clamp(30px, 4.4vw, 44px)`, same tracking/weight.
- Micro-labels (proof lines, "hover to open", dimension chips): mono, 11–13px, gray; numbers/counts in the ink color.
- Card titles 17px/600, card body 14.5px muted, section lede 17–18px muted centered, max ~52ch.

## Signature devices (pick at least two)

1. **Scribble word.** Circle or underline one word of the H1 with a rough hand-drawn SVG stroke in the accent color (absolute-positioned SVG over an inline-block span, `overflow: visible`, ~4.5px round-cap stroke).
2. **Self-demonstrating feature cards.** Each card's gray inset is a miniature of the feature: a button with a size tag, swatches with a contrast-grade chip, an `Aa` type scale, file-type chips, a CSS-variable list, a markdown snippet. The inset is the pitch; the title just names it.
3. **Browser-chrome hero.** A CSS-only browser window (dark toolbar, dots, URL pill) containing the product panel next to fake page content; one floating "inspector chip" overlapping its edge with a mono dimension tag (`img · 894 × 447`).
4. **Block-color footer wordmark.** The product name as huge letters, each on a different saturated block (black, orange, green, pink, purple, blue), flush to the bottom edge, border-radius only on the top corners.
5. **Floating pill CTA.** A fixed bottom-center pill ("try it on this page") with a cursor-arrow icon; optional fake multiplayer cursor label ("guest") floating nearby.

## Layout recipe

1. Sticky translucent nav (blur, hairline bottom border): logo mark + name left, 3 text links, blue icon-link CTA right.
2. Centered hero: mono proof line → H1 with scribble → lede → paired pills (gradient primary + outlined ghost) → browser mock.
3. `H2 + one-line sub` centered, then a 3×2 grid of self-demonstrating cards.
4. Two wide "hover to open" chip-cloud cards (what it reads / where it exports).
5. Pricing: 3 cards, popular middle with gradient border + gradient button; black tier chips; `$N / month` at 44px; circle-check lists (black circle, white check).
6. Testimonials: CSS-columns masonry mixing white review cards (initial avatar, name, date, orange stars) with dark social-post cards; close with a full-width pill bar: avatar stack, rating number, stars, "N reviews", arrow link.
7. FAQ: white accordion cards, circled `+` that rotates 45° when open; end with "Still stuck? Email us…".
8. Footer: gray band, logo/links/copyright/CTA row, then the block-color wordmark.

## Motion

- Scroll-reveal only: fade + 12–20px rise per section, staggered cards. Nothing parallax, nothing continuous.
- Hover: border darkens on cards; accordion plus rotates. Respect `prefers-reduced-motion`.

## Responsive rules

- ≤900px: feature grid 3→2 columns, pricing stacks, hero browser mock drops its side panel (page content only) and the inspector chip hides.
- ≤620px: nav links hide (logo + CTA only), grids 1 column, masonry 1 column, section padding ~76px, H1 via the clamp's low end, rating bar wraps.
- The footer wordmark scales with viewport-width units; letters never wrap.

## Build procedure

1. Single self-contained `index.html`; inline CSS; system font stacks; inline SVG for icons (cursor arrow, circle-chrome dot, checks).
2. Build the browser mock in pure HTML/CSS — no screenshots.
3. Keep all copy, names, prices, reviews and metrics original. Parallel the *structure* of any reference, never its text or assets.
4. Verify: no horizontal overflow at 1280px and 390px; accordion opens; floating pill doesn't cover footer links at short viewport heights.

## Quality gates

- Headline reads at a glance from 2 meters: one short sentence, one scribbled word.
- Every feature card could be screenshotted alone and still explain the feature.
- Exactly one gradient-bordered element on the page (the popular plan).
- Mono is used only for micro-labels and data, never for prose.
