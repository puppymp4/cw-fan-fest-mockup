# CW Fan Fest · Santa Monica

Concept landing page for a **fictional** two-day fan convention on the Santa Monica Pier,
covering The Vampire Diaries, The Flash, Supernatural and Riverdale.

**Live:** https://cw.riftmedia.cc

## This event is not real

CW Fan Fest Santa Monica does not exist. This page is a web design demonstration:
no venue is booked, no performer has been contracted or approached, no tickets are
on sale, and no payment is collected anywhere on the site. Show titles, character
names and performer names appear as unlicensed fan reference only.

Not affiliated with, endorsed by, or connected to The CW Network, Warner Bros.
Discovery, Berlanti Productions, Alloy Entertainment, Archie Comics, or any
performer named on the page.

The page carries a concept notice in the masthead, a first-position FAQ entry, and a
full footer disclaimer. It is also served `noindex, nofollow` so it cannot surface in
search results as a real convention listing. Remove the robots meta tag in
`index.html` to change that.

## Stack

Single static `index.html` — no build step, no dependencies, no framework.
All CSS and JS are inline. The four show illustrations and ten activity icons are
hand-authored inline SVG. The hero is `hero.jpg`.

## Features

- **Day/night theming** — the Day One / Day Two switch in the masthead drives both the
  colour palette and which run sheet is shown. Day One is the daylight palette,
  Day Two the after-dark one. It initialises from the visitor's `prefers-color-scheme`.
- **Live countdown** to Day One doors (9 Aug 2026, 8:00 AM PT).
- **Pass selector** with quantity stepper and an order summary that recalculates
  subtotal, booking fee and total. Checkout is intentionally inert.
- Fully responsive, `prefers-reduced-motion` respected, keyboard focus states.

## Local preview

```bash
python -m http.server 8000
# then open http://localhost:8000
```

---

Built by **Rift Media** · https://riftmedia.cc
