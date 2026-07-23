# Optidata Design

Cursor Agent Skill for the **Optidata Cloud** Ultravioleta design system.

Public marketing/portal UI rules: tokens, hard bans, Visual Contract workflow, and a living feedback log so critiques become permanent agent rules.

## Install (Cursor)

### Personal (all projects)

```bash
git clone https://github.com/victorbenazzi/optidata-design.git ~/.agents/skills/optidata-design
ln -sfn ~/.agents/skills/optidata-design ~/.cursor/skills/optidata-design
```

### Project

```bash
mkdir -p .cursor/skills
git clone https://github.com/victorbenazzi/optidata-design.git .cursor/skills/optidata-design
```

Or copy the folder into `.cursor/skills/optidata-design/`.

## Invoke

In Cursor: `/optidata-design` or ask the agent to follow the Optidata design system when doing UI work.

## Files

| File | Role |
|---|---|
| `SKILL.md` | Workflow + authority order |
| `DESIGN.md` | Ultravioleta tokens + patterns |
| `never.md` | Hard bans |
| `practices.md` | Visual Contract, surfaces, CTA, a11y |
| `checklist.md` | Done gate |
| `feedback-log.md` | Critique → promote pipeline |
| `sources.md` | Resolution map for DESIGN.md |

## Design source resolution

1. Project `Neocloud/Design/DESIGN.md` or `Design/DESIGN.md` or root `DESIGN.md`
2. Else skill-bundled `DESIGN.md`

## License

MIT
