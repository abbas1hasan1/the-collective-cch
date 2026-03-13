# The Collective — Project Instructions

## What This Project Is
A concept proposal/pitch deck (as a single-page website) for **The Collective**, a specialty coffee cafe planned for CityCentre Houston. The `index.html` is a visual pitch page for the landlord (Radom Capital), not a functioning business website.

## Founders
- **Abbas Hasan** — Tech, design, presentation (this is the user)
- **Ali Asad Hasan** — Restaurant/coffee operations

## Key Files
- `index.html` — The concept deck (all inline CSS/JS, single file)
- `logos/` — Brand logo assets (primary, dark, wordmark)
- `renderings/` — Final exterior and interior 3D renders
- `menu/` — Menu item photography (Collective Cups, cold brew lineup, canned cold brew, toast, paninis, coffee packaging)
- `packaging/menu.png` — Menu board visual
- `archive/` — Design iteration history

## Business Documentation
All business details are organized in `docs/`:
- `docs/concept.md` — Brand identity, pillars, aesthetic, colors, typography
- `docs/menu.md` — Full contextual menu story: categories, strategy, packaging philosophy, "why" behind each item
- `docs/space.md` — Physical space layout, renderings, logo assets
- `docs/location.md` — CityCentre stats, target customer, competitive context, landlord info
- `docs/story.md` — Founders' background, insight, vision/philosophy
- `docs/community.md` — Run club, wellness events, seasonal activations

## Design Guidelines
- **Aesthetic**: Warm minimalist — health & wellness focused, essentials only, remove the unnecessary
- **Colors**: Warm taupe `#D5CFC8`, concrete `#C2BAB0`, dark `#1A1917`, accent `#413936`, light `#EEEDEA`
- **Fonts**: Bebas Neue (display), Instrument Sans (body), Lora (serif accent)
- **Reference brands**: % Arabica, Koncrete Dubai, La La Land Kind Cafe, Slowpokes

## Working With This Project
- The pitch deck is a single `index.html` with all CSS inline in `<style>` tags — no external stylesheets
- When making visual changes, keep the warm minimalist concrete aesthetic consistent
- Logo assets are in `logos/` — use the appropriate variant for dark/light backgrounds
- When business details change, update both `index.html` AND the relevant `docs/*.md` file
- Never reference founders by first name in the pitch deck — use "we/our" or "the founders" for the landlord audience
- Brand identity emphasizes health, wellness, and essentials — not concrete aesthetics
- **Image rules**: Never crop or compress renderings/photos — show them in full with `border-radius: 20px`. Never use `object-fit: cover` or `max-height` on images as these will crop them. Only use `width: 100%` with `border-radius`. Give each image its own section with text alongside it. Always verify image display at mobile widths using Playwright before finishing.
- **Card style**: All content cards use dark background (`var(--bg-dark)`) with light text — no white/translucent cards. Keep consistent with the Our Story section style.
- **Scheduling**: Don't commit to specific scheduling (days, frequencies) in the pitch deck — keep community programming aspirational
- **Mobile-first centering**: On mobile (768px), all section text is centered for consistent flow. Desktop stays left-aligned where appropriate. The centering is applied via a block in the `@media (max-width: 768px)` CSS.
- **Menu showcase pattern**: After the menu card grid, there are 5 alternating image+text sections (reusing `.rendering-inner` / `.rendering-inner.reverse`) showcasing Collective Cups, Cold Brew Lineup, Canned Cold Brew, Breakfast Toast, and Paninis. Images sourced from `menu/` folder.
- **Section glow breaker**: A `.section-glow` CSS class creates a subtle warm ambient glow line between sections (inspired by interior rendering bench light). Currently prototyped between Concept and Our Story — can be expanded to other section transitions.

## Last Updated
2026-03-13
