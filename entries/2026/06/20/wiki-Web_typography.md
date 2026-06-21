---
source: sources/wiki-Web_typography.md
source_url: https://en.wikipedia.org/wiki/Web_typography
---

## Web Typography: Font Delivery and Rendering on the Web

This page covers the history, techniques, and standards for controlling typeface display on web pages. It traces the evolution from browser-controlled fonts through CSS font properties, web-safe fonts, and modern web font formats (`@font-face`, WOFF), including the licensing and technical challenges of delivering custom fonts to users.

## Key Concepts

- **Web typography** is the design of web page layout and typeface choices, distinguished from print typography by dynamic presentation and cross-platform rendering challenges.
- **Web-safe fonts** are fonts expected to be installed on most systems, used as a reliability strategy when custom fonts are unavailable.
- **Fallback fonts** are a CSS mechanism where multiple fonts are listed in priority order; the browser walks the list until it finds one available, falling back per-character if needed.
- **Generic font families** (serif, sans-serif, monospace, cursive, fantasy) serve as last-resort categories when no specified font is available.
- **`@font-face`** is the CSS construct that enables downloading and using remote fonts, first specified in CSS2 (1998).
- **WOFF (Web Open Font Format)** is compressed OpenType/TrueType with metadata; it became the de facto standard web font format after joint submission to W3C by Mozilla, Opera, and Microsoft (2010).
- **Unicode fonts** map glyphs to Unicode code points; a single TrueType font is limited to 65,535 glyphs, making full Unicode coverage in one font impossible (159,801+ characters in Unicode 17.0).
- **Font licensing** is a persistent concern — using `@font-face` to serve commercial fonts may violate licenses; web font licenses exist as a separate category from desktop licenses.

## Commands and Syntax

**CSS font-family with fallback chain:**
```css
font-family: "Nimbus Sans L", Helvetica, Arial, sans-serif;
```

**CSS font properties (CSS1):**
- `font-family` — typeface selection
- `font-style` — italic/normal
- `font-variant` — small-caps
- `font-weight` — bold/normal/numeric
- `font-size` — size specification

**@font-face embedding** (CSS3): enables loading remote font files (TTF, OTF, WOFF) for rendering in the browser.

**CSS4 system font generic families (limited browser support):**
- `system-ui`, `ui-serif`, `ui-sans-serif`, `ui-monospace`, `ui-rounded`
- `emoji`, `math`, `fangsong`

## Relationships

- **CSS specifications (CSS1 → CSS2 → CSS2.1 → CSS3 → CSS4):** Font capabilities expanded across each revision; some CSS2 features were removed in CSS2.1 and restored in CSS3.
- **Font format evolution:** TrueDoc (1994) → EOT (1997, IE-only) → TrueType/OpenType linking (2008–2009) → WOFF (2010) → WOFF2.
- **Google Fonts** (launched 2010): Major distribution platform for open-source web fonts, hosting 800+ families by 2016.
- **Microsoft Core Fonts for the Web** (1996–2002): Established Arial, Courier New, Times New Roman, Georgia, Verdana as de facto web standards.
- **SVG fonts** were part of SVG 1.1, later deprecated in SVG 2.0; the surviving standard is SVG glyphs embedded within OpenType (SVGOpenTypeFonts).
- **Alternatives to web fonts** historically included image replacement, Flash-based sIFR, and JavaScript-rendered VML/SVG — all now obsolete.

## Exam-Relevant Points

- The `<font>` element was introduced by **Netscape in 1995** and standardized in **HTML 3.2**.
- **CSS1 (1996)** provided font-family, font-style, font-variant, font-weight, font-size — no font downloading.
- **CSS2 (1998)** introduced `@font-face` for font downloading; **IE4 (1997)** was the first browser to implement it (using EOT format).
- **WOFF** = OpenType/TrueType + compression + metadata. Submitted to W3C in 2010 by Mozilla, Opera, and Microsoft.
- The five original **generic font families**: sans-serif, serif, monospace, cursive, fantasy.
- **TrueType font glyph limit**: 65,535 glyphs maximum — cannot cover all of Unicode in a single font.
- **Web-safe fonts** rely on the fallback mechanism: browser tries each font in the `font-family` list sequentially, including on a per-character basis.
- **CSS4 draft** adds `system-ui` and `ui-*` generic families to match native OS look-and-feel (limited browser support as of 2024).
- **Licensing distinction**: desktop font licenses typically do not permit web use; a separate **web font license** is required for `@font-face` delivery.
- **Google Fonts** serves fonts under open-source licenses, removing licensing friction.
