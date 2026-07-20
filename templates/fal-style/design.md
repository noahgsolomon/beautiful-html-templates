---
version: 1.0
name: fal Style
description: "A signal-dense presentation system derived from fal's own strategy decks. It combines oversized Focal grotesk headlines, Consolas technical labels, a near-white engineering grid, strict hairline frames, and four electric signal colors: fal purple, acid lime, hot pink, and cyan. Slides alternate between sparse thesis statements and dense analytical boards while preserving one shared grammar: tiny square marker + mono label, huge claim, bordered evidence."

colors:
  paper: "#FEFDFF"
  white: "#FFFFFF"
  ink: "#09090B"
  graphite: "#5F5B66"
  grid: "rgba(104, 29, 228, 0.055)"
  rule: "rgba(9, 9, 11, 0.72)"
  purple: "#681DE4"
  purple-light: "#AB77FF"
  lavender: "#F3ECFE"
  lime: "#ADFF00"
  lime-soft: "#E6FFB3"
  pink: "#EB064A"
  pink-soft: "#FDEEF4"
  cyan: "#99E5FF"
  green: "#145C36"

typography:
  display-hero:
    fontFamily: "'Focal', 'Arial Black', sans-serif"
    fontSize: "156px"
    fontWeight: 700
    lineHeight: 0.88
    letterSpacing: "-0.055em"
  display-statement:
    fontFamily: "'Focal', 'Arial Black', sans-serif"
    fontSize: "104px"
    fontWeight: 700
    lineHeight: 0.91
    letterSpacing: "-0.048em"
  display-section:
    fontFamily: "'Focal', sans-serif"
    fontSize: "68px"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.035em"
  title:
    fontFamily: "'Focal', sans-serif"
    fontSize: "42px"
    fontWeight: 700
    lineHeight: 1.02
    letterSpacing: "-0.025em"
  body:
    fontFamily: "'Focal', sans-serif"
    fontSize: "26px"
    fontWeight: 400
    lineHeight: 1.35
  body-large:
    fontFamily: "'Focal', sans-serif"
    fontSize: "34px"
    fontWeight: 400
    lineHeight: 1.28
  mono-label:
    fontFamily: "'Consolas', 'SFMono-Regular', monospace"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.25
    letterSpacing: "0.18em"
  mono-small:
    fontFamily: "'Consolas', 'SFMono-Regular', monospace"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.35
    letterSpacing: "0.12em"
  stat:
    fontFamily: "'Focal', sans-serif"
    fontSize: "96px"
    fontWeight: 700
    lineHeight: 0.9
    letterSpacing: "-0.05em"

canvas:
  width: 1920
  height: 1080
  outerPaddingX: 78
  outerPaddingTop: 50
  outerPaddingBottom: 46

components:
  engineering-grid:
    backgroundSize: "16px 16px"
    description: "A very faint purple graph-paper grid on near-white. It is always present on light slides and never competes with text."
  slide-kicker:
    description: "Top-left chrome: a 13px colored square followed by a lowercase, widely tracked Consolas label."
  page-count:
    description: "Top-right two-digit current/total counter in Consolas, separated by a centered dot."
  signal-period:
    description: "A colored square period attached to the final baseline of major display headlines. It is a square block, not a circular punctuation mark."
  hairline-frame:
    border: "1px solid rgba(9, 9, 11, 0.72)"
    description: "Strict rectangular frames and rules. No rounded corners, no shadows."
  band-header:
    description: "A shallow black or tinted strip spanning a panel, with a square marker and mono label."
  tag:
    description: "Small outlined mono token with 1px border and 8-14px horizontal padding. Used for categories, fields, companies, or data dimensions."
  quote-panel:
    description: "Large rectangular quote block led by an oversized pair of quote marks. May be black, lime, pink, or white with a colored left rule."
  signal-card:
    description: "A strict rectangle with a saturated header band and white/grid body. Used in two- and three-column comparisons."
  code-panel:
    description: "Near-white framed code area. Consolas body, violet function names, pink keys, green strings."
  data-bar:
    description: "Thin horizontal bar with pale track and a saturated fill in purple, lime, pink, cyan, or black."
---

# Overview

fal Style is an **electric product-systems presentation language**. It comes from the visual tension between two extremes: enormous, blunt Focal headlines that make one claim impossible to miss, and tiny Consolas labels that make the deck feel instrumented, technical, and exact. Between those extremes live rigid evidence boards: bordered panels, diagrams, code, tables, quotes, and charts.

The template is general-purpose because its identity does not depend on one fixed composition. The same square markers, grid paper, hairline frames, signal colors, typography, and punctuation treatment can carry a product definition, a technical architecture, a market comparison, customer evidence, a roadmap, or a closing slide.

Density alternates deliberately. A sparse slide may contain only one huge sentence and one chart. The next may contain ten boxes and three data views. This alternation is part of the voice: **claim, prove, claim, prove**.

# Source language

This system is based closely on the supplied fal Insights strategy deck:

- Near-white 16:9 canvas with a barely visible violet engineering grid.
- Focal Bold for display and Focal Regular/Medium for prose.
- Consolas for kickers, page numbers, tags, data labels, names, and code.
- Black structural rules at one pixel.
- Saturated fal purple (`#681DE4`), acid lime (`#ADFF00`), hot pink (`#EB064A`), and cyan (`#99E5FF`).
- Light lavender (`#F3ECFE`) as the only large soft fill.
- Square signal markers rather than circles, pills, gradients, or illustrations.
- Headline punctuation rendered as a small colored square.

# Colors

## Core surfaces

- **Paper** `#FEFDFF`: default slide surface.
- **White** `#FFFFFF`: framed cards that need to lift subtly from grid paper.
- **Ink** `#09090B`: display text, dark panels, charts, and borders.
- **Graphite** `#5F5B66`: body copy and secondary labels.
- **Lavender** `#F3ECFE`: soft product panels, secondary half-slides, and background contrast.

## Signal palette

- **Purple** `#681DE4`: fal's primary brand signal. Default accent for key words, active categories, and major fills.
- **Purple Light** `#AB77FF`: comparison bars and secondary violet data.
- **Lime** `#ADFF00`: live, shipped, active, positive, or structurally important information.
- **Pink** `#EB064A`: risk, model-provider side, friction, decisive emphasis, or a contrasting series.
- **Cyan** `#99E5FF`: technical support color, dark-slide subtitle, alternate comparison series.
- **Green** `#145C36`: restrained positive body emphasis on white.

Colors behave as **signals**, not decoration. A normal light slide should feature one dominant signal color and at most one supporting color. Multi-color slides are reserved for comparisons, segmentations, and diagrams where color distinguishes categories.

# Typography

## Focal

Focal is the identity. The template includes local WOFF2 files for Regular, Medium, Bold, and Italic. Do not substitute another grotesk when building from this template.

- Use **Focal Bold** for all major headlines, stats, and card titles.
- Use **Focal Regular** for most prose.
- Use **Focal Medium** for body emphasis and small section headers.
- Use **Focal Italic** only for quoted fragments or analytical annotations.

Display typography is unusually large, tightly tracked, and short-lined. The best fal headline is a complete spoken claim, not a noun phrase. Aim for 4-10 words on a sparse slide and no more than 18 words on a dense evidence slide.

## Consolas

Consolas is the instrumentation voice. Use it for:

- top-left kickers and top-right counters;
- tags, field names, code, and micro-labels;
- person names and titles under quotations;
- chart labels and axis captions;
- card eyebrows and step numbers.

Mono labels are generally lowercase, spaced out, and separated with centered dots. Do not set long paragraphs in Consolas.

# Layout grammar

The canvas is fixed at **1920x1080** and rendered through `deck-stage.js`. Light slides use an outer inset of 78px left/right, 50px top, and 46px bottom. The top chrome consumes roughly 30px; primary content begins between 110px and 145px from the top.

The grid is geometric but not a visible twelve-column bootstrap grid. Layouts are built from aligned halves, thirds, and horizontal bands:

- **Halves** for direct comparison, architecture + flywheel, or two deliverables.
- **Thirds** for product families, strategic pillars, or three data views.
- **Bands** for customer tiers, milestones, or summary arguments.
- **Asymmetry** for one large claim paired with a smaller table or chart.

No card is rounded. No card floats. Depth comes from adjacency, contrast, scale, and color—not shadows.

# Persistent chrome

Every slide carries:

1. A top-left `.kicker`: colored square + mono text.
2. A top-right `.page-count`: zero-padded current and total.

On closing or fully saturated slides, both may switch to white/cyan/lime. The chrome stays small enough to disappear when the speaker presents but precise enough to make screenshots feel authored.

# Component rules

## Square markers

Square markers are 12-15px. They precede kickers, band headers, and small subheads. They may appear as floating punctuation around large statistics, but use no more than three decorative markers on a slide.

## Signal periods

Major display headlines end with `<span class="period"></span>`. It appears as a 16-24px square aligned to the baseline. Default color follows the slide accent. Never replace it with a round dot.

## Frames and rules

Frames use one-pixel ink rules. Use two pixels only for a critical boundary on a diagram. Avoid gray card outlines. When a panel sits on a black background, use a gray or signal-color rule.

## Tags

Tags are strict rectangles, never pills. They use mono text at 14-16px with 1px borders. Default fill is transparent or white. One active tag may use lime.

## Quote panels

Quotes use Focal Medium or Bold at 26-38px. The opening quotation mark is a separate display element in a signal color. Highlight only the phrase that carries the evidence. Attribution is two mono lines: name first in a signal color, then role/company in graphite.

## Code

Code panels retain white space and thin borders. Syntax colors are limited to the template palette. Avoid dark IDE gradients, traffic-light window chrome, or rounded containers.

## Charts

Charts are flat and editorial. Preferred forms:

- horizontal comparison bars;
- simple vertical ratio bars;
- before/after blocks with a line overlay;
- sparse tables with three analytical rows;
- flow diagrams made from framed nodes and arrow lines.

Axes and labels use Consolas. Gridlines are hairlines. Avoid legends when direct labels fit.

# Slide composition patterns

## 1. Definition cover

Large branded title in the lower-left half. Small eyebrow above. One compact definition below. Preserve large negative space above and to the right.

## 2. Problem + answer board

Top framed thesis box with a colored left rule. Below, a bold answer headline and a dense evidence area combining code, process, or data views.

## 3. Three-step system

Three equal columns with giant step numbers. The middle step may use lime fill to show the system's unique center. Follow with three product cards or outcome cards.

## 4. Structural split

Two equal framed halves: one technical map and one flywheel or organizational mechanism. Use different soft backgrounds but shared rules.

## 5. Light/dark comparison

Split the canvas vertically. One competitor or alternative lives on grid paper; the other lives on ink black. Mirror the information hierarchy while inverting colors.

## 6. Asymmetry chart

One oversized statement, a simple ratio chart, and a three-row evidence table. Finish with a bottom thesis rule.

## 7. Segments + evidence

Stack three pricing/audience bands, then pair two or more quote cards below. Useful for customer research, market tiers, or stakeholder views.

## 8. Three pillars

Three equal bordered cards with saturated headers. Each card ends in one decisive before/after or outcome row. Add a full-width lime conclusion band.

## 9. Ask / roadmap

Large time-bound claim followed by a shallow shipped-foundation band and two or three oversized deliverable blocks.

## 10. Summary

One oversized stacked phrase at left; numbered argument rows at right. Keep the rest empty.

## 11. Closing

Full purple background, white hero word, cyan secondary question, minimal footer metadata.

# Motion and navigation

Navigation is handled by the bundled `deck-stage.js` runtime. Slides cut instantly; the source deck's confidence comes from static composition, not animated transitions. Do not add entrance animations, parallax, or hover-dependent content.

# Responsive and print behavior

The template is a fixed 1920x1080 presentation system. `deck-stage.js` scales the entire canvas uniformly to fit the viewport. There are no mobile breakpoints and no internal scrolling. All slides must be complete at the native canvas size.

# Do

- End major claims with the colored square period.
- Alternate sparse statement slides with dense evidence slides.
- Use one dominant signal color per slide when possible.
- Align frames and rules precisely across adjacent panels.
- Keep mono labels lowercase and widely tracked.
- Use black blocks decisively; when a region is dark, let it be fully dark.
- Write headlines as conclusions: “The loop compounds from the middle,” not “Our flywheel.”
- Use the exact bundled Focal files.

# Don't

- Do not use rounded cards, pills, shadows, gradients, glass effects, or 3D illustration.
- Do not substitute Inter, Helvetica, or Space Grotesk for Focal.
- Do not use purple as a decorative wash on every surface.
- Do not place four signal colors on a slide unless they encode categories.
- Do not center body copy or long quotations.
- Do not make the grid darker than the content.
- Do not add icons when a number, label, or square marker communicates the structure.
- Do not shrink a long headline below 64px to make it fit; rewrite it.

# Accessibility

- Ink on paper, white on ink, ink on lime, and white on purple are primary contrast pairs.
- Do not set small white type on pink or cyan.
- Pair color with labels, position, or border treatment; never encode meaning through color alone.
- Keep body text at 24px or larger on the 1920x1080 canvas.

# Known gaps

- Consolas may not be installed on every platform. The template falls back to SFMono-Regular and system monospace while preserving spacing and hierarchy.
- Focal is loaded from bundled WOFF2 files. Copy the `fonts/` folder with `template.html`; otherwise browser fallback will change wrapping materially.
- The engineering grid can moire at very small viewport scales. It is intentionally faint and should remain at 5-6% opacity.
- Dense diagrams require careful copy fitting. Prefer shortening labels over reducing font sizes.

# Iteration checklist

1. Choose a single dominant claim.
2. Pick one composition pattern that proves it.
3. Assign one dominant signal color.
4. Add top chrome and page count.
5. Place headline and square period.
6. Build evidence with hairline frames and mono labels.
7. Check alignment across all panel edges.
8. Verify no text clips at 1920x1080.
9. Test the slide between a sparse and a dense neighbor.
10. Render the full deck and inspect every frame.
