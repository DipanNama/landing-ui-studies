# Inkline - reference notes

Source observed: https://www.notioly.com/ (current landing page), 19 September 2026.

## Observed system

- Nearly white canvas (#fafafa) with pure black ink and mid-gray supporting copy. No color anywhere except one tiny pink marketplace badge in the final CTA.
- Header: hand-drawn feel logo (circled initial + wordmark) left; plain text links right with a small chevron on one item; black pill purchase button with price inside the label.
- Hero is fully centered: small white announcement chip with a sparkle ("March: +16 Illustrations"), very heavy display headline (~56px, weight 900, Cabinet Grotesk), one-line gray subcopy with a bolded count, and a byline pairing a tiny round avatar with a script-font name.
- The product proof is a borderless 4-column grid of white cards (thin 1px border, ~16-18px radius), each holding one black line-art illustration. Cards are illustration-first: no titles, no prices.
- One full-width light-gray ghost pill button ("View All 500+ Illustrations") closes the gallery.
- Feature section: small gray sparkle mark, centered heavy h2, three text-only columns each with a small line icon, bold title, and short gray paragraph.
- Final CTA is a large inset black panel (~24-26px radius) with a small line flourish, white heavy heading, paired pills (white primary with price, dark-gray secondary), and a one-line social-proof rating with a small badge.
- Footer: single quiet row, copyright left, three text links right.
- Mobile: nav collapses to logo + hamburger, hero headline recomposes around 40px, gallery becomes one column, features stack, CTA buttons go full width, footer stacks centered. No horizontal overflow at 390px.

## Original substitutions in this study

- New product identity: Inkline, by a fictional creator (Rhea Kapoor). New price, counts, month chip, and review line.
- All copy rewritten from scratch in the same register.
- All eight gallery illustrations are locally authored inline SVG line art (bicycle, plant, letter, coffee, cat, rocket, bulb, umbrella). None trace or reference the source's artwork.
- All icons, the logo mark, avatar, sparkles, and the rating badge are original inline SVG.
- System display stack (Archivo Black / Arial Black fallbacks) instead of the source's Cabinet Grotesk files; system script fallbacks for the byline.
- No source images, fonts, logo, copy, gumroad links, or downloaded assets.

## Visual comparison checklist

- [x] Desktop: centered chip + heavy hero, byline with script name, 4-column illustration card grid, full-width ghost button.
- [x] Desktop: sparkle + 3 text columns, inset black CTA panel with white/dark pill pair and rating line, quiet footer.
- [x] Mobile: hamburger header, recomposed hero, single-column gallery, stacked features, full-width CTA buttons, no overflow at 390px.
- [x] Production: root index and permanent study route render from Vercel.
