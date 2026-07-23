# Optidata Design

Cursor / Claude Code / Codex skill for the **Optidata Cloud** Ultravioleta design system.

Public marketing and portal UI rules: tokens, hard bans, Visual Contract workflow, and a living feedback log so design critiques become permanent agent rules.

---

## Ask any AI to install this skill

Paste this prompt into Cursor, Claude Code, Codex, ChatGPT, or any coding agent:

```text
Install the Optidata Design skill from https://github.com/victorbenazzi/optidata-design

1. Detect which agent environment I am in (Cursor, Claude Code, or Codex).
2. Clone or download the repo into the correct personal skills directory for that agent:
   - Cursor: ~/.agents/skills/optidata-design (then symlink to ~/.cursor/skills/optidata-design)
   - Claude Code: ~/.claude/skills/optidata-design
   - Codex: ~/.agents/skills/optidata-design (or ~/.codex/skills/optidata-design if that is what this environment uses)
   If I ask for a project-scoped install instead, use:
   - Cursor: .cursor/skills/optidata-design
   - Claude Code: .claude/skills/optidata-design
   - Codex: .agents/skills/optidata-design
3. Ensure the folder contains SKILL.md at its root (plus DESIGN.md, never.md, practices.md, checklist.md, feedback-log.md, sources.md).
4. Confirm installation with the final path(s) and tell me how to invoke it (/optidata-design or by asking for Optidata Ultravioleta UI work).
5. Do not modify the skill files unless I ask. Prefer a fresh clone over a partial copy.
```

---

## Install

Repo: [github.com/victorbenazzi/optidata-design](https://github.com/victorbenazzi/optidata-design)

### Cursor

**Personal (all projects)**

```bash
git clone https://github.com/victorbenazzi/optidata-design.git ~/.agents/skills/optidata-design
ln -sfn ~/.agents/skills/optidata-design ~/.cursor/skills/optidata-design
```

**Project**

```bash
mkdir -p .cursor/skills
git clone https://github.com/victorbenazzi/optidata-design.git .cursor/skills/optidata-design
```

Invoke with `/optidata-design` or ask the agent to follow the Optidata design system.

### Claude Code

**Personal (all projects)**

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/victorbenazzi/optidata-design.git ~/.claude/skills/optidata-design
```

**Project**

```bash
mkdir -p .claude/skills
git clone https://github.com/victorbenazzi/optidata-design.git .claude/skills/optidata-design
```

Restart or start a new Claude Code session. Invoke with `/optidata-design` or natural language about Optidata / Ultravioleta UI.

### Codex

**Personal (all projects)** — Codex commonly loads `~/.agents/skills/`:

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/victorbenazzi/optidata-design.git ~/.agents/skills/optidata-design
```

If your Codex build expects `~/.codex/skills/` instead:

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/victorbenazzi/optidata-design.git ~/.codex/skills/optidata-design
# optional: keep one copy and symlink the other
# ln -sfn ~/.agents/skills/optidata-design ~/.codex/skills/optidata-design
```

**Project**

```bash
mkdir -p .agents/skills
git clone https://github.com/victorbenazzi/optidata-design.git .agents/skills/optidata-design
```

Ask Codex to use the Optidata Design skill / Ultravioleta rules for UI work.

### Update

```bash
cd /path/to/optidata-design && git pull
```

---

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
