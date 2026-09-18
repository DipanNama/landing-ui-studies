# Reference notes: svg.guide

Source inspected: https://www.svg.guide/ on 2026-09-19 IST.

## Visual observations

- Near-monochrome palette: pale gray hero and curriculum fields, warm off-white content areas, black borders and controls.
- Oversized editorial serif headline, centered in a tall hero. On mobile it wraps to three compact lines.
- Small login link floats at the top right; the hero centers a compact author row and a pill-shaped two-button cluster.
- Technical ruler/tick details introduce the central SVG/course theme without a branded logo.
- Long editorial rhythm alternates plain narrative sections with bordered, interactive module showcases.
- Course modules are numbered with mono labels, large serif numerals, short teaching copy, code snippets, and interactive diagrams.
- Testimonials use a strict grid. Author, enrollment, and FAQ sections close the page with strong contrast and generous spacing.
- Typography mixes a dramatic high-contrast display serif, neutral sans-serif body text, and monospace labels/code.

## Responsive behavior checked

- Desktop: broad single-screen hero, headline reaches roughly 10vw, curriculum modules use side-by-side copy and demos.
- 390px mobile: hero becomes about 540px tall; headline uses three lines; intro, modules, testimonial grid, and author section become one column.
- Buttons remain grouped in one pill and body copy keeps comfortable 24px side gutters.

## Original-study substitutions

- Replaced the source course title, teacher identity, portrait, testimonials, module copy, pricing, and external links.
- Authored every visible diagram locally with HTML/CSS/SVG primitives.
- Used system/local font fallbacks instead of copying the source font files.
- Preserved only transferable design ideas: layout rhythm, scale contrast, borders, neutral palette, technical annotations, and responsive structure.

## Visual comparison checklist

- [ ] Hero scale and vertical centering feel editorial rather than app-like.
- [ ] Display serif remains readable and does not overflow at 390px.
- [ ] Pill actions keep clear primary/secondary hierarchy.
- [ ] Module demos are visible without proprietary imagery.
- [ ] Border/grid rhythm stays crisp in both themes and widths.
- [ ] Reduced-motion preference disables decorative animation.
