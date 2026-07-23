---
name: optidata-design
description: >-
  Optidata Cloud Ultravioleta design system for portal UI. Use when building,
  redesigning, reviewing, or fixing any Optidata Cloud / Neocloud page,
  component, token, CSS, layout, hero, pricing card, or visual polish — and
  whenever the user invokes /optidata-design, critiques the look, or says what
  they do not want in the design.
---

# Optidata Design

Living design system for Optidata Cloud (Ultravioleta). Works across projects: lock brand rules, capture critiques, promote them into permanent agent rules.

## Mandatory reads (every UI turn)

Read these **before** choosing colors, type, spacing, radius, shadows, cards, nav, CTAs, or motion:

1. **DESIGN.md** — tokens + patterns (normative)
   - Prefer project copy if present: `Neocloud/Design/DESIGN.md`, `Design/DESIGN.md`, or `DESIGN.md` at repo root
   - Else use the skill-bundled [DESIGN.md](DESIGN.md)
2. [never.md](never.md) — hard bans
3. [practices.md](practices.md) — Visual Contract, surfaces, CTA, a11y, proof
4. [feedback-log.md](feedback-log.md) — latest critiques not yet promoted
5. [checklist.md](checklist.md) — completion gate

If the project has CSS tokens (e.g. `**/tokens.css`), keep them aligned with DESIGN.md.

Source map: [sources.md](sources.md).

## Authority order

When sources conflict:

1. Explicit user instruction in **this** conversation
2. [never.md](never.md) + open items in [feedback-log.md](feedback-log.md)
3. YAML tokens in the active DESIGN.md (project first, else skill-bundled)
4. [practices.md](practices.md) + prose in DESIGN.md
5. Live project CSS / components

Never invent a second brand CTA color, a cream/white marketing canvas, or Inter/Roboto/Arial as the primary font. Never replace Ultravioleta via external palette tools.

## Workflow branches

### A — Build / redesign UI

1. Read mandatory files above.
2. **Declare a Visual Contract** ([practices.md](practices.md)) for substantial work.
3. Use **only** DESIGN.md token names. No raw hex in new UI unless it already exists as a token.
4. Match **surface type** (home · hub · product · solution · pricing · calculator).
5. Hero budget: brand + one headline + one supporting + one CTA group + one visual anchor. **No eyebrows** unless explicitly asked.
6. **Do not invent emphasis.** Peer cards stay equal. No glow / `card--featured` unless asked.
7. **One primary CTA** per viewport/section; secondary is ghost.
8. Ship against [checklist.md](checklist.md). Verify desktop + mobile mentally or in preview before “done”.

**Done when:** checklist passes, never-list clean, Visual Contract (if used) satisfied.

### B — User critiques the design (“não quero X”, “melhorar Y”)

1. Restate the critique as a crisp rule (do / don't).
2. Append to [feedback-log.md](feedback-log.md).
3. Apply the fix to the UI.
4. **Promote** when stable → `never.md` and/or DESIGN.md (+ project `tokens.css` if any).
5. Mark feedback entry `status: promoted`.

**Done when:** UI fixed **and** the rule is written down.

### C — Review existing UI

1. Read mandatory files.
2. Diff against tokens, never-list, practices, checklist.
3. Report: 🔴 must-fix · 🟡 should-fix · 🟢 optional.
4. Offer to fix + promote.

## Leading words

| Term | Meaning |
|---|---|
| **Ultravioleta** | Dark violet canvas (`#1E002F`), not light SaaS |
| **single voltage** | Only `{colors.primary}` (#8D0DE3) for primary CTAs |
| **hero budget** | First viewport composition limit |
| **hairline depth** | Elevation via surface + lilac hairline, not shadow stacks |
| **white-ink** | Headings/body = white at opacity (not solid lilac fills) |
| **Visual Contract** | Compact pre-edit declaration (surface, job, forbidden tells) |
| **promote** | Critique → never / DESIGN / tokens |

## Do not

- Skip DESIGN.md / never.md / practices.md
- Apply generic AI landing patterns or external “recommended” palettes
- Leave a user “não quero” as a one-off patch with no log entry
- Invent a parallel brand outside the Ultravioleta tokens
