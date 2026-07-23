# Checklist — Optidata UI gate

Copy into the turn and tick before claiming UI work done.

## Process

- [ ] Visual Contract declared (substantial UI) — see practices.md
- [ ] Surface type matched (home / hub / product / solution / pricing / calc)
- [ ] If user critique this turn → logged in feedback-log.md

## Tokens

- [ ] Colors from DESIGN.md / `tokens.css` only (no orphan hex)
- [ ] Text uses **white-at-opacity** (`ink` / `body` / `muted`) — not solid lilac fills
- [ ] Primary CTA uses `{colors.primary}` only; hover `{colors.primary-active}`
- [ ] Canvas is Ultravioleta (`#1E002F` / deep), not light/cream
- [ ] Manrope for display+body; JetBrains Mono only on technical surfaces
- [ ] No typographic orphans on display headlines

## Composition

- [ ] No eyebrows / section kickers unless explicitly asked
- [ ] No pill / badge-pill above `h1` unless explicitly asked
- [ ] Hero budget respected (no stats/cards/chips clutter)
- [ ] One primary CTA per viewport/section; secondary is ghost
- [ ] One job per section: one headline + short support
- [ ] Peer cards visually equal unless told otherwise

## Components & interaction

- [ ] Buttons pill; cards 16–22px; inputs 12px
- [ ] Button hover: **no** translateY — color / border / glow only
- [ ] Cards: **no** hover / glow / featured unless explicitly asked
- [ ] No 01/02/03 on cards unless explicitly asked
- [ ] Focus ring visible; targets ≥ 44px; `cursor: pointer` on clickables
- [ ] No emoji-as-icons; no fake dashboard divs / invented proof
- [ ] Nav matches `top-nav` token (sticky, blur, 68px)

## Verification

- [ ] Desktop layout sane (wrap ~1180px)
- [ ] Mobile: no horizontal scroll; type/CTAs usable
- [ ] Contrast OK for body on canvas (white-ink tokens)

## Fail = not done

Any unchecked critical item (tokens, hero budget, never-list, invented emphasis) blocks “done”.
