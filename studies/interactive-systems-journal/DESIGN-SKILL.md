# Interactive Technical Journal Design Skill

Use this system for an educational developer journal, research notebook, or technical essay collection that needs to feel authored, visual, and calm.

## 1. Build the shell

- Use a warm gray page instead of pure white.
- Center a wide container, cap it near 1450px, and define its edges with 1px lines.
- On desktop, split it into a 280-340px introduction rail and a flexible article column.
- Keep the rail sticky only while it remains a rail. Below about 900px, move it into normal document flow above the feed.

## 2. Establish the type contrast

- Use a distinctive serif for the publication name and essay titles.
- Use a plain UI sans for summaries and navigation.
- Use mono or mono-like 11-13px labels for dates, categories, and reading time.
- Favor short headline measures, tight headline leading, and relaxed body leading.

## 3. Make content visual

- Pair each major story with one locally authored diagram.
- Build diagrams from CSS primitives and simple SVG paths rather than stock illustrations.
- Give each diagram one clear concept: a sequence, path, state change, token stream, or graph.
- Use the diagram as explanation, not decoration. Avoid gradients, glossy effects, and generic dashboard mockups.

## 4. Use notebook details sparingly

- Define hierarchy with fine rules, dashed separators, and small geometric marks.
- Keep card backgrounds close to the page color so borders do the structural work.
- Allow one sharp accent color for active nodes, current state, and a single main action.
- Prefer square or lightly rounded geometry. Pill shapes belong only on compact actions or tags.

## 5. Pace the page

- Start with a compact utility header, then one promoted feature.
- Follow with a chronological feed whose rows have consistent media proportions.
- Use generous vertical padding between entries and let borders connect the sequence.
- Keep descriptions to two or three lines and metadata on a separate line.

## 6. Responsive rules

- At tablet/mobile, stack every image/text pair and put imagery before text.
- Reduce side padding to 20-24px without shrinking touch targets below 40px.
- Let large serif type step down smoothly with `clamp()`.
- Test around 390px and 1440px. Confirm there is no horizontal scrolling and that sticky behavior is disabled on mobile.

## 7. Interaction and accessibility

- Underline article titles on hover instead of moving the whole card.
- Keep animation optional and subtle; honor `prefers-reduced-motion` in production builds.
- Maintain visible focus states and useful labels for icon-only controls.
- Keep text contrast high even when using muted gray metadata.

## Avoid

- Copying a publication's name, author details, prose, illustrations, or proprietary interactive demos.
- Turning the layout into a generic card grid.
- Filling every empty area with decoration.
- Using multiple saturated accents or loud scroll effects.
