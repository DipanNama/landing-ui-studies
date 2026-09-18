# Design Skill: Editorial Interactive Course

Use this skill to build an original learning-product landing page that feels tactile, technical, and editorial.

## Core idea

Pair oversized editorial typography with tiny technical details and live examples. The page should make the subject visible before explaining it. Alternate calm reading space with structured interactive modules.

## System

### Color
- Canvas: `#fafafa`
- Feature field: `#f0f0f0`
- Ink: `#141414`
- Muted text: `#676767`
- Hairline: `#202020` at full strength or `#bbb` for secondary dividers
- Inverse field: `#171717` with `#f6f6f3` text
- Keep accent color inside code syntax or teaching diagrams, not global chrome.

### Type
- Display: high-contrast editorial serif, normal weight, tight tracking around `-0.04em` to `-0.06em`.
- Body: neutral sans serif, 16-19px, line-height 1.6-1.7.
- Technical labels: 12-14px monospace, uppercase where useful, loose letter spacing.
- Let the display face create drama. Do not add decorative gradients or shadows to headings.

### Layout
- Maximum content width: 1160px; reading width: 650-760px.
- Hero: 540-700px tall, centered title, author detail, and compact actions.
- Reading sections: 70-110px vertical padding.
- Curriculum: numbered rows with a narrow index column, teaching copy, and a live demo.
- Switch two-column structures to one column below 760px.
- Use 24px mobile gutters.

### Components
1. **Technical hero**: tiny utility link, oversized 2-3 line title, compact byline, paired pill actions, ruler/tick detail.
2. **Editorial intro**: a short serif thesis opposite plain-spoken body copy.
3. **Module row**: mono label + large numeral, a lesson title and summary, then a bordered diagram or code panel.
4. **Live demo**: use native CSS/SVG geometry. It must communicate the topic even when motion is disabled.
5. **Testimonial grid**: equal bordered cells, large serif quote, small sans attribution.
6. **Inverse author section**: one simple original portrait substitute plus direct personal copy.
7. **Enrollment card**: concise inclusion list, clearly separated price/action row.
8. **FAQ**: native `details` elements with strong horizontal dividers.

## Interaction
- Use slow, legible 3-4 second loops for examples, not ambient decoration.
- Keep actions underlined by structure: border, fill, and weight. Avoid oversized glowing buttons.
- Add `prefers-reduced-motion` support and ensure static demos remain meaningful.
- Use native elements for keyboard and screen-reader behavior.

## Mobile rules
- Clamp the headline and explicitly test at 390px.
- Preserve the two-button pill when labels fit; shorten labels rather than stacking prematurely.
- Number and label can share one line; lesson content and demo stack.
- Test all diagrams in a 230px-high panel and prevent horizontal scroll.
- Keep quote cards one per row.

## Build checklist
- Original copy, identities, testimonials, geometry, and imagery only.
- No source logo, portrait, font files, or screenshots.
- One semantic `h1`, ordered headings, useful SVG labels, and visible focus states.
- No dependency is required for the base experience.
- Verify the top, at least one curriculum row, testimonials, and conversion section at desktop and mobile widths.
