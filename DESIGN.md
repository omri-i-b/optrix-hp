---
version: alpha
name: Optrix
description: >
  Design system for Optrix, an AI command center for industrial operations.
  Modern-minimal SaaS aesthetic — white canvas, warm stone ink, single orange
  accent. Geist sans for everything, Geist Mono for data.
colors:
  primary: "#1c1917"
  secondary: "#57534d"
  tertiary: "#fe551b"
  neutral: "#ffffff"
  neutral-subtle: "#fafaf9"
  muted: "#79716b"
  ghost: "#a8a29e"
  border: "#efeeed"
  tertiary-hover: "#e54a15"
  tertiary-soft: "#c2410c"
  on-primary: "#ffffff"
  on-tertiary: "#ffffff"
  success: "#16a34a"
  warning: "#ca8a04"
  error: "#dc2626"
typography:
  display:
    fontFamily: Geist
    fontSize: clamp(36px, 4.5vw + 8px, 56px)
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: -0.03em
  headline-lg:
    fontFamily: Geist
    fontSize: clamp(28px, 3vw + 8px, 36px)
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: -0.025em
  headline-md:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: -0.02em
  body-lg:
    fontFamily: Geist
    fontSize: 18px
    fontWeight: 400
    lineHeight: 1.55
  body-md:
    fontFamily: Geist
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.6
  body-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: 500
    letterSpacing: 0.14px
  caption:
    fontFamily: Geist
    fontSize: 12px
    fontWeight: 400
    lineHeight: 1.4
  mono:
    fontFamily: Geist Mono
    fontSize: 14px
    fontWeight: 500
    lineHeight: 1.55
rounded:
  none: 0px
  sm: 4px
  md: 6px
  lg: 8px
  card: 12px
  xl: 24px
  full: 999px
spacing:
  3xs: 4px
  2xs: 8px
  xs: 12px
  sm: 16px
  md: 24px
  lg: 32px
  xl: 48px
  2xl: 72px
  3xl: 112px
  gutter: clamp(20px, 4vw, 32px)
  page-max: 1152px
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    height: 38px
    padding: 14px
  button-primary-hover:
    backgroundColor: "#292524"
  button-secondary:
    backgroundColor: "rgba(0, 0, 0, 0.04)"
    textColor: "{colors.primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    height: 38px
    padding: 14px
  button-secondary-hover:
    backgroundColor: "rgba(0, 0, 0, 0.08)"
  button-accent:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    height: 38px
    padding: 14px
  button-accent-hover:
    backgroundColor: "{colors.tertiary-hover}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.muted}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    height: 32px
    padding: 15px
  button-ghost-hover:
    backgroundColor: "rgba(239, 238, 237, 0.4)"
  nav-button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    height: 32px
    padding: 20px
  nav-button-secondary:
    backgroundColor: "rgba(239, 238, 237, 0.7)"
    textColor: "{colors.muted}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.full}"
    height: 32px
    padding: 15px
  card:
    backgroundColor: "{colors.neutral-subtle}"
    textColor: "{colors.primary}"
    rounded: "{rounded.card}"
    padding: 32px
  badge:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    rounded: "{rounded.full}"
    height: 22px
    padding: 7px
  chip:
    backgroundColor: "{colors.neutral-subtle}"
    textColor: "{colors.secondary}"
    rounded: "{rounded.xl}"
    padding: 16px
---

# Optrix Design System

The design system for Optrix — an AI command center for industrial operations.
Modern-minimal SaaS aesthetic in the tradition of Linear, Vercel, and Stripe.
White canvas, warm stone ink scale, single orange accent used sparingly.

## Overview

Optrix targets manufacturing leaders — QA managers, plant operators, purchasing
teams. The design must feel **precise and trustworthy**, never playful or
experimental. Every element earns its place through function.

The visual language is **confident restraint**: large sans-serif headings with
tight tracking, generous whitespace, monochrome surfaces punctuated by a single
orange accent. The accent appears only on primary CTAs, status badges, and the
brand mark — never as decoration.

## Colors

The palette uses a warm stone scale from the Tailwind Stone family, anchored by
a single high-chroma accent orange.

- **Primary (#1c1917):** Near-black warm stone. Used for headings, primary text,
  and filled buttons. Never use pure #000000.
- **Secondary (#57534d):** Medium stone for body text and nav links. The default
  reading color.
- **Tertiary (#fe551b):** Brand orange. Reserved exclusively for: primary CTA
  fills, the brand mark, status badges, and section labels. Maximum 5% of any
  viewport.
- **Neutral (#ffffff):** Pure white page background. No off-white tinting.
- **Neutral Subtle (#fafaf9):** Warm hint surface for banners, card backgrounds,
  chips. One step off white.
- **Muted (#79716b):** Captions, placeholder text, secondary nav buttons.
- **Border (#efeeed):** All hairline rules, card borders, dividers. One value,
  used everywhere — no border color variation.

### Contrast Ratios

| Pair | Ratio | WCAG |
|:-----|:------|:-----|
| Primary on Neutral | 16.75:1 | AAA |
| Secondary on Neutral | 7.14:1 | AAA |
| Tertiary on Neutral | 3.96:1 | AA Large |
| Muted on Neutral | 4.64:1 | AA |
| Primary on Neutral Subtle | 16.42:1 | AAA |

## Typography

Two typefaces only. Geist Sans for all reading and display text. Geist Mono for
code snippets, data values, and terminal-style UI mocks.

- **Display:** Geist 600, 36–56px fluid, tracking -0.03em, line-height 1.08.
  Used once per page for the hero heading.
- **Headline LG:** Geist 600, 28–36px fluid, tracking -0.025em. Section
  headings and card titles.
- **Headline MD:** Geist 600, 24px, tracking -0.02em. Sub-section headings and
  feature card titles.
- **Body LG:** Geist 400, 18px, line-height 1.55. Hero subtitle and pull
  quotes.
- **Body MD:** Geist 400, 16px, line-height 1.6. Default paragraph text.
- **Body SM / Label:** Geist 400–500, 14px, tracking 0.14px. Nav links, button
  labels, badges, captions.
- **Caption:** Geist 400, 12px. Figcaptions, chip badges, small metadata.
- **Mono:** Geist Mono 500, 14px. Code blocks, terminal mocks, data values in
  stat strips.

### Weight Rules

- **600 (SemiBold):** Display and headline levels only. Never on body text.
- **500 (Medium):** Labels, section labels, nav active state, badge text.
- **400 (Regular):** Everything else — body, buttons, captions, nav links.
- **700 (Bold):** Never used. The heaviest weight in the system is 600.

## Layout

The layout follows a single-column centered model with a 1152px max-width
container.

- **Page max-width:** 1152px (72rem), centered with auto margins.
- **Page gutter:** Fluid — `clamp(20px, 4vw, 32px)`.
- **Section spacing:** 112px between major sections (3xl). 72px for tight
  sections (2xl).
- **Section dividers:** 1px solid #efeeed between adjacent sections.
- **Content max-width:** Headings and body text cap at 56ch–60ch to maintain
  readable line lengths.
- **Grid:** 2-column for feature cards and tour rows on desktop, 1-column
  below 768px.

### Spacing Scale

All spacing uses named tokens from a 4px base scale. Raw pixel values are
never used in component CSS — always reference the token.

| Token | Value | Usage |
|:------|:------|:------|
| 3xs | 4px | Micro gaps, badge padding |
| 2xs | 8px | Button gaps, inline spacing |
| xs | 12px | Card internal gaps, nav link padding |
| sm | 16px | Default component padding, nav height offset |
| md | 24px | Card body padding, section sub-gaps |
| lg | 32px | Card padding, section heading gap |
| xl | 48px | Hero vertical padding, major section gaps |
| 2xl | 72px | Tight section padding |
| 3xl | 112px | Major section padding |

## Elevation & Depth

Depth is achieved through **subtle border + shadow layering**, not dramatic
drop shadows.

- **Cards:** 1px solid #efeeed border + `0 1px 3px rgba(0,0,0,0.04)` resting
  shadow. On hover: `0 2px 8px rgba(0,0,0,0.08)` + 2px translateY lift.
- **Screenshot frame:** 1px border + `0 16px 48px -16px rgba(0,0,0,0.12)` for
  a grounded float effect.
- **Nav bar:** No shadow. Uses `backdrop-filter: blur(12px)` and semi-transparent
  white background for glass effect.
- **Flat surfaces (banners, chips):** 1px solid #efeeed border only. No shadow.

## Shapes

The shape language uses three tiers of rounding:

- **Pill (999px):** All buttons, nav bar, badge chips. The primary interactive
  shape.
- **Card (12px):** Content containers — feature cards, screenshot frames, role
  cards, stat blocks.
- **Subtle (6px):** Brand mark, nav link hover backgrounds, small badges.
- **Input (8px):** Form inputs (not currently used but reserved).

### Rules

- Buttons are always pill-shaped. No square or rounded-rectangle buttons.
- Cards are always 12px radius. No variation per card type.
- Never mix pill and card radii on the same element.

## Components

### Buttons

All buttons are pill-shaped (border-radius: 999px) with no visible border.
Three semantic variants exist:

**Primary** — Dark fill for the main page action.
- Background: #1c1917 → hover #292524
- Text: #ffffff, 14px, 400 weight, -0.48px tracking
- Height: 38px, padding: 0 14px
- Used for: Hero CTA ("Start for free"), nav CTA ("Start for free")

**Secondary** — Subtle gray for companion actions.
- Background: rgba(0,0,0,0.04) → hover rgba(0,0,0,0.08)
- Text: #1c1917, 14px, 400 weight, -0.48px tracking
- Height: 38px, padding: 0 14px
- Used for: Hero secondary ("Talk to us"), quote section CTAs

**Accent** — Orange fill for closing CTAs and high-priority actions.
- Background: #fe551b → hover #e54a15
- Text: #ffffff, 14px, 400 weight
- Height: 38px, padding: 0 14px
- Used for: Final CTA section ("Request a pilot")

**Ghost** — Transparent for tertiary nav actions.
- Background: transparent → hover rgba(239,238,237,0.4)
- Text: #79716b, 14px, 400 weight
- Height: 32px, padding: 0 15px
- Used for: Nav "Login" button

**Nav variants** use 32px height and 14px font. Page-body variants use 38px
height. This is the only height variation — there is no "large" button.

### Cards

Feature cards, role cards, and stat blocks share one card archetype:

- Background: #fafaf9 (subtle) or #ffffff (white)
- Border: 1px solid #efeeed
- Border-radius: 12px
- Padding: 32px (body area)
- Hover: translateY(-2px) + shadow lift
- Title: headline-md (24px/600)
- Body: body-md (16px/400) in #57534d

### Badge Chip

The inline hero chip and card badges use:

- Background: #fafaf9
- Border: 1px solid #efeeed
- Border-radius: 24px
- Inner badge: #fe551b fill, white text, 12px, 30px radius
- Text: 14px, #57534d

### Section Labels

Orange accent labels that introduce sections ("The platform", "How it works"):

- Font: 14px, weight 500
- Color: #fe551b (accent)
- No background, no border — text only

### Quote Block

Centered large italic-free quote with attribution:

- Quote text: display size (fluid 36–56px), 600 weight, #1c1917
- Attribution: 14px, #57534d, format "Name · Title, Company"
- CTAs below: secondary button style

### Stat Strip

Four-column grid of key metrics:

- Stat value: headline-lg size (28–36px), 600 weight, #1c1917, Geist Sans
- Stat label: 14px, 500 weight, #1c1917
- Stat description: 14px, 400 weight, #57534d

### Navigation

Full-width sticky bar, 48px height:

- Background: rgba(255,255,255,0.9) + backdrop-filter blur(12px)
- Logo: 22px orange mark + "Optrix" 14px/600 + "Beta" 12px muted
- Links: 14px/400, #57534d, 0.14px tracking, 4px radius hover
- Right: Login (ghost) + Talk to sales (secondary pill) + Start for free
  (primary pill, 32px height)

### Footer

Statement footer — tagline + wordmark + inline links:

- Background: #ffffff
- Tagline: headline-lg, #1c1917
- Wordmark: 14px + orange mark
- Links: 14px, #57534d
- Copyright: 14px, #79716b
- Top border: 1px solid #efeeed

## Do's and Don'ts

- **Do** use the accent orange only for: primary CTAs, section labels, the brand
  mark, and status badges. Nothing else.
- **Do** maintain pill shape on every button. No exceptions.
- **Do** use 1px #efeeed for all borders and dividers. One border color system-wide.
- **Do** keep heading weight at 600 and body weight at 400. No other weights on
  visible text.
- **Don't** use pure black (#000000). The darkest value is #1c1917.
- **Don't** add shadows to flat surfaces (banners, chips, badges). Only cards and
  the screenshot frame get shadows.
- **Don't** use more than one accent color. Orange is the only chromatic hue.
- **Don't** use italic text anywhere. The system is upright-only.
- **Don't** use Geist Mono for anything except code blocks, terminal mocks, and
  stat values.
- **Don't** set border-radius on buttons to anything other than 999px (pill).
- **Don't** use raw pixel values for spacing — always use named tokens.
