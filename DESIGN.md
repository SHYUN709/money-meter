---
name: 알바 머니 미터
description: A calm everyday-money app where the live amount and what's next are the only loud things.
colors:
  warm-ground: "#F5F1EC"
  card-white: "#FFFFFF"
  sunk-oat: "#EFEAE3"
  warm-ink: "#222019"
  warm-muted: "#625B53"
  hairline: "#E3DCD2"
  action-green: "#1F7A5A"
  action-ink: "#FFFFFF"
  action-soft: "#E3F1EA"
  danger-red: "#B42318"
  danger-soft: "#FBE9E7"
  warm-ground-dark: "#191714"
  card-dark: "#24211D"
  sunk-dark: "#2E2A25"
  warm-ink-dark: "#F2EEE8"
  warm-muted-dark: "#B4ACA2"
  hairline-dark: "#3A352F"
  action-green-dark: "#5CC79A"
  action-ink-dark: "#0E1F17"
  action-soft-dark: "#1F3229"
  danger-red-dark: "#F08A7E"
  danger-soft-dark: "#3A2420"
typography:
  display:
    fontFamily: "Gothic A1, system-ui, -apple-system, Apple SD Gothic Neo, Malgun Gothic, sans-serif"
    fontSize: "clamp(2.75rem, 10vw, 4.25rem)"
    fontWeight: 800
    lineHeight: 1.08
    letterSpacing: "-0.035em"
    fontFeature: "\"tnum\""
  display-rest:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "clamp(2.25rem, 8vw, 3.25rem)"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.03em"
    fontFeature: "\"tnum\""
  headline:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "2.25rem"
    fontWeight: 800
    lineHeight: 1.1
    letterSpacing: "-0.03em"
    fontFeature: "\"tnum\""
  headline-setup:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 800
    lineHeight: 1.3
    letterSpacing: "-0.02em"
  title-figure:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "1.375rem"
    fontWeight: 700
    fontFeature: "\"tnum\""
  title:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 700
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "1rem"
    fontWeight: 500
    lineHeight: 1.55
  body-secondary:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 500
    lineHeight: 1.55
  label:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 600
  tag:
    fontFamily: "Gothic A1, system-ui, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 500
rounded:
  pill: "99px"
  tabbar: "22px"
  card: "20px"
  float: "18px"
  inner: "16px"
  control-lg: "14px"
  control: "12px"
  segment: "10px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "12px"
  lg: "16px"
  card: "22px"
components:
  button-primary:
    backgroundColor: "{colors.action-green}"
    textColor: "{colors.action-ink}"
    rounded: "{rounded.control-lg}"
    padding: "0 20px"
    height: "48px"
  button-ghost:
    backgroundColor: "{colors.sunk-oat}"
    textColor: "{colors.warm-ink}"
    rounded: "{rounded.control-lg}"
    padding: "0 20px"
    height: "48px"
  button-danger:
    backgroundColor: "{colors.danger-soft}"
    textColor: "{colors.danger-red}"
    rounded: "{rounded.control-lg}"
    padding: "0 20px"
    height: "48px"
  button-mini:
    backgroundColor: "{colors.sunk-oat}"
    textColor: "{colors.warm-ink}"
    rounded: "{rounded.control}"
    padding: "0 14px"
    height: "44px"
  input:
    backgroundColor: "{colors.card-white}"
    textColor: "{colors.warm-ink}"
    rounded: "{rounded.control}"
    padding: "0 14px"
    height: "48px"
  card:
    backgroundColor: "{colors.card-white}"
    rounded: "{rounded.card}"
    padding: "22px"
  segmented:
    backgroundColor: "{colors.sunk-oat}"
    rounded: "{rounded.control-lg}"
    padding: "4px"
  segmented-selected:
    backgroundColor: "{colors.card-white}"
    textColor: "{colors.warm-ink}"
    rounded: "{rounded.segment}"
    height: "40px"
  chip:
    backgroundColor: "{colors.card-white}"
    textColor: "{colors.warm-ink}"
    rounded: "{rounded.control}"
    padding: "0 12px"
    height: "44px"
  chip-selected:
    backgroundColor: "{colors.action-soft}"
    textColor: "{colors.action-green}"
  tabbar:
    backgroundColor: "{colors.card-white}"
    rounded: "{rounded.tabbar}"
    padding: "6px"
  tab-active:
    backgroundColor: "{colors.action-soft}"
    textColor: "{colors.action-green}"
    rounded: "{rounded.inner}"
    height: "56px"
  status-pill:
    backgroundColor: "{colors.card-white}"
    textColor: "{colors.warm-muted}"
    rounded: "{rounded.pill}"
    padding: "0 14px"
    height: "36px"
---

# Design System: 알바 머니 미터

## Overview

**Creative North Star: "The Quiet Pay Slip"**

A warm, paper-tinted everyday-money app. One column of soft white cards sits on an oat-coloured ground; the only loud thing on any screen is the money figure in heavy Gothic A1, and the only colour is a deep green that marks what you can press and what is live or filling up. Everything else is warm ink and warm grey.

Density is relaxed but not sparse: 16px gaps between cards, 22px inside them, hairline dividers instead of boxes within a card. Depth is a soft ambient lift, never an outline or an offset block. Motion is short and soft: a slight press-in on buttons, eased fills on bars and the goal ring, no entrance bounce.

The system ships in light and dark from the same token names; dark keeps the warmth (brown-black ground, not neutral grey) and lifts the green to a mint that keeps AA on dark cards.

**Key Characteristics:**
- Warm tinted ground, borderless white cards at 20px radius with ambient shadow.
- One action colour (green) reserved for pressables, live status, and progress/selected marks.
- One typeface, Gothic A1, carried from 0.75rem tags to a 4.25rem live amount; tabular figures on every money value.
- Line icons drawn as inline SVG symbols, 1.8 stroke, round caps.
- Floating bottom tab bar on every breakpoint.

## Colors

A warm neutral palette with a single deep green accent; red appears only for destructive actions and errors.

### Primary
- **Ledger Green** (action-green; dark: action-green-dark): primary buttons, links, focus rings, the active tab text, the live dot in the status pill, the shift bar, the XP meter, the goal ring arc, checked chips and choice cards, the earned-badge tile, the "근무 중" friend marker.
- **Green Wash** (action-soft; dark: action-soft-dark): the tinted ground behind selected tabs, selected chips/choices, earned tiles, the "나" tag and text selection.
- **Ledger Ink-on-Green** (action-ink): text on filled green buttons only.

### Neutral
- **Oat Ground** (warm-ground): page background; also the toast's text colour.
- **Card White** (card-white): every card, the tab bar, the status pill, icon buttons, inputs, unselected chips, the selected segment.
- **Sunk Oat** (sunk-oat): recessed surfaces inside cards: segmented-control track, bar and ring tracks, ghost and mini buttons, icon tiles, conversion tiles, bulk-edit panel, "진행 중" tag.
- **Warm Ink** (warm-ink): primary text and money figures; the toast background; the first-place rank disc.
- **Warm Muted** (warm-muted): labels, secondary lines, decimals of the live amount, inactive tabs and segments (5.6:1 or better on every light surface).
- **Hairline** (hairline): in-card dividers, input and chip strokes (1.5px), resting status dot, unfilled setup steps.

### Danger
- **Receipt Red** (danger-red) on **Red Wash** (danger-soft): the reset button, delete mini-buttons on hover, field errors and invalid input borders, the danger-zone card outline.

### Named Rules
**The Green Means Go Rule.** Green appears only on something you can press, something live, or something filling/selected (bars, ring, checked state). It is never used to decorate a heading, a number or an icon at rest.

**The Same Names, Two Lights Rule.** Every colour exists as one token name with a light and a dark value (`:root`, `prefers-color-scheme: dark`, and `[data-theme]` override). New surfaces use the variables, never literal hex.

## Typography

**Display Font:** Gothic A1 (with system-ui, Apple SD Gothic Neo, Malgun Gothic)
**Body Font:** Gothic A1, same stack
**Label/Mono Font:** none distinct; figures use Gothic A1 with tabular numerals

**Character:** A single humanist Korean sans doing all the work through weight (500 body, 600 labels, 700 titles, 800 figures) and tight negative tracking on large numbers. `word-break: keep-all` keeps Korean words intact.

### Hierarchy
- **Display** (800, clamp(2.75rem, 10vw, 4.25rem), 1.08, -0.035em): the live amount only. Its decimals drop to 0.42em/700/muted and the 원 unit to 0.45em/700.
- **Display Rest** (800, clamp(2.25rem, 8vw, 3.25rem), 1.1): the off-shift "다음 출근" time that replaces the amount.
- **Headline** (800, 2.25rem, 1.1): payday D-day. Setup headings use 1.5rem/800/1.3.
- **Title Figure** (700, 1.375rem): secondary money values (payday amount); conversion counts use the same size at 800. Goal ring percentage 1.5rem/800.
- **Title** (700, 1.0625rem, -0.01em): card headings; app name 1.125rem/800.
- **Body** (500, 1rem, 1.55): default text and list titles (700).
- **Body Secondary** (0.9375rem): leads, rate line, buttons in segments, links. Sub-lines 0.875rem.
- **Label** (600, 0.8125rem): tab labels, tally captions, help text. Tags 0.75rem.

### Named Rules
**The Tabular Money Rule.** Every money or count figure carries tabular numerals (`.num`), so ticking values never jitter.

**The One Loud Number Rule.** Only one Display-size figure per screen: the live amount, or the next-shift time when resting. Other figures step down to Headline or below.

## Layout

A single centred column, max 1040px, 16px side padding, with 112px bottom padding (plus safe area) clearing the floating tab bar. Cards stack with a 16px gap. At 900px and up the home view becomes two columns (1.35fr hero / 1fr side cards, stretched to equal height) with the growth card spanning full width; settings become two columns. Between 560px and 899px the payday and goal cards sit side by side; below 560px everything stacks. The conversion grid is 2 columns, 4 at 640px+. Spacing steps are 4, 8, 12, 16 and 22px; inside cards, sections are separated by 22px plus a hairline top border with 18px padding.

## Elevation & Depth

Soft ambient layering in warm-brown shadow (pure black in dark mode, stronger opacity). Three tokens only.

### Shadow Vocabulary
- **Resting** (`--shadow`: `0 1px 2px rgba(60,45,30,.06), 0 6px 20px rgba(60,45,30,.06)`): cards, status pill, icon buttons.
- **Floating** (`--shadow-float`: `0 2px 6px rgba(60,45,30,.08), 0 12px 32px rgba(60,45,30,.12)`): fixed and sticky layers: tab bar, settings save bar.
- **Segment** (`--shadow-seg`: `0 1px 3px rgba(60,45,30,.12)`): the selected segment lifting off its sunk track.

### Named Rules
**The Lift, Not Line Rule.** Cards have no border; separation comes from the tinted ground and the resting shadow. Inside a card, depth goes down (sunk-oat recesses), never up.

## Shapes

Generously soft corners that tighten as elements get smaller: card 20px, tab bar 22px, save bar 18px, tiles/tabs/toast 16px, buttons/segment track/choice cards 14px, inputs/chips/mini/icon buttons 12px, segments 10px. Bars, dots, tags and the status pill are full pills (99px). Icon tiles are 44px rounded squares; rank markers are 36px circles. Strokes, where used, are 1.5px hairline.

## Components

### Buttons
- **Shape:** soft rounded rectangle (14px), 48px tall.
- **Primary:** green fill, white text (dark: mint fill, near-black text), 700, 0 20px.
- **Hover / Focus / Active:** hover brightens 6%; active scales to 0.97 over 150ms (cubic-bezier(.16,1,.3,1)); focus is a 2px green outline at 3px offset; disabled 45% opacity.
- **Ghost:** sunk-oat fill, ink text. **Danger:** red wash fill, red text.
- **Mini:** 44px square-minimum, 12px radius, sunk fill, 0.875rem/600, optional 18px icon. Delete mini is transparent red text, red wash on hover.
- **Link:** green 700 text with a chevron, padded to a 44px hit area.

### Chips
- **Style:** 44px, 12px radius, card fill, 1.5px hairline stroke, 700.
- **State:** selected turns the stroke green on green wash with green text. Radio choice cards follow the same pattern at 14px radius.

### Cards / Containers
- **Corner Style:** 20px.
- **Background:** card-white.
- **Shadow Strategy:** Resting shadow.
- **Border:** none (the danger-zone card is the single exception: 1.5px red-wash outline).
- **Internal Padding:** 22px; card title, then content at 14px (row-head) spacing.

### Inputs / Fields
- **Style:** 48px, card fill, 1.5px hairline stroke, 12px radius; label 0.9375rem/700 above, help 0.8125rem muted below, 6px gaps.
- **Focus:** stroke turns green plus a 2px green outline at 1px offset.
- **Error:** red stroke with a 0.8125rem/600 red message.

### Navigation
- **Tab bar:** fixed, bottom-centred, min(560px, 100% - 24px), card fill, 22px radius, floating shadow, 6px inset. Four 56px tabs, each a 22px line icon over a 0.8125rem/600 label; inactive muted, active green text on green wash at 16px radius. Same on phone and desktop.
- **Top bar:** app name left (1.125rem/800), status pill (resting grey dot / green live dot) and 44px icon button right.

### Segmented Control
Sunk-oat track (14px radius, 4px padding) with four equal 40px segments; the selected one becomes a white card with the segment shadow and ink text.

### Lists
Rows separated by hairlines, 14px vertical padding, optional 44px sunk icon tile left, bold value right-aligned. Inline status tags are 0.75rem pills on sunk (neutral) or green wash (self).

### Goal Ring (signature)
A 124px ring (96px under 440px): 10px sunk track and one round-capped green arc that fills via stroke-dashoffset over 1s; percentage centred at 1.5rem/800 with a muted 0.75rem caption, the goal figures beside it.

### Progress Bars
8px pill tracks in sunk-oat with a green fill that eases its width over 0.8s (cubic-bezier(.16,1,.3,1)); used for the shift bar and XP meter. Setup steps are 6px pills, hairline until reached, then green.

### Toast
Inverted: ink background, ground-coloured text, 16px radius, slides up 16px and fades in over 300ms above the tab bar; optional action button on a 14% white wash.

## Do's and Don'ts

### Do:
- **Do** put every new surface in a white 20px card on the oat ground with the Resting shadow.
- **Do** keep green for pressables, live status, and progress/selected state only.
- **Do** mark every money value with tabular numerals and keep a single Display-size figure per screen.
- **Do** draw icons as inline SVG line symbols (24 viewBox, 1.8 stroke, round caps, currentColor).
- **Do** keep controls at 44px minimum (48px for primary buttons and inputs) and respect `prefers-reduced-motion`, which disables all transitions.
- **Do** define any new colour in both light and dark token sets.

### Don't:
- **Don't** add borders or hard offset shadows to cards; use the three shadow tokens.
- **Don't** use gradients, emoji icons, or green on decorative text and numbers at rest.
- **Don't** introduce a second typeface or a display face for numbers; hierarchy comes from Gothic A1 weight and size.
- **Don't** add entrance bounces; motion is press feedback and eased fills only.
