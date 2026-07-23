# Never — Optidata Cloud UI

Hard bans for agents. If a request conflicts, ask before violating.

## Brand & color

- Never introduce a **second brand CTA color** (orange, blue SaaS, green-as-CTA).
- Never use **pure white / cream / warm paper** as the page canvas.
- Never use `{colors.primary}` (#8D0DE3) as large background fills — CTAs and scarce emphasis only.
- Never put **gradient text** on full paragraphs — only short `.grad` spans in display headlines.
- Never invent hex values that are not in DESIGN.md tokens.
- Never use solid lilac (`#ECDFFF` / `#D6B9FE` / `#CBA5FD`) as default heading or body fill — use **white at opacity** tokens (`ink`, `body`, `muted`).
- Never replace Ultravioleta via external palette / font recommenders.

## Typography

- Never use Inter, Roboto, Arial, or system-ui as the **primary** family.
- Never use JetBrains Mono for marketing body copy — tags, code, CIDR, price tables only.
- Never set display headlines at weight 400 (magazine) — display is **700**.
- Never leave **orphans** — a single short word alone on the last line of a headline or display line. Fix with `text-wrap: pretty`, `&nbsp;` before the last word, or rewrite.

## Layout & hero

- Never use **eyebrows** (section kickers / uppercase mono labels above headlines) unless the user **explicitly** asks.
- Never put **pill tags / badge-pills above an `h1`** unless the user **explicitly** asks. Hero starts at the headline.
- Never put **cards, stat strips, floating badges, or promo chips** in the first viewport hero.
- Never ship a hero that still looks like “any cloud SaaS” after removing the nav (brand too weak).
- Never exceed **hero budget**: brand + 1 headline + 1 supporting + 1 CTA group + 1 visual anchor.
- Never use inset hero media cards / tiled collages as the default marketing hero.

## Components

- Never mix radius systems: **buttons = pill**; **inputs = md (12px)**; **cards = 16–22px**.
- Never **number** cards, boxes, or sequential items (01 / 02 / 03) unless the user **explicitly** asks.
- Never add **hover effects on cards** by default (no translate, border change, shadow lift).
- Never put **glow / purple shadow / featured gradient** on cards unless the user **explicitly** asks.
- Never invent **visual hierarchy highlights** on peer cards or text without an explicit request.
- Never put two **filled primary** CTAs in the same group — one primary, secondary is ghost.
- Never use **emoji as structural icons** — SVG only, one family.
- Never ship **fake product UI** (empty div dashboards) or invent logos / metrics / testimonials.
- Never default to generic shadcn/light dashboard chrome on marketing pages.
- Never remove **focus rings** on interactive elements.

## Motion & polish

- Never use **`translateY` / lift-up** on button hover. Hover = color, border, and/or glow only.
- Never add motion that distracts from hierarchy. Prefer 2–3 intentional motions max; honor `prefers-reduced-motion`.
- Never rely on **hover alone** to show clickability — use `cursor: pointer` and clear chrome.

## Process

- Never “finish” substantial UI without a Visual Contract ([practices.md](practices.md)) and [checklist.md](checklist.md).
- Never absorb a user design critique without logging it in [feedback-log.md](feedback-log.md).

---

Add new bans at the top of the relevant section. Source: promote from feedback-log.
