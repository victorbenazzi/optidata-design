# Sources — Optidata Design skill

Portable skill. Resolve DESIGN.md in this order:

1. Project `Neocloud/Design/DESIGN.md`
2. Project `Design/DESIGN.md`
3. Project root `DESIGN.md`
4. Skill-bundled [DESIGN.md](DESIGN.md)

## Canonical (read every UI turn)

| File | Role |
|---|---|
| Active `DESIGN.md` (see above) | Tokens + patterns (YAML + prose) |
| `never.md` | Hard bans |
| `practices.md` | Visual Contract, surfaces, CTA, a11y, proof |
| `feedback-log.md` | Critiques awaiting / after promote |
| `checklist.md` | Pre-done gate |
| `SKILL.md` | Agent workflow |

## When used inside optidata.cloud

Also keep in sync when present:

| File | Role |
|---|---|
| `Neocloud/site/src/styles/tokens.css` | CSS variables — must track DESIGN.md |
| `Neocloud/site/src/styles/global.css` | Base type, layout, card patterns |
| `Neocloud/content/*.md` | Page copy (not visual tokens) |
| `Neocloud/foundation/catalog.md` | Names / slugs (IA, not paint) |

When DESIGN.md tokens change, update any project `tokens.css` in the same change set.
