---
version: alpha
name: NewForm
description: A stark editorial system with oversized typography, bright green accents, and minimal chrome.
colors:
  primary: "#2BEE4B"
  secondary: "#121613"
  tertiary: "#E5E7EB"
  neutral: "#FFFFFF"
  surface: "#FFFFFF"
  on-surface: "#121613"
  accent: "#2BEE4B"
  border: "#E5E7EB"
  muted: "#F7F8F7"
  shadow: "#105E1D73"
typography:
  headline-display:
    fontFamily: "TWK Lausanne"
    fontSize: "120px"
    fontWeight: 550
    lineHeight: "120.015px"
    letterSpacing: "-4.8006px"
  headline-lg:
    fontFamily: "TWK Lausanne"
    fontSize: "99px"
    fontWeight: 550
    lineHeight: "119px"
    letterSpacing: "-0.55377px"
  headline-md:
    fontFamily: "Times New Roman"
    fontSize: "82px"
    fontWeight: 550
    lineHeight: "98px"
    letterSpacing: "0px"
  headline-sm:
    fontFamily: "Times New Roman"
    fontSize: "67px"
    fontWeight: 550
    lineHeight: "80px"
    letterSpacing: "0px"
  body-lg:
    fontFamily: "Editorial New"
    fontSize: "55.3675px"
    fontWeight: 300
    lineHeight: "83px"
    letterSpacing: "-1.10735px"
  body-md:
    fontFamily: "Editorial New"
    fontSize: "18px"
    fontWeight: 300
    lineHeight: "28px"
    letterSpacing: "-0.02em"
  body-sm:
    fontFamily: "Editorial New"
    fontSize: "14px"
    fontWeight: 300
    lineHeight: "22px"
    letterSpacing: "-0.01em"
  label-lg:
    fontFamily: "TWK Lausanne"
    fontSize: "12.0015px"
    fontWeight: 550
    lineHeight: "16px"
    letterSpacing: "0px"
  label-md:
    fontFamily: "TWK Lausanne"
    fontSize: "12px"
    fontWeight: 550
    lineHeight: "14px"
    letterSpacing: "0px"
  label-sm:
    fontFamily: "Times New Roman"
    fontSize: "12.0015px"
    fontWeight: 400
    lineHeight: "16px"
    letterSpacing: "0px"
  caption:
    fontFamily: "TWK Lausanne"
    fontSize: "10px"
    fontWeight: 550
    lineHeight: "12px"
    letterSpacing: "0.06em"
rounded:
  none: "0px"
  sm: "4px"
  md: "8px"
  lg: "12px"
  xl: "16px"
  full: "9999px"
spacing:
  xs: "10px"
  sm: "20px"
  md: "46px"
  lg: "74px"
  xl: "116px"
  base: "16px"
  gutter: "32px"
  margin: "40px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: "18.4559px 27.6885px"
    height: "50px"
  button-secondary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-lg}"
    rounded: "{rounded.sm}"
    padding: "18.4559px 27.6885px"
    height: "50px"
  button-link:
    backgroundColor: "transparent"
    textColor: "{colors.on-surface}"
    typography: "{typography.label-sm}"
    rounded: "{rounded.none}"
    padding: "0px"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "16px"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
    padding: "12px"
  chip:
    backgroundColor: "{colors.muted}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.full}"
    padding: "6px 10px"
---

# NewForm

## Overview
NewForm feels like a high-contrast editorial landing page for a finance, technology, or research audience. The tone is confident, modern, and slightly experimental, driven by oversized typography, monochrome imagery, and a sharp neon accent. The composition is spacious and cinematic rather than dense, with content floating in a quiet white field.

## Colors
- **Primary (#2BEE4B):** A vivid neon green used as the brand’s signal color for emphasis, links, underlines, and button fills. It adds optimism and technical energy without overwhelming the page.
- **Secondary (#121613):** A deep near-black used for the main text and interface chrome. It provides the strong editorial contrast that defines the system.
- **Tertiary (#E5E7EB):** A soft cool gray used for subtle borders and separation. It should stay understated so the layout keeps its light, airy feel.
- **Neutral (#FFFFFF):** The dominant background color. It keeps the experience minimal and allows text and imagery to carry most of the visual weight.
- **Surface (#FFFFFF):** Card and content surface color, matching the page background for a nearly flat presentation.
- **On-surface (#121613):** Default text and icon color on light surfaces.
- **Border (#E5E7EB):** Hairline divider color for cards, inputs, and low-contrast framing.
- **Muted (#F7F8F7):** A very light off-white for optional chips, tags, or secondary UI fills.
- **Shadow (#105E1D73):** A translucent green-shadow tone used only when a component needs a subtle glow; keep shadows minimal overall.

## Typography
The system uses three distinct typographic voices. TWK Lausanne is the primary sans-serif for navigation, labels, and large display headlines; it carries the brand’s modern, institutional tone. Editorial New provides the softer body voice and link text, while Times New Roman appears as a traditional serif counterpart for secondary and link-style treatments.

Headlines are extremely large and tightly tracked, with negative letter spacing on the biggest display sizes to create a compact, powerful block of text. Body copy is lighter and more open, with generous leading that supports the editorial feel. Labels and UI text are small, crisp, and mostly uppercase-adjacent in spirit through weight and spacing rather than explicit casing; the system does not rely on heavy letter-spacing except in the largest display setting.

## Layout
The layout is fluid and full-bleed, with a very wide hero composition that sits in generous whitespace. Spacing follows a loose cinematic rhythm: small offsets for chrome and nav, then large leaps for the hero content using the 46px, 74px, and 116px spacing tiers. Content should generally feel centered but slightly asymmetrical, with images interrupting the headline block as compositional accents.

Padding should remain minimal for the page shell and moderate for cards and interactive surfaces. Use wide margins and avoid tight multi-column packing unless the content is intentionally editorial or data-heavy. The system favors open breathing room over rigid grid density.

## Elevation & Depth
The visual language is intentionally flat. There are no meaningful shadows in the main interface, and hierarchy comes from scale, contrast, and placement instead of elevation. If depth is needed, prefer thin borders, tonal separation, or a subtle shadow using the green-tinted shadow token rather than strong blur-heavy effects.

Imagery and text create the primary layering by overlapping in a collage-like way. Cards should stay shallow and crisp, with border-based definition rather than pronounced elevation.

## Shapes
The shape language is restrained and mostly rectangular, with small rounded corners on interactive and media elements. Use 4px rounding for buttons and other controls, 8px for cards, and reserve fuller radii only for chips or pills. Overall, the system feels architectural and precise rather than soft or playful.

## Components
Buttons are compact, high-contrast, and label-driven. `button-primary` and `button-secondary` share the same bright green fill, black text, 4px radius, and a minimum height of 50px; they should feel assertive rather than decorative. Keep padding generous enough for a tactile feel, but avoid oversized pill shapes. `button-link` is bare and underlined, using Editorial New and no fill, border, or radius.

Cards use a white surface, 1px light-gray border, 8px radius, and no shadow. They should look like framed content containers, not floating panels. Inputs should follow the same calm treatment: white background, light border, compact radius, and clear text contrast.

Chips and tags, when needed, should be understated and compact, ideally using the muted surface with a full radius. Navigation items and utility labels should stay small and crisp, with the brand color reserved for underlines, markers, or micro-accents rather than large blocks of UI.

## Do's and Don'ts
- Do use the neon green sparingly to punctuate important actions and brand marks.
- Do keep typography large, confident, and tightly tracked in display contexts.
- Do preserve the open, airy composition with substantial whitespace around the hero.
- Do use flat surfaces and light borders instead of heavy shadows or layered panels.
- Don't introduce saturated secondary colors that compete with the primary green.
- Don't round components aggressively; avoid soft, pill-heavy UI except for chips.
- Don't crowd the layout with dense grids or small-text content blocks.
- Don't replace the editorial serif/sans contrast with a single generic UI font.