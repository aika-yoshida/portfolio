---
name: Aika Yoshida Portfolio
description: An editorial case-file portfolio for a sales-to-UX/CX career changer — ink, cream, and one borrowed accent color per case.
colors:
  ink: "#141310"
  ink-soft: "#3a3833"
  mute: "#6f6a61"
  line: "#e0ddd4"
  page: "#f5f3ee"
  card: "#ffffff"
  accent-index: "#7c2cd6"
  accent-index-deep: "#5c1ba3"
  accent-index-soft: "#f1e6fb"
  accent-index-light: "#d9bdfb"
  accent-clinic: "#2f6fb0"
  accent-clinic-deep: "#1f4d80"
  accent-clinic-soft: "#e8f1fa"
  accent-clinic-light: "#b7d4ec"
  accent-wedding: "#b8577a"
  accent-wedding-deep: "#8a3457"
  accent-wedding-soft: "#fbeaf0"
  accent-wedding-light: "#eec0d3"
  accent-tohto: "#2c3a63"
  accent-tohto-deep: "#1c2745"
  accent-tohto-soft: "#e9edf5"
  accent-tohto-light: "#aab7d1"
  accent-penelope: "#a33b2e"
  accent-penelope-deep: "#7c2418"
  accent-penelope-soft: "#f7e8e2"
  accent-penelope-light: "#e7b6a3"
typography:
  display:
    fontFamily: "Inter, Noto Sans JP, Hiragino Kaku Gothic ProN, sans-serif"
    fontSize: "clamp(23px, 3.2vw, 46px)"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-.015em"
  headline:
    fontFamily: "Inter, Noto Sans JP, Hiragino Kaku Gothic ProN, sans-serif"
    fontSize: "clamp(18.5px, 2.6vw, 26px)"
    fontWeight: 800
    lineHeight: 1.25
    letterSpacing: "-.01em"
  body:
    fontFamily: "Inter, Noto Sans JP, Hiragino Kaku Gothic ProN, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.85
    letterSpacing: ".01em"
  label:
    fontFamily: "Inter, Noto Sans JP, Hiragino Kaku Gothic ProN, sans-serif"
    fontSize: "11px"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: ".14em"
rounded:
  pill: "999px"
  lg: "26px"
  md: "18px"
  sm: "12px"
  xs: "8px"
spacing:
  s1: "8px"
  s2: "16px"
  s3: "24px"
  s4: "32px"
  s5: "40px"
  s6: "48px"
  s7: "64px"
  s8: "80px"
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "#ffffff"
    rounded: "{rounded.pill}"
    padding: "13px 26px"
  button-primary-hover:
    backgroundColor: "{colors.accent-index}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "13px 26px"
  button-ghost-hover:
    backgroundColor: "{colors.ink}"
    textColor: "#ffffff"
  feature-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.lg}"
    padding: "38px 36px"
  tag-chip:
    backgroundColor: "{colors.page}"
    textColor: "{colors.ink-soft}"
    rounded: "{rounded.pill}"
    padding: "5px 14px"
---

# Design System: Aika Yoshida Portfolio

## 1. Overview

**Creative North Star: "The Case File"**

Every page reads like a folder pulled from a records office: ink-black type on warm cream paper, a single stamped accent color per case, borders instead of shadows, and numbered rows instead of decorative cards. Nothing performs; the layout gets out of the way of the argument each page is making — that a sales background is a design asset, proven case by case rather than claimed once on a hero.

The system explicitly rejects the generic AI-portfolio grammar: no gradient text, no tiny tracked eyebrows stacked above every section, no glassmorphism, no identical icon-plus-heading card grids, no hero-metric templates. Where the site needs emphasis it uses one accent color and plain, specific language — numbers, roles, timeframes — never adjectives doing the work numbers should do.

**Key Characteristics:**
- Ink (#141310) on cream (#f5f3ee), one accent color per page, everything else neutral.
- Flat at rest; shadow appears only as a hover response on clickable cards.
- Pill buttons and pill tags are the only rounded-to-circle shapes; content containers use a shared 26/18/12px radius scale, never fully square, never a stripe border.
- Bilingual type: Inter carries Latin/UI text, Noto Sans JP carries Japanese prose, in the same weight scale.

## 2. Colors

Ink and cream stay fixed across every page; only the accent swaps, page by page.

### Primary
- **Editorial Purple** (`#7c2cd6`, deep `#5c1ba3`): the site-wide identity accent on `index.html` — nav CTA hover, links, the works-grid hover glow, `<em>` emphasis in the hero headline.

### Secondary — The Borrowed Palette
Each case study borrows one accent from the client's own world instead of reusing the site's purple. The shared ink/cream/line neutrals prove it's one system; the swapped accent proves each case was designed on its own terms.
- **Clinical Blue** (`#2f6fb0`, deep `#1f4d80`): Patient Record Management case study — evokes hospital signage and clinical calm.
- **Rose Quartz** (`#b8577a`, deep `#8a3457`): Wedding Venue Redesign — warmer, celebratory, without tipping into pastel-cute.
- **Ceremonial Navy** (`#2c3a63`, deep `#1c2745`): 東都典範 (funeral services) — sober, formal, trustworthy.
- **Terracotta** (`#a33b2e`, deep `#7c2418`): Penelope a casa — an Italian trattoria's warmth, party-and-home in one hue.

### Neutral
- **Ink** (`#141310`): all body text, headings, the dark full-bleed statement bands and contact panel background.
- **Ink Soft** (`#3a3833`): secondary body copy, subtitles, description text under headlines.
- **Mute** (`#6f6a61`): labels, metadata, timestamps — anything that shouldn't compete with body copy.
- **Line** (`#e0ddd4`): every hairline border, section divider, and card outline.
- **Page** (`#f5f3ee`): the body background and tag-chip fill.
- **Card** (`#ffffff`): elevated content surfaces (feature cards, callout boxes on some pages).

### Named Rules
**The Borrowed Palette Rule.** A case study's accent color comes from its client's world, not the site's default purple. Ink, cream, line, and card neutrals never change; only the accent — and its `-deep`, `-soft`, `-light` steps — swaps per page. Consistency lives in the shared structure, not a shared color.

**The One Voice Rule.** Exactly one accent color is active on any given page. It never mixes with another page's accent, and it never appears at more than a small fraction of the surface — links, one button state, small tags, and the radial glow accents in dark panels.

## 3. Typography

**Display Font:** Inter (with Noto Sans JP, Hiragino Kaku Gothic ProN, sans-serif fallback)
**Body Font:** Inter, Noto Sans JP, Hiragino Kaku Gothic ProN, sans-serif
**Label/Mono Font:** same stack, used at small size with wide tracking instead of a distinct mono face

**Character:** One family carries the whole system in varied weights (400 body, 600–700 subheads, 800 for section titles), so Latin and Japanese text sit at the same visual weight without a jarring font swap mid-sentence.

### Hierarchy
- **Display** (700, `clamp(28px,4.2vw,46px)` on the home hero / `clamp(26px,4vw,40px)` on case-study titles, 1.1–1.16 line-height, `-.015em` tracking): hero headlines and case-study `h1.title`; `<em>` spans inside them carry the accent color.
- **Headline** (800, `clamp(18.5px,2.6vw,26px)`–`clamp(23px,3.2vw,34px)`, `-.01em` to `-.015em`): section titles (`h2.big`, `.caps-head h3`) and step headings (`.crow h4`).
- **Title** (700, 18.5px, 1.6 line-height): feature-card headings (`.feature .body h4`) and callout stat headlines.
- **Body** (400, 14–15px, 1.85 line-height): all paragraph copy; capped near 620–640px measure (`.sec-lead`, `.subtitle`) so Japanese prose doesn't run past a comfortable line length.
- **Label** (600–700, 11–11.5px, `.1em`–`.16em` tracking, uppercase): the `.mono`/`.idx`/`.lab`/`.tag` family — section indices, works-card meta, tag chips. Always small and quiet, never a standalone attention-grabber.

### Named Rules
**The No-Eyebrow Rule.** Section labels (`01 — Selected Works`, `Now & Next`) sit as small tracked metadata beside a heading, never as a centered standalone kicker above it. They're a page index, not a decorative device — never let one eyebrow style repeat identically above every section.

## 4. Elevation

Flat by default. Every card, callout, and panel is built from a fill color plus a 1px `--line` border or a solid ink background — no ambient drop shadows at rest. Shadow exists only as a response to interaction: the works-grid feature cards and thumbnail cards lift with a soft shadow and a `translateY(-3px/-4px)` on hover, signaling "this is clickable" rather than implying permanent depth.

### Shadow Vocabulary
- **hover-lift** (`box-shadow: 0 22px 46px -28px rgba(20,19,16,.3)`): feature-card hover state on the works grid.
- **thumb-lift** (`box-shadow: 0 18px 36px -18px rgba(0,0,0,.55)`): works-grid thumbnail/screenshot mockups, at rest (they simulate a physical screenshot, not an interactive lift) and on card hover.

### Named Rules
**The Flat-By-Default Rule.** Surfaces are flat at rest — border and fill only. A shadow appears exclusively as a hover response on something clickable; it is never used to fake depth on static content.

## 5. Components

### Buttons
- **Shape:** full pill (`border-radius: 999px`), 44px minimum height, 13–26px horizontal padding.
- **Primary (solid):** ink background, white text; hover swaps to the page's accent color (`.btn.solid:hover`).
- **Ghost (outline):** 1px ink border, ink text, transparent fill; hover inverts to solid ink with white text.
- **Hover/Focus:** all state changes are background-color transitions only (`.15s`); focus-visible adds a 2px accent outline with 3px offset — never removed, never replaced with a color-only cue.

### Chips / Tags
- **Style:** 1px `--line` border, `--page` background, `--ink-soft` text, full pill radius, 11px uppercase-adjacent label type.
- **Signature variant:** the `.pdf` tag swaps border and text to the page's accent color, marking "this case includes a downloadable proposal" without adding a new shape.

### Cards / Containers
- **Corner Style:** 26px for primary content cards (case-study `.card`), 18px for callouts/pdfboxes, 12–16px for smaller inline items — one shared descending scale, never ad hoc.
- **Background:** white `--card` or `--page` tint; `.card.dark` inverts to ink with cream text for a full-bleed statement moment.
- **Shadow Strategy:** none at rest (see Elevation); reserved for the works-grid hover state only.
- **Border:** 1px `--line`, the system's only structural line — never a colored side-stripe.
- **Internal Padding:** generous, `--s4`–`--s6` (32–52px+) on primary cards; tighter `--s3` (24px) on inline items.

### Inputs / Fields
- **Style:** 1px `--line` border, white background, 10px radius, 44px min-height (the password gate input is the only current instance).
- **Focus:** 2px accent outline, 2px offset — matches the global focus-visible treatment exactly.

### Navigation
- **Style:** sticky topbar, translucent cream (`rgba(245,243,238,.9)`) with backdrop blur, 1px bottom border. Nav links are 13px/600 weight, ink-soft, with a 44px-min-height tap target; hover shifts to the page's accent color. The primary CTA (`.cta`) is a solid ink pill that inverts to accent on hover. Mobile (<640px) drops the CTA and tightens link padding rather than collapsing into a hamburger.

### Feature Card (signature component)
The works-grid `.feature` card is the site's most distinctive pattern: a two-column split (dark "visual" panel with a small CSS-built motif representing the case + light "body" panel with role, tags, and a "Read case study →" link), alternating sides down the page (`.feature` / `.feature.alt`), collapsing to a single column under 820px. The dark panel always carries a soft radial accent-color glow bottom-right — the one place gradients are allowed, since it's a glow effect, not gradient text.

## 6. Do's and Don'ts

### Do:
- **Do** keep ink/cream/line/card neutrals identical across every page; only the accent token changes per case study (The Borrowed Palette Rule).
- **Do** use full-pill radius (999px) for every button and tag, and the 26/18/12px descending scale for content containers — never square corners on a card.
- **Do** keep shadows exclusive to hover states on clickable elements (The Flat-By-Default Rule); everything else is border + fill.
- **Do** state real numbers, roles, and timeframes in case-study copy instead of adjectives — the honesty distinction between 実務経験 and 学習・実践中 is a credibility feature, not a hedge.
- **Do** keep the radial accent-color glow confined to dark full-bleed panels (`.fullbleed`, `.contact-panel`, feature-card `.vis`) as the one allowed gradient-adjacent effect.

### Don't:
- **Don't** use `border-left`/`border-right` as a colored accent stripe on any card, callout, or list item.
- **Don't** apply `background-clip: text` gradient text for emphasis — emphasis is a solid accent color via `<em>` or font-weight only.
- **Don't** use glassmorphism decoratively; the topbar's backdrop-blur is the one sanctioned, functional use (legibility while scrolling), not a visual motif to repeat elsewhere.
- **Don't** stack a tiny tracked all-caps eyebrow above every section — the `.idx`/`.mono` labels sit beside a heading as metadata, never centered above it as a kicker (The No-Eyebrow Rule).
- **Don't** build identical icon+heading+text card grids; the "Other Works" grid varies thumbnail treatment per project instead of repeating one template.
- **Don't** mix two accent colors on one page, and never reuse another case study's accent instead of the current page's own.
