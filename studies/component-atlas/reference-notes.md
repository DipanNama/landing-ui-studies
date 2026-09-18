# Untitled UI React reference notes

Source observed: https://www.untitledui.com/react on September 19, 2026 (IST), live in the cloud browser.

## Page structure

- Sticky white header (~64px): gradient square mark + wordmark at left, six text nav links, ghost "Sign in" and purple primary button at right. Mobile collapses to mark + hamburger.
- Centered hero on a dot-grid canvas: small black rounded-square glyph tile, purple eyebrow, oversized tight-tracked headline, gray two-line subcopy, then a three-button row (two ghost buttons with icons + one purple). Mobile stacks all three buttons full width.
- Hero proof is two overlapping docs-app windows (sidebar + article, then a component-page window) built from real product screenshots on the source. A purple name-tag chip with a tiny caret floats beside the lower window. The second window overlaps the first with a negative top margin.
- Component grid: eyebrow, centered H2, subcopy, a "Built with X and styled with Y" line with mini brand marks, then a 4-column card grid. Each card is a light-gray preview panel with a small UI mock (avatars, footers, calendars, charts, date pickers, color spectrum, command menu, buttons, modals, badges, sliders, landing-page examples) over a footer row with bold name + muted variant count. A centered ghost "View all components" button closes the section.
- "How it works" section is one huge light rounded panel holding eyebrow, H2, sub, and a 16:9 near-black video block with a circular play button.
- "Build fast. Build consistently." 2x2 feature grid: icon tile on a soft purple chip, bold title, muted paragraph, text link.
- "Built with" divider (hairline, centered label) + 4 stack cards (logo tile, name, version) + the same CTA trio repeated.
- CLI section: left column has a mono terminal box with the npx command and a second box showing an interactive prompt with a highlighted option; right column is a 2x3 grid of starter-kit cards (Next.js, Vite, Bolt, Claude, v0, Lovable).
- Dark-mode section: side-by-side light and dark panels showing the same two mini widgets.
- Pricing: three tiers with large price figures ($0 / $349 / $999 on the source, five tiers total), small-caps tier tags, muted descriptions, check/minus feature lists with purple circled checks and help icons, full-width buttons; the middle tier carries the accent border and shadow.
- FAQ accordion inside another large rounded panel, plus a "Show more FAQs" ghost button.
- Wall of love: centered header, three testimonial cards with amber star rows, purple-highlighted phrases, and avatar + name + role rows.
- Footer: multi-column sitemap (brand column with award badge chips, then four link columns with purple column heads), a legal row, and a giant light-gray wordmark cropped at the bottom edge.

## Visual measurements and behavior

- Desktop observed at 1440 x 1000; full page height about 20,232px. Mobile observed at 390 x 844; full page height about 22,036px. No horizontal overflow at 390px on the source.
- Accent is a single violet (~#6C4CF6 family) used for eyebrows, primary buttons, checks, links, and highlight phrases; everything else is near-black text, gray secondaries, hairline borders, and #f9fafb panels.
- Type is a tight neo-grotesque sans (Inter class); display headlines around 60px desktop / 38px mobile with -0.02 to -0.03em tracking.
- Cards use 12-16px radii, 1px #eaecf0 borders, and hover lift shadows.
- Mobile: 4-col grid collapses to 1 column, pricing stacks, CLI/kits stack, dark-mode panels stack, footer columns go single file, giant wordmark remains.

## Original-study translation

This study keeps the source's section sequence, spacing logic, dot-grid hero, overlapping-docs proof, card-grid composition, purple-on-white system, and responsive rules. It replaces the source name, logo, wordmark, all copy, screenshots, prices, testimonials, people, version numbers, and brand marks. Every preview is drawn with HTML/CSS/inline SVG; no source assets, fonts, or imagery are used. The fictional library is "Atlas UI React".
