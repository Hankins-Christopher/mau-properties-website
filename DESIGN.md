---
name: MAU Properties LLC
description: A restrained editorial identity for real estate and independent digital ventures.
colors:
  green: "#18382b"
  paper: "#f7f8f4"
  ink: "#23382c"
  muted: "#5c6b5f"
  line: "#ccd4c9"
  lime: "#dae6b1"
  light: "#edf2e3"
  ventures-surface: "#e7ecdf"
  focus: "#779438"
  button-hover: "#f0f5d8"
typography:
  display:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "clamp(57px, 6.2vw, 88px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "clamp(38px, 4vw, 56px)"
    fontWeight: 400
    lineHeight: 1.12
    letterSpacing: "-0.025em"
  title:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "clamp(32px, 3.5vw, 47px)"
    fontWeight: 400
    lineHeight: 1.2
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.75
  label:
    fontFamily: "Manrope, Arial, sans-serif"
    fontSize: "12px"
rounded:
  button: "3px"
spacing:
  desktop-column: "110px"
  tablet-column: "65px"
  mobile-column: "28px"
components:
  button-primary:
    backgroundColor: "{colors.lime}"
    textColor: "{colors.green}"
    rounded: "{rounded.button}"
    padding: "15px 21px"
  button-primary-hover:
    backgroundColor: "{colors.button-hover}"
---

# Design System: MAU Properties LLC

## Overview

The implemented identity is editorial and grounded: large serif statements, compact sans-serif details, generous space, and ruled rows. Deep green establishes the company presence; pale surfaces organize the supporting content. This document records the code-led implementation rather than a separate visual comp.

**Key Characteristics:**

- Typographic hierarchy carries the design without photography.
- Wide paired columns become a clear single-column reading order.
- Restrained lime emphasis and small directional arrows identify actions.

## Colors

### Primary

Deep green anchors the header and hero. Lime highlights the hero's second phrase and the primary action; light supplies text on the green surface.

### Neutral

Paper is the page background. Ink and muted distinguish headings and supporting prose. Line divides light surfaces; the ventures section uses a pale green surface. Additional local green tints in the stylesheet support rules, captions, and small marks; they are contextual values rather than a separate accent system.

**The Surface Rule.** Keep contrast appropriate to each surface: lime focus outlines on green, the dedicated focus color on light backgrounds.

## Typography

Newsreader and Manrope are self-hosted variable TrueType fonts, with Georgia and Arial fallbacks. Both files declare weights 200–800 and use `font-display: swap`. Newsreader carries headings and the MAU wordmark; Manrope carries prose, navigation, and actions.

The frontmatter defines the desktop hierarchy. Section prose is generally (14px, line-height 1.9), with lead paragraphs (20px, line-height 1.65) and reading widths up to (65ch). Hero supporting copy uses (16px, line-height 1.8). Action labels use weight (750). Heading tracking is tight; headings use balanced wrapping.

## Layout

The centered container is capped at (1264px), with total horizontal inset (112px). The hero uses columns (1.65fr / 1fr) with a (90px) gap. Real estate, venture rows, and company content use (1.2fr / 1fr) columns with the desktop column gap. Section spacing is generous, generally around (88–110px) vertically.

At widths up to (1100px), the container inset becomes (72px), hero gap becomes (45px), its columns become (1.7fr / 1fr), and the display heading becomes (66px). Paired content uses the tablet column gap; the footer may wrap.

At widths up to (760px), the container inset becomes (40px). Hero and content grids stack. Hero typography becomes `clamp(46px, 9.6vw, 68px)` with line-height (1.05); venture titles become (38px). Most content sections use (62px) vertical spacing. The header retains only the Digital ventures navigation link. The footer's legal group occupies a full row. Keep the narrow-screen reading order identical to the source order.

## Elevation & Depth

There are no box shadows. Broad background changes, spacing, and one-pixel rules establish separation. The header and hero baseline use subdued green rules; venture rows use stronger pale-green dividers.

## Shapes

Surfaces and content rows are square. The primary action has a subtle button radius; property principles use tiny square markers (5px). Arrows are unfilled SVG strokes with rounded caps and joins (1.5px stroke), sized by their context.

## Components

**Primary action.** A lime inline link with a trailing arrow, compact bold label, and (42px) internal gap. Hover lightens the background over (0.2s).

**Branch navigation.** Two full-width ruled links pair a serif title with a short caption and diagonal arrow. Hover changes the title to lime and moves the arrow (4px, -4px).

**Venture rows.** Open ruled rows pair the venture name and category with prose, availability context, and an underlined outbound link. The link arrow moves (3px, -3px) on hover. Preserve status text beside the project description.

**Navigation and focus.** Header links are compact and unadorned, with lime hover text. Links receive a visible (3px) outline offset by (6px). A keyboard skip link appears on focus. Reduced-motion preference disables transitions and animations and restores automatic scrolling.

## Do's and Don'ts

- **Do** use typography, spacing, and rules as the primary visual structure.
- **Do** preserve visible focus and reduced-motion behavior when extending components.
- **Do** keep company and project identity distinct through the existing title/category/description hierarchy.
- **Don't** introduce elevated dashboard cards into the current flat editorial system.
- **Don't** add fabricated property photography, listing badges, availability claims, or contact forms to this informational portfolio.
