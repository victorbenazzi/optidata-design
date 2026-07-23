# Feedback log — Optidata Design

Living critique → rule pipeline. Newest first.

When the user says what they **don't want** or how to **improve**, append an entry, fix the UI, then **promote** into `never.md` and/or `Neocloud/Design/DESIGN.md` + tokens.

## Entry template

```md
### YYYY-MM-DD — short title
- **Surface:** page / component (e.g. Home hero, Pricing cards)
- **Don't want:** …
- **Do instead:** …
- **Status:** open | promoted
- **Promoted to:** never.md §… · DESIGN.md §… · tokens.css (if any)
```

---

## Open

_(none)_

---

## Promoted

### 2026-07-23 — White-ink text (opacity, not solid lilac)
- **Surface:** Global typography (headings + paragraphs)
- **Don't want:** Solid lilac text (`#ECDFFF` / `#D6B9FE`) — weak contrast / muddy
- **Do instead:** White at opacity — ink 0.92 · body 0.72 · muted 0.55. Hairlines stay lilac for atmosphere
- **Status:** promoted
- **Promoted to:** DESIGN.md colors · tokens.css · never.md §Brand · checklist · practices (white-ink)

### 2026-07-23 — Practices pack (anti-slop + UX)
- **Surface:** Skill process
- **Don't want:** Missing Visual Contract, fake proof, dual primary CTAs, emoji icons, hover-only affordance
- **Do instead:** practices.md — Visual Contract, surfaces, CTA hierarchy, proof, a11y, icons; wired into SKILL + never + checklist
- **Status:** promoted
- **Promoted to:** practices.md · SKILL.md · never.md · checklist.md · sources.md

### 2026-07-23 — No glow / invented card highlights
- **Surface:** Home dual-motion `article.card.card--featured` (Private Cloud)
- **Don't want:** Glow on cards; agent inventing visual emphasis (featured vs peer) without request or criteria
- **Do instead:** Peer cards share the same treatment. `card--featured` / glow / strong border / purple shadow only when explicitly asked. Never “decide” one card is more important
- **Status:** promoted
- **Promoted to:** never.md §Components · DESIGN.md · global.css comment · equalized home/products/pricing/solutions/ProductPage cards

### 2026-07-23 — No card hover by default
- **Surface:** Home path cards `a.card.path-link` (Cloud Platform)
- **Don't want:** Any hover on cards — border change, translate, shadow lift
- **Do instead:** Cards are static by default. Hover only when the user explicitly requests it for that surface
- **Status:** promoted
- **Promoted to:** never.md §Components · DESIGN.md Elevation · global.css · checklist.md · LP prototype

### 2026-07-23 — No numbered cards / steps by default
- **Surface:** Home `#how` step cards `p.step-num` (“01”)
- **Don't want:** Numbering cards, boxes, or sequential items (01/02/03) unless explicitly asked
- **Do instead:** Title + body only; order implied by layout. Render step numbers only when the user requests them for that surface
- **Status:** promoted
- **Promoted to:** never.md §Components · DESIGN.md step-card · ProductPage + home · checklist.md

### 2026-07-23 — No orphan words in headlines
- **Surface:** Home section `h2.display-lg` — “Same platform. Pick how you buy / it.”
- **Don't want:** Orphan — last line with a lone short word
- **Do instead:** `text-wrap: pretty` on display type; non-breaking space before the last word (`buy&nbsp;it.`); or rewrite. Check display headlines visually at wrap width
- **Status:** promoted
- **Promoted to:** never.md §Typography · DESIGN.md Typography · global.css `.display-*` · checklist.md · home headline fix

### 2026-07-23 — No translate-up on button hover
- **Surface:** Hero CTA `a.btn.btn--primary` (“Explore products”)
- **Don't want:** `translateY(-…)` / lift on button hover
- **Do instead:** Hover changes background, border, and optional purple glow only — button stays in place
- **Status:** promoted
- **Promoted to:** never.md §Motion · DESIGN.md Elevation · Button.astro · checklist.md

### 2026-07-23 — No pill tags above h1
- **Surface:** Home hero `p.badge-pill` (“OPTIDATA CLOUD”)
- **Don't want:** Pill / badge-pill tags stacked above the `h1`
- **Do instead:** Hero opens on the headline. Brand lives in the nav wordmark. Re-add a pill above `h1` only when the user explicitly requests it for that page
- **Status:** promoted
- **Promoted to:** never.md §Layout & hero · Hero.astro (eyebrow/badge-pill prop removed) · DESIGN.md hero-band

### 2026-07-23 — No eyebrows / section kickers
- **Surface:** Global (Home `PRODUCT PORTFOLIO` kicker selected; all section/hero eyebrows)
- **Don't want:** Eyebrows / kickers above headlines (e.g. `PRODUCT PORTFOLIO`, hero badge-pills)
- **Do instead:** Lead with the headline only. Use Manrope display titles. Mono (`typography.kicker`) remains only for machine surfaces — step numbers, table headers, tags — never as a section/hero eyebrow
- **Status:** promoted
- **Promoted to:** never.md §Layout & hero · DESIGN.md Agent contract / Hero · checklist.md · site pages + Hero/ProductPage
