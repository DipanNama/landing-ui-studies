---
name: annotated-editorial-course-landing
version: 1.0.0
source-study: https://uidesigncourse.com/
scope: landing pages for educational products, tools, and technical guides
---

# Annotated editorial landing design skill

Use this skill to make an original page that feels like a precise design document: calm, educational, technically credible, and unusually clear. Do not reuse the reference brand, copy, assets, lessons, or offer.

## 1. Visual thesis

Build on a mostly white canvas. Make typography and spacing do the work. Use one saturated accent only where the user should look next. Add a few measurement labels, guides, or selection outlines so the interface demonstrates its own rules.

## 2. Tokens

```css
--ink: #171717;
--muted: #666b73;
--line: #e6e7e9;
--paper: #ffffff;
--soft: #f7f7f8;
--accent: #3478f6;
--radius-control: 999px;
--radius-panel: 18px;
--space: 4, 8, 12, 16, 24, 32, 48, 64, 96, 128px;
```

Use a neutral variable sans if licensed for the project. Otherwise use `Inter, ui-sans-serif, system-ui`. Use a neutral mono only for measurements and labels.

## 3. Typography

- Hero: `clamp(2.25rem, 5vw, 3.5rem)`, 600, line-height 1.05, tracking -0.035em, max-width 13em.
- Section title: 24px, 600, 1.3.
- Item title: 16px, 600, 1.3.
- Body: 16px, 400, 1.55, max-width 68-72ch.
- Meta label: 11-12px mono, uppercase, 0.04em tracking.
- Do not introduce more than three text sizes inside one section.

## 4. Layout

- Page max-width: 1120-1200px with 24px mobile gutters.
- Hero content max-width: 760px, centered.
- Reading sections max-width: 840px.
- Hero vertical padding: 80-112px desktop, 52-72px mobile.
- Section gap: 96-128px desktop, 72-88px mobile.
- Space within a group must always be smaller than space between groups.

## 5. Signature components

### Annotated hero
Use a faint radial dot background. Add no more than four annotations. Labels are quiet mono capsules connected by thin gray rules. One headline word may be blue and surrounded by a dashed selection box with tiny handles. An annotation toggle may hide the teaching overlay.

### Offer CTA
A black capsule with white text. Pair it with a small uppercase offer label above and a low-contrast reassurance line below. The CTA stays one clear sentence.

### Preview form
A rounded single-line field with the button nested on the right at desktop. Stack only below 440px. Always include a visible label.

### Curriculum rows
Use 1px separators and number labels. The first group may be expanded to expose lesson rows; others stay collapsed. Avoid card grids here.

### Prompt/code panel
Use an off-white panel, mono type, a 16-18px radius and a small accent badge. The panel should feel like a reusable artifact, not a decorative screenshot.

### Audience list
Use a simple three-column grid on desktop and one column on mobile. Thin top rules replace heavy cards.

## 6. Motion

- Keep transitions 160-220ms with an ease-out curve.
- Animate annotation visibility with opacity and 4px translation.
- Accordion disclosure may animate grid rows; respect `prefers-reduced-motion`.
- Never use autoplay video, parallax, marquee, or springy button motion for this system.

## 7. Responsive rules

At 720px: reduce headline, remove side annotations, allow the header actions to tighten, switch multi-column content to one column. At 440px: stack the preview field action if needed. Keep 44px minimum hit targets. Prevent a single highlighted hero word from creating horizontal overflow.

## 8. Build procedure

1. Write the product's one-sentence promise and primary action.
2. Map sections to proof: promise, method, contents, reusable artifact, audience, final action.
3. Apply the spacing and type tokens before decoration.
4. Add the dot grid and only the annotations that teach something real.
5. Build the desktop reading rhythm.
6. Recompose at 390px rather than merely shrinking.
7. Check keyboard focus, reduced motion, contrast, label association, and overflow.
8. Compare screenshots at 1280px and 390px against the intended hierarchy, not against copied assets or text.

## 9. Quality gates

Reject the page if it uses generic glass cards, several accent colors, heavy shadows, vague startup copy, icons as decoration, or annotations that do not describe actual values. The final page should still work after all annotations are turned off.
