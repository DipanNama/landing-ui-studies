# Linear landing page reference notes

Source inspected: https://linear.app/ on September 19, 2026.

## Composition

- Restrained dark header with wordmark, compact navigation, and a high-contrast signup action.
- Oversized, centered hero copy followed by a large product mockup rather than a decorative marketing illustration.
- Quiet customer-logo band transitions into an editorial statement about the product's point of view.
- Three concise principles introduce the system before feature sections expand into detailed workflow demonstrations.
- Feature storytelling alternates focused copy with framed, credible app-like scenes.
- Changelog cards, customer proof, and a simple closing call to action complete the page.

## Visual system

- Near-black surfaces (`#08090a` family) with subtle one-pixel white borders and layered charcoal panels.
- White type is softened through opacity rather than many unrelated gray values.
- Headlines are large, tightly tracked, medium weight, and use compact line heights.
- Purple/periwinkle acts as the main signal color, used sparingly for status and ambient glow.
- Radius is controlled: roughly 8px for controls and 14–16px for large frames.
- Background grain and low-opacity radial light prevent flat black sections without becoming illustration.
- Product scenes use dense 10–13px interface typography to contrast with expansive marketing copy.

## Responsive behavior

- Desktop navigation collapses to brand, primary action, and menu affordance on mobile.
- The hero stays centered while actions become full-width stacked controls.
- Product mockups crop intentionally instead of shrinking the interface until it is unreadable.
- Three-column principles, update cards, and complex split features become single-column flows.
- Large type scales down strongly while preserving tight tracking and short measures.

## Original-study boundary

The recreation at `studies/northstar-product-os/` uses the original fictional product Northstar, original copy, CSS-authored app scenes, and invented customer names. It studies hierarchy, rhythm, density, responsive cropping, and color behavior without copying Linear's logo, screenshots, testimonials, proprietary media, or brand copy.

## Comparison checklist

- [x] Dark monochrome foundation with controlled periwinkle accent
- [x] Large editorial hero and credible product UI scene
- [x] Product-principle statement followed by three concise pillars
- [x] Alternating workflow sections with original CSS visuals
- [x] Changelog, testimonial, and closing conversion section
- [x] Dedicated mobile reflow at 760px and below
