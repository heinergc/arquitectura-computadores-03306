---
name: Laboratorio de la Unidad de Control · 03306 UNED
description: The course portal as a textbook chapter; each resource is a numbered figure plate with a working diagram and a caption.
colors:
  page: "#eaeef5"
  plate: "#ffffff"
  ink: "#16223d"
  ink-2: "#46526b"
  fig: "#2350c8"
  fig-tint: "#e3eafb"
  data: "#a8470a"
  rule: "#c3cbda"
  ink-rule: "#34405e"
  on-ink: "#dfe5f1"
  on-ink-quiet: "#c9d3ea"
  on-ink-link: "#b9cbff"
typography:
  display:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "clamp(5rem, 11vw, 8.5rem)"
    fontWeight: 600
    lineHeight: 0.8
  headline:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "clamp(2.2rem, 4.4vw, 3.6rem)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.01em"
  title-section:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "clamp(1.6rem, 2.6vw, 2.1rem)"
    fontWeight: 600
    lineHeight: 1.15
  title-plate:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "1.5rem"
    fontWeight: 600
    lineHeight: 1.2
  title-item:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "1.25rem"
    fontWeight: 600
    lineHeight: 1.2
  lead:
    fontFamily: "Source Sans 3, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(1.05rem, 1.4vw, 1.2rem)"
    fontWeight: 400
    lineHeight: 1.6
  body:
    fontFamily: "Source Sans 3, Segoe UI, system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.6
    fontFeature: "lnum"
  meta:
    fontFamily: "Source Sans 3, Segoe UI, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.6
  label:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "17px"
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: "0.02em"
    fontFeature: "smcp"
  label-runhead:
    fontFamily: "Source Serif 4, Georgia, serif"
    fontSize: "16px"
    fontWeight: 600
    lineHeight: 1.3
    letterSpacing: "0.05em"
    fontFeature: "smcp, c2sc"
rounded:
  none: "0"
  focus: "2px"
  diagram: "4px"
spacing:
  gutter: "clamp(16px, 4vw, 56px)"
  item: "10px"
  plate-gap: "24px"
  plate-pad: "24px"
  column-gap: "64px"
  section: "clamp(40px, 6vw, 72px)"
  container: "1280px"
components:
  plate:
    backgroundColor: "{colors.plate}"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
  plate-art:
    padding: "24px 24px 8px"
  plate-caption:
    padding: "18px 24px 22px"
  figure-label:
    textColor: "{colors.fig}"
    typography: "{typography.label}"
  link-open:
    textColor: "{colors.fig}"
    typography: "{typography.body}"
  toc-row:
    textColor: "{colors.ink}"
    padding: "10px 0"
  last-flag:
    textColor: "{colors.data}"
  running-head-resource:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.on-ink}"
    padding: "6px 16px"
    height: "40px"
  running-head-label:
    textColor: "{colors.on-ink-quiet}"
    typography: "{typography.label-runhead}"
  footer:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.on-ink}"
    padding: "48px 0"
  footer-link:
    textColor: "{colors.on-ink-link}"
---

# Design System: Laboratorio de la Unidad de Control · 03306 UNED

## Overview

**Creative North Star: "The Textbook Figure Plate"**

The portal is a chapter of the course textbook, Capítulo R. Each resource appears as a numbered figure (Figura R.1 to R.3): a white plate with a hairline frame, a working SVG diagram of the concept the resource teaches, and a caption below with the title, a description, and an «Abrir» link. The page reads like printed matter: a running head at the top, a large serif chapter letter, a table of contents, numbered figures, a captioned table, and a dark closing band.

Density is moderate and editorial. The type pairing is a serif for chapter heads and figure labels (Source Serif 4) with a sans for reading text (Source Sans 3), both self-hosted from `assets/fonts/` under the OFL. Colour stays cool and quiet: navy ink on a pale blue-grey page, one figure blue for structure, and a single amber for the datum that moves. Depth comes from paper against plate and from rules, never from shadows or gradients.

The motion is the mechanism itself. Each diagram runs its process once when it scrolls into view and again on hover or focus. With reduced motion it stays static in its finished state.

**Key Characteristics:**
- Resources are numbered figure plates, not link cards.
- Hairline 1px rules separate items. A 2px ink rule opens a section or list.
- Two inks inside figures: blue for structure, amber for the moving datum.
- Serif small-caps labels for figure, table, TOC, route and level numbers.
- Chapter identity lives in the running head, never in a kicker above the title.
- Diagrams demonstrate their mechanism once on entering view and on hover/focus.

## Colors

A cool, low-chroma paper palette with one structural blue and one amber reserved for data in motion.

### Primary
- **Figure Blue** (`fig`): diagram wires, figure and table numbers, links, the square markers in fact lists and the coverage table, the focus ring, and text selection. It is the textbook's second colour.
- **Figure Blue Tint** (`fig-tint`): fill of the Unidad de Control box in R.1, the one component the figure singles out.

### Secondary
- **Data Amber** (`data`): only the thing that travels or gets fetched. Used for the R.1 token, the R.2 data cells and legend swatch, and the «Último abierto» flag in Contenido.

### Neutral
- **Plate Paper** (`page`): page background, a pale blue-grey sheet.
- **Plate White** (`plate`): figure plate surface and diagram box fill.
- **Navy Ink** (`ink`): text, headings, diagram box strokes, the internal bus, 2px opening rules, and the footer and resource running-head background.
- **Slate Ink** (`ink-2`): secondary text: captions, descriptions, credit, side notes, diagram sublabels.
- **Hairline** (`rule`): 1px plate frames, list separators, table rows, empty bus cells.
- **On-Ink set** (`on-ink`, `on-ink-quiet`, `on-ink-link`, `ink-rule`): text, the quiet running-head label, links, and dividers on the navy footer and the resource running head.

### Named Rules
**The Two Inks Rule.** Inside figures, Figure Blue draws structure and Navy Ink draws components. Data Amber marks only the datum that moves or the place the student last was. Never use amber for decoration or emphasis.

**The No Gradient Rule.** All surfaces are flat fills. No gradients, glows or tinted overlays.

## Typography

**Display Font:** Source Serif 4 (with Georgia, Times New Roman, serif)
**Body Font:** Source Sans 3 (with Segoe UI, system-ui, sans-serif)

**Character:** A textbook pairing. The serif carries the chapter letter, headings and every numbered label. The sans carries reading text and the text inside diagrams. Body numerals are lining.

### Hierarchy
- **Display** (600, clamp(5rem, 11vw, 8.5rem), 0.8): the chapter letter «R», in Figure Blue, beside the title. Only once per page.
- **Headline** (600, clamp(2.2rem, 4.4vw, 3.6rem), 1.08, -0.01em): page title (h1), balanced wrap.
- **Title, section** (600, clamp(1.6rem, 2.6vw, 2.1rem), 1.15): reading-section headings in the left column.
- **Title, plate** (600, 1.5rem, 1.2; 1.9rem on the lead plate R.1, 1.6rem below 560px): figure caption titles.
- **Title, item** (600, 1.25rem): route-step headings and the Contenido heading.
- **Lead** (400, clamp(1.05rem, 1.4vw, 1.2rem), max 62ch): the single opening paragraph.
- **Body** (400, 17px/1.6; 16px below 560px; max 62–64ch): reading text.
- **Meta** (400, 15px, Slate Ink): descriptions, credit, captions, fact lists.
- **Label** (Source Serif 4 600, 17px, 0.02em, `font-variant-caps: small-caps`, Figure Blue): «Figura R.n», «Tabla R.1», TOC numbers, route steps («1 · R.3»), level numbers (N1–N6). Written in normal case so small caps apply only to lowercase letters.
- **Running-head label** (Source Serif 4 600, 16px, 0.05em, `all-small-caps`): only the current-resource label inside the resource running head.

### Named Rules
**The Small-Caps Label Rule.** Every numbered label is the serif label style in small caps. Use all-small-caps only for the running-head label inside resources.

**The No Kicker Rule.** Never put an eyebrow or kicker above a heading. Chapter identity («Capítulo R · Recursos interactivos») belongs in the running head.

## Layout

A single centred container (max 1280px) with fluid side gutters (clamp(16px, 4vw, 56px)). Page structure from top to bottom:

1. **Running head**: a 14px meta line, course left and chapter right, over a 1px hairline.
2. **Opener**: a 7fr / 5fr grid (64px column gap). On the left, the chapter letter sits beside the title, lead and credit. On the right, Contenido.
3. **Plates**: a 12-column grid with a 24px gap. R.1 spans columns 1–7 across two rows. R.2 and R.3 stack in columns 8–12. Plates are not three in a row.
4. **Reading sections**: a 4fr / 8fr grid with a 2px ink top rule and clamp(40px, 6vw, 72px) vertical padding. The heading and side note sit left, the content right.
5. **Footer**: a navy band with the same 7fr / 5fr grid.

**Responsive.** At 980px and below, every two-column grid collapses to one column and all plates stack full width. At 560px and below, body drops to 16px, the chapter letter stacks above the title, plate padding tightens (art 16px 14px 6px, caption 16px), R.1 swaps to a vertical SVG version, the level list goes to one column, and the coverage table goes fixed-layout so its three mark columns fit without scrolling.

**Rhythm.** List rows are 9–10px top and bottom (route steps 18px). Inside plates the art padding is 24px and caption elements are 10px apart.

### Named Rules
**The Numbered Figure Rule.** Only resources get numbers (R.1–R.n). In-page sections are listed without numbers under a 2px ink rule. A future resource becomes R.4 with its own plate, TOC row, table column and running-head link.

## Elevation & Depth

Flat. There are no shadows anywhere. Depth comes from three things only: the white plate against the blue-grey page, the 1px hairline frame around each plate (with the same hairline between art and caption), and the navy footer band that closes the page.

### Named Rules
**The Hairline and Heavy Rule.** A 1px Hairline separates things of equal rank: plates, list rows, table rows. A 2px Navy Ink rule opens a group: Contenido, the in-page list, each reading section, and the table header.

## Shapes

Plates, rules, table cells and markers are square-cornered (0). The only rounding is functional. Diagram component boxes use 4px, as in a textbook schematic. The R.1 travelling token is a full pill. The focus ring has a 2px radius. List markers are solid 5px squares (facts) or 12px squares (coverage marks, filled for interactive and a 2px outline for term-only). The bus is a 5px round-capped Navy Ink stroke.

## Components

### Figure Plate (signature)
The resource unit. A white plate with a 1px Hairline frame, no radius and no shadow. The top art area holds a live SVG diagram. Below a hairline, the figcaption stacks the «Figura R.n» label, a serif title linked to the resource, a description (max 62ch), optional square-bullet facts, and the «Abrir» link pinned to the bottom.
- **Mechanisms:** R.1 sends a token PC → MAR → Memoria → MBR → IR → UC, changing «0» to «LOAD» once the address leg ends (2.6s, ease-out cubic, resets after 0.9s). R.2 fills bus cells in sequence for the real 20-cycle vs 14-cycle schedule (60ms stagger, 0.25s fill). R.3 swaps the entry between its INGLÉS and ESPAÑOL faces (0.45s fade with an 8px slide).
- **Trigger:** once at 50% visibility, then again on mouseenter or focusin. With reduced motion every figure shows its finished state and nothing animates.

### «Abrir» Link
A 600-weight Figure Blue sans link with no underline at rest and a trailing 18px stroked arrow. On hover or focus the arrow slides 4px right (0.35s, cubic-bezier(.16,1,.3,1)) and the label underlines.

### Inline Links
Figure Blue with a 1px underline at a 3px offset. The underline thickens to 2px on hover. Focus everywhere uses a 2px Figure Blue outline at a 3px offset.

### Contenido (table of contents)
Opens with a 2px Navy Ink rule. Each resource row is a 3.2em label column holding the serif small-caps number, then a 600 Navy Ink title (Figure Blue and underlined on hover) and a 15px Slate description, with hairlines between rows. The «Último abierto» flag (13px, 600, Data Amber) appears beside the resource stored under localStorage key `portal03306_ultimo`. In-page sections follow as an unnumbered 400-weight list under a 2px rule.

### Route and Level Lists
Grid rows with a fixed label column (3.5em for route, 2.4em for levels) holding serif small-caps labels, separated by Hairlines.

### Coverage Table
Full width with a 2px ink header rule and hairline rows. Mark columns are centred, using a filled 12px Figure Blue square for interactive coverage, an outlined square for term-only, and a Slate em dash for not covered. The caption sits below with a «Tabla R.n» label.

### Running Head, resource pages
A navy bar (min height 40px, padding 6px 16px, 1px `ink-rule` bottom border) injected at the top of each resource. Left: a 600 white «Recursos 03306» link with a 16px stroked back arrow. Middle: the current figure label in all-small-caps serif, hidden below 560px. Right: links to the other resources. Hover underlines. Focus is a 2px `on-ink-link` outline. Hidden in print. Fonts load under scoped family names and values are literal hex, so the bar cannot collide with each resource's own styles.

### Footer
A navy band with the course title in white serif, the credit, and a resource link list split by `ink-rule` dividers. Links use `on-ink-link`.

**Out of scope:** the internal designs of `recursos/cpu-quest.html`, `recursos/von-neumann.html` and `recursos/glosario.html` predate this system. They keep their own independent styles and are not governed by this document. Only the running-head bar on those pages belongs to it.

## Do's and Don'ts

### Do:
- **Do** present every resource as a numbered figure plate with a working diagram of its concept, a «Figura R.n» label and a caption.
- **Do** set every numbered label in Source Serif 4 600 17px with `font-variant-caps: small-caps` in Figure Blue.
- **Do** separate peers with a 1px Hairline (#c3cbda) and open groups with a 2px Navy Ink rule.
- **Do** reserve Data Amber (#a8470a) for the datum in motion and the «Último abierto» flag.
- **Do** make each diagram run its mechanism once on entering view and again on hover/focus, and render it static with reduced motion.
- **Do** keep chapter identity in the running head and add the same running-head bar to any new resource page.

### Don't:
- **Don't** add a kicker or eyebrow above the title or any heading.
- **Don't** give plates shadows, radius or gradients. Depth is paper, plate and rule.
- **Don't** number in-page sections. Numbers belong to resources only.
- **Don't** lay the plates out as an equal three-column card row. The lead plate spans 7 of 12 columns across two rows.
- **Don't** use all-small-caps outside the resource running-head label.
- **Don't** restyle the resources' internals to match the portal. Only the running head is shared.
