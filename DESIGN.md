---
version: alpha
name: Optidata-Cloud-redesign
description: >
  Plataforma cloud brasileira (Optidata Cloud / OCS) com atmosfera Ultravioleta —
  canvas roxo profundo (#1E002F), texto em branco com opacidade (ink/body/muted)
  e um único voltagem de marca, Optidata Purple (#8D0DE3), reservado a CTAs
  primários e ênfase da wordmark. Display e body em Manrope (700 no hero, 600 em
  títulos de componente, 400/500 no corpo) com letter-spacing negativo no display.
  JetBrains Mono em tags, tabelas de preço e superfícies de código/CLI. Cards usam
  borda hairline lilás, cantos generosos (16–22px) e elevação por contraste de
  superfície — sombra/glow só se featured for pedido. Ritmo de seção ~110px.
  Assinatura visual — radial glow violeta + grid sutil no hero.

colors:
  primary: "#8D0DE3"
  primary-active: "#9B27F0"
  primary-glow: "#AF63FD"
  ink: "rgba(255, 255, 255, 0.92)"
  body: "rgba(255, 255, 255, 0.72)"
  body-strong: "rgba(255, 255, 255, 0.88)"
  muted: "rgba(255, 255, 255, 0.55)"
  muted-soft: "rgba(255, 255, 255, 0.40)"
  hairline: "rgba(203, 165, 253, 0.14)"
  hairline-soft: "rgba(203, 165, 253, 0.08)"
  hairline-strong: "rgba(175, 99, 253, 0.45)"
  canvas: "#1E002F"
  canvas-deep: "#0B0019"
  canvas-soft: "#3F026A"
  surface-card: "rgba(63, 2, 106, 0.35)"
  surface-card-solid: "#3F026A"
  surface-elevated: "rgba(11, 0, 25, 0.55)"
  surface-strong: "rgba(93, 5, 153, 0.30)"
  mid: "#5D0599"
  on-primary: "#ffffff"
  gradient-start: "#AF63FD"
  gradient-mid: "#CBA5FD"
  gradient-end: "#ECD9FF"
  semantic-error: "#F07178"
  semantic-success: "#3DDC97"
  semantic-warning: "#F5C542"
  semantic-info: "#5B9FFF"

typography:
  display-mega:
    fontFamily: "'Manrope', system-ui, sans-serif"
    fontSize: 72px
    fontWeight: 700
    lineHeight: 1.04
    letterSpacing: -0.03em
  display-lg:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 46px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.025em
  display-md:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.15
    letterSpacing: -0.02em
  display-sm:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.015em
  title-md:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 18px
    fontWeight: 600
    lineHeight: 1.35
    letterSpacing: -0.01em
  title-sm:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 16px
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: 0
  body-md:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0
  body-lg:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0
  body-sm:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: 0
  caption:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 13px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0
  kicker:
    fontFamily: "'JetBrains Mono', monospace"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0.14em
    textTransform: uppercase
  code:
    fontFamily: "'JetBrains Mono', 'Fira Code', monospace"
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0
  button:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 15px
    fontWeight: 600
    lineHeight: 1.0
    letterSpacing: 0
  nav-link:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: 0
  price:
    fontFamily: "'Manrope', sans-serif"
    fontSize: 40px
    fontWeight: 700
    lineHeight: 1.0
    letterSpacing: -0.03em

rounded:
  none: 0px
  xs: 6px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 18px
  xxl: 22px
  hero-cta: 28px
  pill: 9999px
  full: 9999px

spacing:
  xxs: 4px
  xs: 8px
  sm: 12px
  base: 16px
  md: 20px
  lg: 24px
  xl: 32px
  xxl: 48px
  section: 110px

components:
  top-nav:
    backgroundColor: "rgba(11, 0, 25, 0.72)"
    textColor: "{colors.body}"
    typography: "{typography.nav-link}"
    height: 68px
    backdropFilter: blur(14px)
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: 12px 26px
    height: 44px
  button-primary-active:
    backgroundColor: "{colors.primary-active}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.pill}"
  button-ghost:
    backgroundColor: transparent
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: 11px 25px
    height: 44px
  button-secondary:
    backgroundColor: "{colors.surface-elevated}"
    textColor: "{colors.ink}"
    typography: "{typography.button}"
    rounded: "{rounded.pill}"
    padding: 12px 26px
    height: 44px
  hero-band:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.ink}"
    typography: "{typography.display-mega}"
    padding: 140px 0 80px
  product-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.title-md}"
    rounded: "{rounded.xl}"
    padding: 30px 28px
  pricing-tier-card:
    backgroundColor: "{colors.surface-elevated}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xxl}"
    padding: 38px 34px
  pricing-tier-featured:
    backgroundColor: "rgba(93, 5, 153, 0.45)"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xxl}"
    padding: 38px 34px
  console-mockup-card:
    backgroundColor: "{colors.canvas-deep}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    padding: 0
  console-pane:
    backgroundColor: "{colors.canvas}"
    textColor: "{colors.body}"
    typography: "{typography.code}"
    rounded: "{rounded.md}"
    padding: 16px
  step-card:
    backgroundColor: "rgba(11, 0, 25, 0.45)"
    textColor: "{colors.ink}"
    typography: "{typography.title-sm}"
    rounded: "{rounded.lg}"
    padding: 26px 24px
  feature-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.ink}"
    typography: "{typography.title-md}"
    rounded: "{rounded.xl}"
    padding: 28px
  badge-pill:
    backgroundColor: "{colors.surface-strong}"
    textColor: "{colors.muted}"
    typography: "{typography.kicker}"
    rounded: "{rounded.pill}"
    padding: 7px 16px
  tag-chip:
    backgroundColor: "{colors.surface-strong}"
    textColor: "{colors.muted}"
    typography: "{typography.code}"
    rounded: "{rounded.xs}"
    padding: 4px 10px
  text-input:
    backgroundColor: "{colors.surface-elevated}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.md}"
    padding: 12px 16px
    height: 44px
  calc-panel:
    backgroundColor: "{colors.surface-elevated}"
    textColor: "{colors.ink}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xxl}"
    padding: 32px
  cta-band:
    backgroundColor: "{colors.canvas-deep}"
    textColor: "{colors.ink}"
    typography: "{typography.display-lg}"
    padding: 90px 60px 100px
  testimonial-card:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.body}"
    typography: "{typography.body-md}"
    rounded: "{rounded.xl}"
    padding: 28px
  footer:
    backgroundColor: "{colors.canvas-deep}"
    textColor: "{colors.body}"
    typography: "{typography.body-sm}"
    padding: 48px 32px
  footer-link:
    backgroundColor: transparent
    textColor: "{colors.body}"
    typography: "{typography.body-sm}"
---

## Agent contract

This file is the **token source of truth** for Optidata Cloud UI.

AI agents working on Neocloud visuals must load the skill **`optidata-design`** (`.cursor/skills/optidata-design/SKILL.md`) and also read:

- `.cursor/skills/optidata-design/never.md` — hard bans
- `.cursor/skills/optidata-design/feedback-log.md` — latest critiques
- `.cursor/skills/optidata-design/checklist.md` — done gate
- `Neocloud/site/src/styles/tokens.css` — CSS mirror of these tokens

When the human says what they **don't want**, agents log it, fix the UI, then **promote** the rule into `never.md` and/or this file — never leave taste as a one-off patch.

**Eyebrows:** Do **not** render section kickers or hero badge-pills by default. Lead with the headline. **Text:** white-at-opacity (`ink` / `body` / `muted`) — not solid lilac. JetBrains Mono only for machine surfaces (table `th`, tags, CLI). No step numbers on cards unless explicitly asked.

**White-ink:** Headings and paragraphs are `rgba(255,255,255,…)` via tokens. Opacity keeps Ultravioleta soft without muddy lilac readability.

---

## Overview

O redesign da **Optidata Cloud** lê como uma marca de infraestrutura confiante e contemporânea: fundo Ultravioleta profundo, tipografia Manrope com peso sólido no display, e um único voltagem de ação — o roxo Nubank-core `#8D0DE3` — usado com parcimônia em CTAs e na ênfase da wordmark.

O canvas dominante é **Ultravioleta Primary** (`{colors.canvas}` — #1E002F), com profundidade máxima em **UV Black** (`{colors.canvas-deep}` — #0B0019) e superfícies elevadas em **UV Deep** (`{colors.canvas-soft}` — #3F026A). **Texto** usa branco com opacidade — display/títulos `{colors.ink}` (0.92), corpo `{colors.body}` (0.72), metadados `{colors.muted}` (0.55) — não lilás sólido. Hairlines e atmosfera continuam lilás.

**Manrope** carrega display e body (400–800). Display de marketing usa 700 com tracking negativo (−0.025em a −0.03em). Títulos de componente em 600. JetBrains Mono fica restrito a kickers uppercase, tags de produto, tabelas de preço, IPs/CIDR e blocos CLI.

A assinatura atmosférica é o **radial glow** violeta (primary / mid) + **grid hairline** lilás mascarado no hero — nunca flat single-color, nunca cream/white editorial.

**Key Characteristics:**
- Canvas Ultravioleta escuro (`#1E002F`), não cream nem slate genérico.
- Texto **white-ink**: branco com opacidade (não lilás sólido).
- Único CTA brand: `{colors.primary}` (#8D0DE3). Escasso.
- Display Manrope 700 (não 400 editorial). Voz de produto cloud, não revista.
- CTAs em pill (`{rounded.pill}`); cards em 16–22px.
- Depth por contraste de superfície + hairline lilás; sombra roxa **só** em featured **quando pedido** ou no hover de CTA.
- Ritmo de seção `{spacing.section}` (110px).
- Gradient de texto no hero: `{colors.gradient-start}` → `{colors.gradient-mid}` → `{colors.gradient-end}` (opt-in em trechos `.grad`).

## Colors

### Brand & Accent
- **Optidata Purple** (`{colors.primary}` — #8D0DE3): CTA primário, chip de plano featured, ênfase da wordmark. Usar com parcimônia.
- **Optidata Purple Active** (`{colors.primary-active}` — #9B27F0): Hover/press do CTA (mantém contraste AA com branco).
- **Violet Bright** (`{colors.primary-glow}` — #AF63FD): Glow, focus ring, acentos pontuais (não usar para numerar steps por padrão).

### Surface
- **Canvas** (`{colors.canvas}` — #1E002F): Piso da página — dominante absoluto.
- **Canvas Deep** (`{colors.canvas-deep}` — #0B0019): Bandas de produto, footer, fundo de mockups.
- **Canvas Soft** (`{colors.canvas-soft}` — #3F026A): Superfície elevada sólida, ícones de card.
- **Mid** (`{colors.mid}` — #5D0599): Gradientes de featured, fundo de tags.
- **Surface Card** (`{colors.surface-card}` — rgba(63,2,106,0.35)): Cards de produto (gradient translúcido permitido).
- **Surface Elevated** (`{colors.surface-elevated}` — rgba(11,0,25,0.55)): Planos de preço, painéis de calculadora.
- **Surface Strong** (`{colors.surface-strong}` — rgba(93,5,153,0.30)): Badges e chips.

### Hairlines
- **Hairline** (`{colors.hairline}` — rgba(203,165,253,0.14)): Borda padrão de card / divider.
- **Hairline Soft** (`{colors.hairline-soft}` — rgba(203,165,253,0.08)): Linhas internas de tabela.
- **Hairline Strong** (`{colors.hairline-strong}` — rgba(175,99,253,0.45)): Borda do plano featured (e hover de card **somente** se pedido explícito).

### Text
- **Ink** (`{colors.ink}` — rgba(255,255,255,0.92)): Display, títulos, ênfase.
- **Body** (`{colors.body}` — rgba(255,255,255,0.72)): Parágrafos e supporting copy.
- **Body strong** (`{colors.body-strong}` — rgba(255,255,255,0.88)): Ênfase leve no corpo.
- **Muted** (`{colors.muted}` — rgba(255,255,255,0.55)): Labels, microcopy, nav secondary.
- **Muted soft** (`{colors.muted-soft}` — rgba(255,255,255,0.40)): Disabled / placeholder.
- **On Primary** (`{colors.on-primary}` — #ffffff): Texto sobre CTA roxo.

Não usar `#ECDFFF` / `#D6B9FE` / `#CBA5FD` como fill de texto de marketing — esses hex ficam para hairline/atmosfera/gradiente de destaque, não para parágrafos.

### Gradient (hero highlight)
- **Start** (`{colors.gradient-start}` — #AF63FD)
- **Mid** (`{colors.gradient-mid}` — #CBA5FD)
- **End** (`{colors.gradient-end}` — #ECD9FF)

Usar só em trechos de headline (`.grad`), nunca como fundo de página inteira.

### Semantic
- **Success** (`{colors.semantic-success}` — #3DDC97): Status online, deploy ok.
- **Error** (`{colors.semantic-error}` — #F07178): Validação, falha.
- **Warning** (`{colors.semantic-warning}` — #F5C542): Quotas, avisos de billing.
- **Info** (`{colors.semantic-info}` — #5B9FFF): Tips e estados informativos.

## Typography

### Font Family
**Manrope** (Google Fonts, weights 400 / 500 / 600 / 700 / 800) é a família única de display + body. Fallback: `system-ui, sans-serif`. Superfícies técnicas usam **JetBrains Mono** (400 / 500).

### Hierarchy

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---|---|---|---|---|
| `{typography.display-mega}` | 72px (clamp 2.6–4.8rem) | 700 | 1.04 | −0.03em | Hero h1 |
| `{typography.display-lg}` | 46px (clamp 1.9–2.9rem) | 700 | 1.1 | −0.025em | Section heads |
| `{typography.display-md}` | 32px | 700 | 1.15 | −0.02em | Sub-section / pricing name |
| `{typography.display-sm}` | 24px | 600 | 1.2 | −0.015em | Group titles |
| `{typography.title-md}` | 18–20px | 600 | 1.35 | −0.01em | Card titles |
| `{typography.title-sm}` | 16px | 600 | 1.4 | 0 | Step / list labels |
| `{typography.body-lg}` | 18px | 400 | 1.6 | 0 | Hero subhead |
| `{typography.body-md}` | 16px | 400 | 1.6 | 0 | Default body |
| `{typography.body-sm}` | 14px | 400 | 1.55 | 0 | Footer, notes |
| `{typography.caption}` | 13px | 500 | 1.4 | 0 | Micro labels |
| `{typography.kicker}` | 12px | 500 | 1.4 | 0.14em | Section labels — JetBrains Mono, uppercase |
| `{typography.code}` | 13px | 400 | 1.5 | 0 | Code, tags, tabular mono |
| `{typography.button}` | 15px | 600 | 1.0 | 0 | CTA labels |
| `{typography.nav-link}` | 14px | 500 | 1.4 | 0 | Top nav |
| `{typography.price}` | 40px | 700 | 1.0 | −0.03em | Preço em cards / calc |

### Principles
- **Display em 700.** Marca cloud com presença; não magazine 400.
- **Tracking negativo só no display** (−0.015em a −0.03em).
- **Manrope em tudo que é humano**; JetBrains Mono só no que é máquina (kicker, tag, CLI, CIDR, preço tabular).
- **Números de preço e stats** com `font-variant-numeric: tabular-nums`.
- **Sem órfãos.** Nunca deixar uma palavra curta sozinha na última linha de um headline (widow/orphan). Use `text-wrap: pretty` nos displays; se ainda órfão, `&nbsp;` antes da última palavra ou reescreva.

### Load
```html
<link href="https://fonts.googleapis.com/css2?family=Manrope:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
```

## Layout

### Spacing System
- **Base unit:** 4px.
- **Tokens:** `{spacing.xxs}` 4 · `{spacing.xs}` 8 · `{spacing.sm}` 12 · `{spacing.base}` 16 · `{spacing.md}` 20 · `{spacing.lg}` 24 · `{spacing.xl}` 32 · `{spacing.xxl}` 48 · `{spacing.section}` 110.
- **Section padding:** 110px vertical.
- **Wrap:** max-width 1180px, padding horizontal 32px.

### Grid & Container
- Max content: ~1180px.
- Product grid: 3-up desktop → 2-up tablet → 1-up mobile.
- Pricing: 2-up (Balanced / Dedicated) no desktop.
- Deploy steps: 3-up.
- Footer: flex space-between (ou 4-col em portal expandido).

### Whitespace Philosophy
Respiro generoso entre seções (110px), cards próximos entre si (16–22px gap). Hero ocupa viewport completo com composição única — marca, 1 headline, 1 supporting, 1 grupo de CTA, 1 âncora visual (glow/grid ou mockup de console). Sem stat strips, chips flutuantes ou cards no primeiro viewport além do necessário.

## Elevation & Depth

Depth vem de **contraste de superfície + hairline lilás**, não de multi-layer shadow genérico.

| Level | Treatment | Use |
|---|---|---|
| Flat (canvas) | `{colors.canvas}` | Body bands |
| Deep band | `{colors.canvas-deep}` | Products, deploy, footer |
| Card | `{colors.surface-card}` + 1px hairline | Product / feature cards |
| Elevated | `{colors.surface-elevated}` + hairline | Pricing, calc, steps |
| Featured | gradient mid→canvas + `{colors.hairline-strong}` + soft purple shadow | Plano destacado |
| Nav | rgba(11,0,25,0.72) + blur(14px) | Top nav sticky |

### Decorative Depth
- **Hero radials:** ellipse glow em `{colors.primary}` / `{colors.mid}` sobre o canvas.
- **Hero grid:** linhas `rgba(203,165,253,0.05)` em 56px, mascaradas com radial.
- **CTA hover:** background → `{colors.primary-active}` + optional `box-shadow: 0 12px 32px rgba(141,13,227,0.45)`. **No `translateY` / lift.**
- **Card hover:** **Off by default.** No translate, no border change, no shadow on hover unless the human explicitly asks for that surface.

## Shapes

### Border Radius Scale

| Token | Value | Use |
|---|---|---|
| `{rounded.none}` | 0px | Reservado |
| `{rounded.xs}` | 6px | Tags / chips |
| `{rounded.sm}` | 8px | Nav link hover |
| `{rounded.md}` | 12px | Inputs, ícones de card, panes |
| `{rounded.lg}` | 16px | Step cards, console panes |
| `{rounded.xl}` | 18px | Product / feature cards |
| `{rounded.xxl}` | 22px | Pricing tiers, calc panel |
| `{rounded.hero-cta}` | 28px | Top do CTA band (deploy) |
| `{rounded.pill}` | 9999px | Todos os botões, badge hero |
| `{rounded.full}` | 9999px | Avatars, dots |

## Components

### Top Navigation

**`top-nav`** — Sticky. Background `rgba(11,0,25,0.72)` + `backdrop-filter: blur(14px)`, border-bottom 1px `{colors.hairline}` suave, height 68px. Wordmark Manrope 700 à esquerda (`Optidata` + em em `{colors.primary-glow}`). Links `{typography.nav-link}` em `{colors.body}`; CTA compacto `button-primary` à direita.

### Buttons

**`button-primary`** — CTA signature. Background `{colors.primary}`, text `{colors.on-primary}`, type `{typography.button}`, padding 12×26, height 44px, `{rounded.pill}`. Hover → `{colors.primary-active}` + purple glow. **Sem translate/lift.**

**`button-primary-active`** — Press/hover filled.

**`button-ghost`** — Transparent, 1px border `{colors.ink}` a 30% opacity, text `{colors.ink}`, same pill geometry.

**`button-secondary`** — Surface elevated + hairline; para ações secundárias em bandas escuras.

### Hero

**`hero-band`** — min-height 100vh, padding 140×0×80, background canvas + radials + grid mask. Ordem padrão: h1 (`display-mega`, trecho `.grad` opcional) → body-lg supporting → CTAs (primary + ghost). **Sem eyebrow, sem badge-pill acima do h1** a menos que pedido explicitamente. Sem cards, stats ou overlays flutuantes no primeiro viewport.

**`badge-pill`** — Componente opt-in. **Proibido acima de h1 por padrão.** Só quando o humano pedir explicitamente nessa superfície. Kicker mono + dot pulse `{colors.primary-glow}`. Background surface-strong, border hairline, `{rounded.pill}`.
### Console Mockups (produto)

**`console-mockup-card`** — Mock do Optidata Cloud Console. Background `{colors.canvas-deep}`, `{rounded.lg}`, 1px hairline, panes edge-to-edge. Substitui o “IDE mockup” do template Cursor: sidebar de projetos + painel de instâncias + billing snippet.

**`console-pane`** — Pane interno. Background `{colors.canvas}`, type `{typography.code}`, padding 16px, `{rounded.md}`.

### Cards

**`product-card`** — Ícone 42×42 em `{colors.canvas-soft}` → título `{typography.title-md}` → body-sm → `tag-chip`. Background surface-card (gradient 160deg permitido), `{rounded.xl}`, padding 30×28, hairline.

**`feature-card`** — Mesma família do product-card; para features 4–6 em páginas de produto.

**`step-card`** — Deploy / how-it-works cards. Título title-sm, body-sm. **Sem número (01/02/03) por padrão** — só se o humano pedir explicitamente. Ordem = posição no grid.

**`testimonial-card`** — Quote. Surface-card + hairline; sem aspas decorativas gigantes.

### Pricing & Calculator

**`pricing-tier-card`** — Surface elevated, `{rounded.xxl}`, padding 38×34. Nome display-sm, preço `{typography.price}`, tabela com th em kicker mono e td tabular.

**`pricing-tier-featured`** / **`card--featured`** — Opt-in only. Gradient mid→canvas, border `{colors.hairline-strong}`, soft purple glow. **Nunca aplicar por julgamento do agente** (ex.: destacar Private Cloud vs Self-serve sem pedido). Peers no mesmo grid ficam iguais até o humano pedir ênfase.

**`calc-panel`** — Painel público da calculadora. Mesma geometria do pricing card; inputs `text-input`; breakdown em mono; CTA primary só no final do fluxo.

### Forms & Tags

**`text-input`** — Surface elevated, text ink, `{rounded.md}`, height 44px, focus ring 2px `{colors.primary-glow}` offset 3px.

**`tag-chip`** — Mono 0.7–0.8rem, `{rounded.xs}`, surface-strong, text muted. Labels de produto (“tráfego interno privado”, “NVMe”, etc.).

### CTA / Footer

**`cta-band`** — Bloco deploy final. Top radius `{rounded.hero-cta}`, radial glow bottom, border hairline-strong. Headline display-lg centrado + steps 3-up + primary CTA grande.

**`footer`** — Canvas deep, hairline top, body-sm em `{colors.body}`.

**`footer-link`** — Transparent; hover → `{colors.ink}`.

## Do's and Don'ts

### Do
- Reservar `{colors.primary}` (#8D0DE3) para CTAs primários e ênfase da wordmark.
- Usar **Manrope** em display e body; **JetBrains Mono** só em superfícies técnicas.
- Manter canvas Ultravioleta (`#1E002F`) — nunca pure white / cream editorial.
- CTAs sempre pill; cards 16–22px.
- Uma composição no primeiro viewport: marca + headline + supporting + CTAs + âncora visual.
- Referenciar tokens `{token.refs}` — nunca hex solto no código de UI nova.

### Don't
- Não introduzir segunda cor de ação (laranja, azul “SaaS”, verde de CTA).
- Não usar Inter / Roboto / Arial / system-ui como família principal.
- Não copiar o cream canvas do template Cursor — a estrutura sim, a paleta não.
- Não colocar cards, stat strips, chips flutuantes ou overlays no hero.
- Não usar drop shadows multi-camada em todo card — sombra/glow roxo **somente** se featured for pedido explícito, ou no hover de CTA.
- Não inventar destaque visual entre cards peers sem pedido (Private Cloud vs Self-serve iguais até o humano pedir ênfase).
- Não aplicar gradient de texto em parágrafos inteiros.
- Não misturar radius: botões são pill; inputs são md (12px).

## Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 640px | Hero h1 clamp ↓; product grid 1-up; pricing 1-up; steps 1-up; nav hamburger; wrap padding 20px. |
| Tablet | 640–1024px | Product 2-up; pricing 2-up comprimido; steps 3-up apertado. |
| Desktop | 1024–1280px | Grid 3-up; hero full; console mockup multi-pane. |
| Wide | > 1280px | Content cap 1180px. |

### Touch Targets
- Primary / ghost CTA ≥ 44px height (AAA).
- Nav links padding ≥ 12px vertical.

### Collapsing Strategy
- Top nav → hamburger abaixo de 768px.
- Console mockup multi-pane → single pane preview no mobile.
- Product grid: 3 → 2 → 1.
- Pricing: 2 → 1 (featured primeiro).

## Iteration Guide

1. Um componente por vez; variants como entradas separadas em `components:`.
2. CTAs → `{rounded.pill}`. Cards → `{rounded.xl}` / `{rounded.xxl}`.
3. Sempre `{token.refs}` — nunca hex inline em UI nova.
4. Hover de botão: cor / borda / glow — **nunca** `translateY`. Cards **sem hover** por padrão.
5. Manrope 700 display · 600 titles · 400/500 body. JetBrains Mono em kickers/código.
6. Optidata Purple permanece escasso.
7. Hero sem clutter; seções com um job, um headline, uma supporting sentence.
8. Antes de qualquer UI: ler este `DESIGN.md` e casar tokens, type scale e patterns.

## Known Gaps

- Wordmark oficial / logo SVG ainda não versionados neste repo — usar wordmark tipográfico Manrope 700 até o asset final.
- Tokens de tema claro (se o console exigir light mode) fora de escopo desta versão alpha.
- Motion timings (reveal 0.7s, pulse do badge) parcialmente definidos na LP; padronizar em motion tokens numa iteração seguinte.
- Estados de formulário além de focus (error/success filled) derivados dos semantic colors — validar com QA de contraste.
- Componentes exclusivos do console autenticado (tabelas densas, side nav, resource quotas) devem estender este sistema, não criar paleta paralela.
