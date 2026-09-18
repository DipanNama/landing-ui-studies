---
name: product-craft-dark-landing
summary: Build a calm, high-craft dark landing page for a serious product-development or workflow tool.
---

# Product Craft Dark Landing

Use this skill for products that need to feel fast, opinionated, technically credible, and premium without looking loud.

## Core idea

Treat the actual product interface as the strongest visual asset. Marketing hierarchy should create space around credible workflow scenes, not compete with them.

## Build sequence

1. Start with a restrained 64–72px navigation. Keep secondary actions quiet and make one conversion action unmistakable.
2. Write a short category claim as the hero. Keep it within two lines on desktop and support it with one sentence describing the operating benefit.
3. Place a large CSS-authored product scene below the hero. Show realistic density, hierarchy, status, and work states. Avoid generic gradient dashboards.
4. Add a low-key customer or trust strip.
5. State the product philosophy in one large editorial sentence, then split it into three principles.
6. Build two or three feature sections. Pair focused copy with purpose-built interface scenes rather than screenshots repeated in identical cards.
7. Add current product updates to signal momentum.
8. Close with one strong proof point and a simple call to action.

## Tokens

```css
--background: #090a0b;
--surface: #111214;
--surface-raised: #151619;
--line: rgba(255,255,255,.09);
--text: #f7f7f8;
--text-secondary: rgba(255,255,255,.58);
--text-muted: rgba(255,255,255,.38);
--signal: #7b7cff;
--radius-control: 8px;
--radius-frame: 16px;
```

Use one signal hue and no more than two functional companions. The accent should occupy less than 8% of the visible page.

## Typography

- Use a clean system sans or neutral grotesk.
- Hero: 48–84px, 0.98–1.02 line height, -0.045em to -0.065em tracking, 550–620 weight.
- Section statement: 36–60px, about 1.08 line height.
- Body: 15–18px, 1.5–1.65 line height.
- Interface text: 10–13px.
- Create hierarchy with scale and opacity, not many font weights.

## Surfaces and depth

- Use one-pixel translucent borders on dark surfaces.
- Add depth with subtle radial glow behind the hero product, never a bright neon cloud.
- A fine grain layer can prevent large black fields from looking synthetic.
- Keep shadows broad, dark, and low contrast.
- Product scenes need nested panel values so their hierarchy reads before their labels do.

## Product-scene rules

- Invent plausible IDs, labels, statuses, owners, and progress data.
- Show one main workflow per scene.
- Use dense information with strong alignment and generous outer framing.
- A product frame can crop on mobile. Do not scale it until its labels become useless.
- Avoid copied screenshots, logos, customer names, testimonial wording, or proprietary assets.

## Responsive rules

At 760px or below:

- Collapse full navigation into brand, primary action, and menu affordance.
- Stack hero actions and keep tap targets at least 42px high.
- Convert split features and three-column content to one column.
- Crop complex product visuals within an overflow-hidden frame.
- Reduce outer gutters to 15–20px while keeping section spacing at 72–90px.
- Preserve the dramatic headline contrast rather than shrinking every element proportionally.

## Interaction

- Keep motion restrained: soft hover borders, subtle surface lift, and eased scrolling.
- Avoid autoplay carousels, constant floating, or decorative cursor effects.
- Honor reduced-motion preferences if adding animation.

## Quality checks

- The hero communicates category and benefit without the mockup.
- The app scene looks usable at a glance and contains no placeholder lorem ipsum.
- Accent color does not dominate the monochrome foundation.
- Mobile typography has no clipping or horizontal page overflow.
- Every large visual is local or CSS-authored.
- The page still has rhythm when viewed as a long screenshot.
