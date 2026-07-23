# Practices — Optidata Design

Positive rules from anti-slop + UX (adapted for Neocloud marketing portal). Hard bans stay in [never.md](never.md).

## Visual Contract (before substantial UI edits)

State this compactly in the turn, then implement:

```md
Visual Contract
- Surface: home | products-hub | product | solution | pricing | calculator | security | other
- User job: …
- Design source: DESIGN.md + optidata-design
- Density: medium-low (marketing) | medium (hub/pricing)
- Layout: …
- Forbidden tells: (from never.md + surface below)
- Verification: desktop + mobile check planned
```

Skip the full block only for tiny one-line CSS tweaks after a critique.

## Surface types

| Surface | Job | Density | Must | Avoid |
|---|---|---|---|---|
| **Home / landing** | Convert → product or architect path | medium-low | Hero budget, dual motion, real proof below fold | Fake metrics, generic SaaS hero, inventing featured cards |
| **Products hub** | Pick a path in ≤2 clicks | medium | Four equal paths, catalog links | Ranking one path with glow |
| **Product page** | Explain capability + CTA | medium | Hero → sections → final CTA | Numbered steps, fake screenshots |
| **Solution** | Sales-assisted outcome | medium | Proof + architect CTA | Product-SKU template |
| **Pricing** | Clarify economics | medium | Billing rules, product rows | Invented rates as locked |
| **Calculator** | Size stack without login | medium | Clear totals, disclaimer | Blocking signup to explore |

## CTA hierarchy

- **One primary CTA** per viewport / major section (`button-primary`).
- Secondary = `ghost` or text link — never a second filled purple button competing in the same group.
- Card grids: equal visual weight; CTA style may differ by motion (self-serve vs architect) but cards themselves stay peers.

## Product proof

- Prefer real console mock, real screenshot, or honest placeholder labeled as such.
- Never ship fake dashboards made of empty div rectangles.
- Never invent logos, customer counts, or testimonials not in approved copy (`content/` / live site quotes).

## Accessibility & interaction

- Body text contrast target: **≥ 4.5:1** on canvas (use white-at-opacity tokens — see DESIGN.md).
- Focus ring: 2px `{colors.primary-glow}`, offset 3px — never remove.
- Interactive targets ≥ 44px height (CTAs, key nav).
- Do not rely on hover alone to show that something is clickable (`cursor: pointer`, clear link/button chrome).
- Respect `prefers-reduced-motion` when adding motion.

## Icons & chrome

- Structural icons = SVG (one family/stroke). **No emoji as icons.**
- Clickable non-button elements: `cursor: pointer`.

## Design source discipline

- Ultravioleta tokens in DESIGN.md win. Do **not** run external palette/font recommenders that replace the brand.
- Critiques → [feedback-log.md](feedback-log.md) → promote to never / DESIGN / tokens.
