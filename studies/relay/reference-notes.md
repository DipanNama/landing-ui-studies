# Reference notes — resend.com landing study

Investigated the live https://resend.com/ homepage on 2026-09-19 (01:54-01:58 IST) through a
real browser at 1280x713 (desktop) and 390x844 (mobile emulation), full 12,141px page
(desktop) / 14,146px (mobile). This file records what the page does so the study can be
rebuilt faithfully. The study (`index.html` in this folder) recreates the *design language*
with original copy, fictional companies, and CSS/SVG-generated visuals — no Resend assets,
logo, brand name, or copy are reused.

## Page structure (desktop scroll order)

1. **Fixed header** — wordmark left; centered menu of dropdown buttons (Features, Company,
   Enterprise, Help, Docs, AI) + Pricing link; right: Log in + "Get started" dark pill.
   Transparent at top, gains blur + hairline border after scroll.
2. **Hero** — gradient-bordered announcement pill ("Join us at Resend Forward"), giant
   serif H1 "Email for developers" (2 lines), gray 17px subcopy, dark "Get started" pill +
   "Documentation" text link. Right side: glossy 3D cube-of-cubes (Rubik-like, black glass
   tiles, subtle iridescent reflections) floating over a soft floor reflection.
3. **Logo wall** — centered 2-line statement, 12 white customer logos in 2 rows of 6
   (Warner Bros., Max, Raycast, Mistral AI, Replit, Anghami, Gumroad, Decathlon, Supabase,
   Leap, Payload, Paper), "Explore Enterprise ›" link.
4. **"Integrate this weekend"** — centered 3D app-icon tile (envelope glyph, colorful edge
   glow), H2 with purple→blue→teal gradient on "this weekend", subcopy, horizontally
   scrollable strip of 13 SDK icon tiles (Node.js, Serverless, Ruby, Python, PHP, CLI, Go,
   Rust, Java, Elixir, .NET, REST, SMTP). Below: framework-tabbed code window (Node.js,
   Next.js, Remix, Nuxt, Express, Hono, Redwood, Bun, Astro + copy button), line-numbered
   mono code with syntax colors (purple keywords, green strings), footer links "View on
   GitHub" / "Download ZIP".
5. **"First-class developer experience"** — left-aligned sans H2 (note: section H2s are
   sans, only hero/final are serif), subcopy with italic accent, two large rounded cards:
   - Test mode: floating "Delivered … [Send]" pill over mono HTTP 200 log lines.
   - Modular webhooks: event feed with colored status pills (Bounced=red, Complained=amber)
     + timestamps + small tag chips (recipient, type, agent, OS).
6. **"Write using a delightful editor"** — centered heading + product mockup: toolbar
   (Styles button, doc title, "a day ago", Test + white Send button), From/To/Subject rows
   (To holds an audience chip), white body canvas with "Press '/' for commands" — the white
   canvas inside the dark UI is a deliberate contrast beat.
7. **"Go beyond editing"** — two cards: Contact management (icon tile + audience dropdown +
   metric columns ALL CONTACTS / UNSUBSCRIBED / sparkline) and Broadcast analytics
   (DELIVERABILITY 98% big number over green radial glow, Delivered/Bounced rows; dimmed
   ENGAGEMENT 41% beside it).
8. **"Develop emails using React"** — centered orbit-atom 3D icon, heading, subcopy, two
   CTAs; then a window: macOS traffic lights, desktop/mobile + dark/light preview toggles,
   3-pane split — file tree (welcome/reset/invite/digest .tsx), TSX code with line numbers,
   live white email preview (cyan logo circle, heading, blue #00A3FF button).
9. **"Reach humans, not spam folders"** — one large rounded container; left-aligned H2;
   3x3 grid of deliverability features with small outline icons (blocklist tracking, regional
   sending, BIMI, dedicated IPs, suppression list, IP/domain monitoring, DNS verification,
   infrastructure, DMARC). Key terms bolded inside gray copy.
10. **Testimonial** — dark panel with white triangle (customer logo), big centered quote,
    avatar + name + role (Guillermo Rauch, CEO at Vercel).
11. **"Everything in your control"** — three selectable cards (Intuitive analytics / Full
    visibility / Domain authentication; active gets green glow underline) above a dashboard
    mockup: left sidebar (Emails, Broadcasts, Audiences, Metrics, Domains, Logs, API Keys,
    Webhooks, Settings, user row), top bar (Help, Docs, Feedback), metric cards
    (DELIVERABILITY/REPUTATION/ENGAGEMENT with status rows + percentages), and a
    "SENT EMAILS 29,486" line chart (green line + fading area fill, dashed gridline).
12. **"Beyond expectations"** — centered heading + sub, horizontal scroll row of testimonial
    cards (company logo circle + stacked avatar, name, role).
13. **Final CTA** — giant serif "Email reimagined. / Available today." + Get started pill;
    below, a huge near-black "Resend" wordmark cropped by the footer.
14. **Footer** — address + social icon circles (X, Discord, LinkedIn, YouTube) + green-dot
    "All systems operational" status pill; 5 link columns (Features, Resources, Company,
    Help, Community).

## Measured design tokens

- Background: `#000000`; primary text: `#f0f0f0` / `rgba(252,253,255,.937)`; secondary:
  ~`#a3a3a3`; faint: ~`#6e6e6e`. Hairline borders: white at 5-8% opacity.
- Type: body/UI — Inter 16px/24px; section H2 — "ABC Favorit" (grotesk) 56px/67px,
  letter-spacing -2.8px, weight 400; card H3 — 20px/26px; hero + final display — "Domaine"
  (sharp transitional serif) 96px/96px, -0.96px; code — "Commit Mono" ~13.5px.
  Study substitutes: Instrument Serif (display), Inter (sans), JetBrains Mono (code).
- Buttons: 48px tall, padding 0 20px, radius 16px, Inter 600 16px, dark fill (#1b1b1e) +
  2px `rgba(255,255,255,.05)` border. Nav button: 38px, radius ~11px. White Send button
  inside mockups.
- Accent gradient (text + icon edges): violet `#c084fc` → blue `#60a5fa` → teal `#2dd4bf`.
- Status colors: green `#3dd68c`, red `#ff6369`, amber `#ffb224`; pills are 12%-alpha
  tinted bg + full-strength text.
- Accent blue (email preview CTA): `#00A3FF`.
- Radius: base 8px; buttons 16px; tiles 18px; cards 20-24px; big containers 28px.
- Color system underneath: Radix-style 12-step dark scales (gray, amber, blue, bronze…).

## Interactions

- Header gains blur + border on scroll; dropdown menus on the nav items.
- Code window tabs swap samples; copy button.
- Control cards switch the dashboard panel content; active card shows a glowing green
  baseline.
- Testimonial row scrolls horizontally (scroll-snap).
- Mobile (390px): hamburger menu; hero stacks (visual above copy), H1 → 64px centered;
  CTAs full-width; SDK strip + code tabs scroll horizontally with visible thin scrollbar;
  all card pairs and the 3x3 grid stack; dashboard sidebar collapses to an icon rail;
  footer becomes a 2-column grid.

## Substitution choices in the study

- Product renamed "Relay" (fictional). All copy rewritten. Fictional customers
  (Northwind, Globex, Initech, …) replace real logos; real-person testimonial replaced
  with fictional people.
- The 3D cube render → CSS `preserve-3d` cube with three 3x3 glossy tile faces + float
  animation + radial floor glow.
- 3D app icons → CSS gradient tiles with inline SVG glyphs and a conic gradient edge.
- Product screenshots (editor, dashboard, email preview) → hand-built HTML/CSS mockups
  matching layout, colors, and density.
- Photographic avatars → initial monograms on gradient circles.
