# Selene - reference notes

Source observed: https://www.fumadocs.dev/ (current landing page), 19 September 2026, via cloud browser at 1280x720 and 390x844.

## Observed system

- Near-black canvas with dark charcoal panels, thin warm-gray borders, and generous corner radii.
- Signature dithered/halftone artwork: warm orange-to-olive gradient orbs rendered as dot rasters, plus a large halftone moon in the closing banner.
- Pale cream-yellow primary accent (buttons, highlighted headline words, mono labels) against the dark field; one vivid orange gradient panel for testimonials and a product shot.
- Typography: modern grotesk with tight tracking for display, monospace for eyebrow labels, terminal content, and the "BUILD YOUR DOCS" banner.
- Layout: sticky top nav (logo, links, search pill with Ctrl+K, theme toggle, repo icon), centered hero with outlined pill tag and paired pill CTAs, then a docs-app mock (sidebar + content) peeking from the hero bottom.
- Intro paragraph sets key phrases in the cream accent inline.
- "TRY IT OUT" mono eyebrow, copyable command bar, and a CLI terminal panel floating over a dithered backdrop with a "localhost:3000 / New App launched!" toast.
- Social proof: two-column row pairing a text card with an orange panel containing a horizontal testimonial marquee of dark cards.
- Feature storytelling alternates split rows (code card + copy with bullet list) and two-card grids; tabs (Writer -> Developer -> Automation) and CMS labels switch emphasis without leaving the section.
- Community block: sponsor card with overlapping avatar stack beside the mono-type moon banner.
- Final CTA: quiet card with three icon-led promises and the same paired pill buttons.
- Mobile (390px): nav collapses to search + hamburger, hero recenters, CTAs stack full-width, app mock drops its sidebar, two-column grids go single column.

## Original substitutions in this study

- New product identity: Selene, a documentation toolkit.
- All copy, testimonial people and companies, CLI commands, code samples, and layer names are invented.
- The dithered orb/moon artwork is rebuilt with CSS radial gradients under a dot-pattern mask; no source images.
- Docs app mock, terminal, search pill, avatars, and icons are locally authored HTML/CSS.
- System font stack instead of the source's webfonts.
- No source logo, screenshots, videos, fonts, testimonials, brand names, or downloaded assets.

## Visual comparison checklist

- [x] Desktop: sticky dark nav, pill tag, oversized tight-tracked headline with accent words, paired pill CTAs, docs-app mock.
- [x] Desktop: dithered orb atmosphere, terminal over dithered field with toast, orange testimonial marquee, split code rows, moon banner, final CTA card.
- [x] Mobile: collapsed nav, centered hero, stacked full-width CTAs, single-column grids, no overflow at 390px.
- [x] Production: root index and permanent study route render from Vercel.
