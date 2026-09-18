# Dark Framed Developer-Tool Landing

Use this skill to design an original landing page for a build tool, framework, runtime, SDK or developer platform. It captures a visual method, not any source brand.

## Design intent

Make the product feel fast, exact and infrastructure-grade. The interface should read as a technical instrument: dark surfaces, fine structural lines, compact controls, one energetic spectral accent and generous breathing room.

## System

- Canvas: near-black `#121318`; inset panels `#16171d`; terminal surfaces `#0f1015`.
- Text: warm white `#f7f7fa`; supporting copy `#a6a7b1`.
- Dividers: cool gray `#30313a`, always 1px.
- Accent: purple led gradient with blue/orange edges. Use on one hero object, focus borders and tiny active indicators.
- Type: neutral system sans for interface and editorial copy; monospace for labels, commands and metadata.
- Radius: 8-14px. Avoid soft pill shapes except tags.
- Width: cap the page around 1,400px and expose the outer frame lines.

## Composition

1. Optional 36-42px announcement strip with a dark spectral gradient.
2. 72-80px utility navigation with a compact wordmark and quiet controls.
3. Split hero on desktop. Copy and terminal occupy one half; abstract product object occupies the other.
4. A trust strip follows immediately, then a large centered section statement.
5. Benefits live in a 2x2 bordered grid. Give every card a technical, locally drawn visual.
6. Follow with a tool/framework matrix, community proof, and a single final CTA.
7. Keep vertical section spacing between 96 and 120px on desktop.

## Hero rules

- Heading: 56-68px desktop, 36-42px mobile, line-height near 1.03, strong negative tracking.
- Description: 18-20px, muted, no more than three lines at desktop.
- Primary action uses an accent outline and subtle outer glow. Secondary action is neutral.
- The terminal is part of the composition rather than a floating demo card. Provide 3-5 package-manager tabs and one live command row.
- Use CSS geometry, gradients, grids or generated local artwork for the hero. Do not import a reference product's mark.

## Responsive behavior

At 720px or below:
- Hide the announcement unless it contains critical information.
- Reduce navigation to wordmark plus 1-2 controls.
- Stack hero copy over hero art and center the text.
- Hide or simplify the terminal when it competes with the hero object.
- Convert paired grids to one column.
- Turn testimonial grids into horizontal, scroll-snapping cards.
- Let logo rows become a masked or clipped marquee.

## Interaction

- Package-manager tabs update the visible command without moving layout.
- Announcement dismissal removes its space.
- Add smooth in-page navigation.
- Motion should suggest transfer or compilation: a line sweep, pulse or orbit. Respect `prefers-reduced-motion` in production work.

## Avoid

- Large undifferentiated purple gradients.
- Glass cards everywhere.
- Bright filled primary buttons that overpower the hero object.
- Copied brand marks, source testimonials, partner logos or source copy.
- More than one decorative visual language. Pick lines plus one geometric object and stay consistent.

## QA checklist

- Check at 1280px and 390px widths.
- Confirm frame borders align and do not double to 2px.
- Ensure heading wraps intentionally at both widths.
- Test package tabs, close control, navigation and CTA links.
- Ensure horizontal mobile scrollers do not create page-level overflow.
- Inspect actual pixels for contrast, crop, spacing and z-order before delivery.
