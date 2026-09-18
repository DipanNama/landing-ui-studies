---
name: adaptive-product-story-landing
version: 1.0.0
source-study: https://croct.com/
scope: optimization, personalization, analytics, CMS, and developer SaaS landing pages
---

# Adaptive product story landing design skill

Use this skill for an original SaaS page that feels optimistic, technically credible, and product-led. Reuse the composition logic, not the reference brand, copy, assets, customer marks, or product screens.

## Visual thesis

Pair a nearly white canvas with soft lavender and mint light. The page should feel precise rather than sterile: large rounded type, pill actions, thin borders, and one rich product scene that explains the promise before the feature grid begins.

## Tokens

```css
--ink: #111a2e;
--muted: #63738f;
--line: #e3e9f2;
--paper: #ffffff;
--soft: #f7f7ff;
--lavender: #7b79f6;
--mint: #4dd684;
--radius-control: 999px;
--radius-card: 22-28px;
--space: 4, 8, 12, 16, 24, 32, 48, 64, 80, 108px;
```

## Typography

- Display: rounded geometric sans, 600-650, `clamp(2.75rem, 6vw, 4.5rem)`, line-height 1.07, tracking -0.05em.
- Section heading: `clamp(2.25rem, 4.5vw, 3.375rem)`, line-height 1.1.
- Body: 16-19px, 1.55, slate gray, no more than 70 characters wide.
- Eyebrow: 12-13px, 700, uppercase, 0.04em tracking, lavender.
- Use a system sans if a suitable licensed display face is unavailable.

## Layout

- Content max-width 1120px with 24px desktop and 20px mobile gutters.
- Announcement strip: 36-42px. Navigation: 78-88px.
- Hero content max-width 900px. Supporting copy max-width 780px.
- Product scene max-width 980px and placed 64-80px below the CTAs.
- Standard section padding: 96-112px desktop and 72-84px mobile.
- Use pale full-width section bands to reset rhythm.

## Signature components

### Atmospheric hero
Use two large radial gradients at opposite edges. They should be barely visible and must never reduce text contrast. Apply a lavender gradient to only the promise line, leaving the outcome line navy.

### Product stage
Build a browser shell with a quiet URL bar. Inside, pair the adapted content with a visitor profile or activity timeline. The scene needs to explain cause and effect without relying on a screenshot.

### CTA pairing
Primary action is a navy pill with white text. Secondary action is white with a thin cool-gray border. Add one short reassurance below. On mobile, stack both at full width.

### Feature cards
Use three columns, thin borders, 22-28px radii, and almost no shadow at rest. Every card gets one small tinted icon tile and one locally drawn mini product visualization.

### Developer proof
Use a 50/50 split. Place a plain-language value statement beside a dark code panel with one lavender and one mint syntax accent.

### Final action
Use a rounded inset navy panel rather than a full-bleed footer. Add a subtle lavender radial glow and invert the primary action to white.

## Motion

- Hover lift: 4px over 180-220ms.
- Product-scene state changes may cross-fade over 250ms.
- Avoid marquees, parallax, autoplay media, and constant decorative motion.
- Respect `prefers-reduced-motion`.

## Responsive rules

Below 760px: hide full nav, use a menu affordance, remove announcement strip, stack CTA pair, reduce headline to 40-46px, turn feature grids and split sections into one column, and hide the secondary panel in the hero demo. Keep every visual inside 390px without horizontal scrolling.

## Build procedure

1. Write the promise as an action plus a human outcome.
2. Design the hero and product stage as one narrative.
3. Add audience/activity detail to explain why content changed.
4. Map three core abilities into a restrained card row.
5. Add implementation proof for technical confidence.
6. End with one low-friction action in a dark inset panel.
7. Test at 1280x720 and 390x844 using actual pixels.
8. Check contrast, focus states, 44px targets, overflow, reduced motion, and useful alt text.

## Quality gates

Reject the page if its gradients are loud, every section uses cards, the product scene is decorative, copy uses vague claims, or the mobile layout merely shrinks the desktop. The result should remain understandable with all brand color removed.
