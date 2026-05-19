# DATA Mobility Partners — Pitch Site Overview

## Context
I'm pitching a website management contract to **DATA Mobility Partners**, a Northern Virginia 501(c)(3) nonprofit serving seniors, veterans, and individuals with disabilities. The pitch meeting is **Friday, May 8, 2026** with **Ray Billings** (executive director) over Zoom.

- **Their current live site:** `datatrans.org` — the status quo I'm critiquing (accessibility, performance, dated design). I audited it along with their 990 financials.
- **My proposed redesign (this repo):** hosted at `https://vcarranza1.github.io/datamobility/`
- **Repo:** `github.com/Vcarranza1/datamobility` (main branch, clean working tree)
- **Proposed terms:** $25/hr, capped at 20 hrs/month ($500 max), first month free.

## Tech stack
Static multi-page site, hand-written HTML/CSS/JS, deployed via GitHub Pages.
- `styles.css` (891 lines) — single global stylesheet, custom CSS (no framework)
- `main.js` (148 lines) — small vanilla JS (mobile menu toggle, fade-up animations, animated stat counters)
- Google Fonts: Inter + Plus Jakarta Sans
- Font Awesome 6.5.1 for social icons
- Unsplash for hero/feature imagery
- Official DATA Mobility Partners logo (`logo.png`, transparent, ~70px in nav)

## Pages (7 total)
1. **`index.html`** — Home: hero ("Mobility for All"), two-pillar service split (TMA Hub / Community Hub), Cook for Vets spotlight, animated stats bar, "Why It Matters" feature row, programs overview, CTA banner
2. **`tma-hub.html`** — Professional services side (transportation demand management, employer/developer partnerships)
3. **`community-hub.html`** — Direct human services side (rides for seniors and veterans)
4. **`venture-out.html`** — Group travel / outings program (also where Cook for Vets lives)
5. **`enhanced-mobility.html`** — Federal/state-funded gap-filling transportation
6. **`about.html`** — Org info, governance section
7. **`contact.html`** — Contact form, donation CTAs

Shared header (logo + nav + "Donate Now" CTA) and footer (brand blurb, social links FB/LinkedIn/YouTube/Instagram, services list, org links, newsletter signup) across all pages. Mobile menu via hamburger toggle.

## Brand / design system (current state)
- **Navy:** `#1B3A6B` (primary brand, headers, CTA banner)
- **Teal:** accent color for cards/icons (we tried gold `#D4A017` and reverted)
- **Soft White:** `#F2F4F7` (background)
- Typography: Plus Jakarta Sans for headlines (600/700/800), Inter for body (400/500/600)
- Component vocabulary: `.btn-primary`, `.btn-outline`, `.card`, `.stat-item`, `.section-label`, `.fade-up` (scroll-triggered animation), `.cards-grid` / `.cards-grid-3`

## Recent work (last ~15 commits)
Mostly logo + brand polish:
- Brand palette iteration: introduced gold `#D4A017` for CTAs alongside navy `#1B3A6B`, then reverted gold accents back to teal (kept the navy update and soft white)
- Replaced inline SVG social icons with Font Awesome for consistency; added Instagram; fixed Instagram fill style
- Logo work: swapped in 2025 full-color official logo, transparent background, sized down nav logo from 90px → 70px, removed border line, made navbar taller
- Fixed 2 broken Unsplash images on community-hub
- Initial commit was a full multi-page scaffold (`ea679bf Add full multi-page website for DATA Mobility Partners`)

## Where we are
The site is **demo-ready** for the Friday pitch. Working tree is clean, deployed to GitHub Pages. The brand identity has settled on **navy + teal + soft white** (gold experiment rolled back). The structural skeleton across all 7 pages is in place.

## Likely next steps before / during the meeting
- Listen to Ray first; affirm existing work; propose specific quick wins doable inside the 20 hr/month cap
- Anything touching the live `datatrans.org` is out of scope until the contract is signed
- Possible polish areas if asked: real photography (replace Unsplash placeholders), real program content / stats from Ray, a working donation flow, accessibility pass, content for `about.html` governance section
