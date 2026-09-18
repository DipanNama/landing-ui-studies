---
name: calm-social-publisher
source-study: https://typefully.com/
---

# Calm social-publisher landing system

Use this skill to build original landing pages for writing, scheduling, creator, communication, or lightweight collaboration products.

## Core feel

Make the page feel calm, capable, and product-first. The user should see the product before they encounter a long feature list. Confidence comes from space, crisp typography, and believable interface details rather than decoration.

## Tokens

```css
--ink: #151619;
--muted: #6c7078;
--line: #e7e8eb;
--surface: #f5f6f7;
--accent: #3080ff;
--accent-2: #8d54ff;
--dark: #09090b;
--radius-control: 10px;
--radius-card: 18px;
--radius-stage: 17px;
--shadow-stage: 0 22px 70px rgba(16,24,40,.10);
```

Use Inter or a close system sans. Keep paragraph copy around 15-19px. Use tight display tracking between -0.045em and -0.065em.

## Page recipe

1. **Quiet navigation** - 62-70px tall, compact wordmark, four or fewer text links, secondary login and one dark primary action.
2. **Centered hero** - a small status pill, a two-line 46-82px headline, one gradient phrase, 500-650px supporting copy, paired actions, and one small adoption cue.
3. **Product stage** - 960-1100px wide desktop application mockup with a light border and soft deep shadow. Compose it from a left workspace menu, focused editor, and right live preview.
4. **Feature grid** - three equal cards. Give each card about two-thirds visual UI and one-third copy. Use collaboration, calendar, and analytics as distinct visual shapes.
5. **Dark workflow contrast** - near-black full-width band containing two large cards. Keep borders visible but quiet; use blue/violet only for state and focus.
6. **Conversion close** - one pale gradient rounded panel, a short headline, one sentence, and one action.

## Component rules

- Buttons: 42-48px tall, 10px radius, 14px semibold label. The primary button is near-black, not the accent color.
- Cards: 1px cool-gray border, 18px radius, little or no outer shadow. Put shadows inside cards on interface miniatures instead.
- Product chrome: use a 52px title bar and tiny traffic-light dots. Keep the interface text at 11-15px so the product stage reads as an application.
- Accent: reserve blue-violet gradients for one headline phrase, a brand mark, charts, and selected states.
- Copy: lead with outcomes. Feature titles should be direct verbs or benefits, not category labels.
- Motion: one subtle cursor blink or small hover lift is enough. Avoid animated gradients and floating decorative blobs.

## Responsive rules

At 900px, hide the right preview panel and reduce the app to sidebar + editor. Let feature cards become two columns, with the last card spanning the row. At 600px:

- hide text navigation and secondary action;
- stack hero actions full-width;
- remove the product sidebar so only the editor remains;
- switch all grids to one column;
- left-align section intros even if the hero stays centered;
- keep 14px viewport gutters and 42px minimum control height;
- target a 43px hero headline and 35-38px section headlines.

Never squeeze desktop interface chrome into mobile. Remove secondary panels and preserve the core task.

## Originality guardrails

Do not copy a reference company's name, logo, social proof, customer identities, product screenshots, avatars, testimonial wording, or exact feature copy. Build local interface miniatures from simple CSS geometry and original text. Keep the hierarchy and rhythm, then change the brand, message, illustrations, interface details, and product story.

## Quality check

Render at desktop and 390px mobile. Confirm no horizontal overflow, the hero CTA is visible without awkward wrapping, the app stage remains legible, the dark section has enough contrast, and all original UI geometry survives without source assets.
