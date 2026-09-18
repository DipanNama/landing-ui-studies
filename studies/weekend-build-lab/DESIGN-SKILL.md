---
name: dark-event-conversion-landing
version: 1.0.0
source-study: https://www.outskill.com/
scope: landing pages for live cohorts, workshops, bootcamps, conferences, and event-style education offers
---

# Dark event conversion landing design skill

Use this skill to build an original page that converts for a time-bound live offer: a workshop weekend, cohort, bootcamp, or summit. The system is a dark, cinematic, high-proof sales page with one electric accent and a persistent conversion bar. Do not reuse the reference brand, copy, photography, names, or offer details.

## 1. Visual thesis

Dark canvas, near-black. A full-viewport photographic or scenic hero establishes mood; everything after alternates dark proof sections with one or two light utility sections (schedule, FAQ) so the page breathes. One high-chroma accent (lime/chartreuse family) marks every action. Photography is desaturated so the accent owns the eye. Trust is built by volume: stats, backer headshots, employer logos, testimonials, brand walls.

## 2. Tokens

```css
--ink: #0b0b0c;        /* page background */
--coal: #131316;       /* raised dark surface */
--panel: #1a1a1f;      /* card surface */
--line: #2a2a30;       /* dark borders */
--paper: #ffffff;      /* light section background */
--fog: #a7a7ad;        /* muted text on dark */
--fog-d: #5c5c62;      /* muted text on light */
--accent: #c9f24b;     /* single action color */
--radius-card: 14px;
--radius-control: 8px; /* CTAs are soft rectangles, not pills */
```

Use a neutral grotesque (`Inter, ui-sans-serif, system-ui`). Use mono only for eyebrows and session metadata.

## 3. Typography

- Hero: `clamp(2.5rem, 5.4vw, 4.1rem)`, 700, line-height 1.04, tracking -0.035em, left aligned.
- Section headline: `clamp(1.9rem, 3.6vw, 2.75rem)`, 650-700, 1.1, tracking -0.03em.
- Card title: 17-18px, 600.
- Body: 15-16px, 1.55, muted.
- Eyebrow: 12px mono, uppercase, 0.12-0.14em tracking, quiet gray. Every section gets one.

## 4. Layout

- Content max-width: 1120-1180px, 24px mobile gutters.
- Hero: full viewport width, min-height ~90vh, content left-aligned in a 760-880px column.
- Section padding: 88-104px desktop, 64-80px mobile.
- Alternate dark and light sections deliberately: hero (dark), backers (dark), logos (dark), program (dark), schedule (LIGHT), audience (dark), testimonials (dark), next programs (dark), FAQ (LIGHT), final CTA (dark).
- Grids: 3 columns on desktop for cards/quotes, 6 for backer wall, collapsing to 2 then 1.

## 5. Signature components

### Cinematic hero
Layered scenic backdrop (photography or generated gradient scene with silhouetted ridge lines), soft radial glow near the horizon, subtle grain. Left-aligned headline, one-line sub, then a CTA row: accent button beside a start-date/start-time meta block separated by thin left rules. Below, a stat row (3 stats) divided by 1px vertical rules, big number over small muted label.

### Accent CTA
Flat accent rectangle, dark text, 8px radius, 650 weight. Never outlined, never ghost. One primary action repeated through the page with the same words.

### Backer wall
Uniform portrait cards in a strict grid: grayscale photo (or generated avatar substitute), name, one-line credential. Card borders 1px, background one step above the page.

### Logo strip
Employer or partner wordmarks, desaturated, low contrast, generous gap. No carousel chrome.

### Program cards
Dark cards with a small illustrative visual on top (product-UI sketches, waveforms, node diagrams - generated, not screenshots) and a two-line promise below. 3 per row.

### Schedule switcher (light section)
Left: numbered session list (01-05), uppercase titles, active row in full ink. Right: detail panel with a dark banner image, mono session metadata (`DAY 1 · SESSION 1 · 10 AM - 1 PM`), title, summary, and checkmark bullets that break the border with hairline separators. Clicking a list row swaps the panel. On mobile the list becomes a horizontal scroll strip.

### Testimonial grid
Static 3-column grid of quote cards with circular avatars. Quote first, identity second. No autoplay carousel.

### FAQ split (light section)
Left column: eyebrow + large headline. Right column: bordered accordion rows with a plus that rotates 45 degrees when open. First row may start open.

### Sticky conversion bar
Fixed bottom bar, blurred near-black, present after the hero: offer name left, accent CTA center, struck price + "Free" + live countdown right. Compress to two rows on mobile. The countdown is real JS; it may reach zero and stop.

## 6. Motion

- Almost none. Hover states only (button darkens, links brighten).
- Schedule switch swaps content without transition or with a 150ms fade.
- Accordion plus rotates 45deg.
- Never autoplay video, parallax, marquees, or count-up animations. The urgency comes from the copy and the countdown, not motion.

## 7. Responsive rules

At 900px: card and quote grids to 2 columns, schedule stacks with a horizontally scrolling session list, FAQ to one column. At 760px: nav links collapse behind a menu button, hero min-height relaxes, stat row wraps, grids to 1 column, sticky bar wraps to two rows. Keep the accent CTA full-width friendly and 44px+ tall.

## 8. Build procedure

1. Write the offer: name, promise, date, time, price anchor, and the single CTA sentence. Repeat that sentence everywhere.
2. Order sections by proof escalation: mood, authority (backers), peers (logos), substance (program), logistics (schedule), belonging (audience), voices (testimonials), path (next programs), objections (FAQ), final ask.
3. Apply the dark/light alternation before styling details.
4. Build the hero scene and stat row first; it sets the tone budget for the page.
5. Build the schedule switcher and sticky bar JS; verify both at 390px.
6. Recompose grids at 900px and 760px rather than shrinking.
7. Check contrast of muted text on both canvases, reduced motion, keyboard focus, and horizontal overflow.

## 9. Quality gates

Reject the page if it uses more than one accent, gradient text, glassmorphism, stock-looking colorful illustration, autoplay anything, fake countdowns that reset on reload claims, or copied photography/names from the reference. All imagery must be owned or generated. The page must still convert with every image removed - type, stats, and structure carry it.
