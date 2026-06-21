---
source: sources/wiki-Cascading_Style_Sheets.md
source_url: https://en.wikipedia.org/wiki/Cascading_Style_Sheets
---

## Cascading Style Sheets (CSS) — Core Language Overview

CSS is a style sheet language used to control the presentation and styling of documents written in markup languages such as HTML and XML. Developed by the W3C and first released in December 1996, CSS separates content from presentation, enabling reusable styles across pages, improved accessibility, and device-adaptive rendering. It is one of the three cornerstone technologies of the World Wide Web alongside HTML and JavaScript.

## Key Concepts

- **Selectors** determine which HTML elements a style rule applies to — by element type, class (`.classname`), ID (`#id`), attribute, pseudo-class, pseudo-element, or combinator
- **Declaration block** consists of `{}` containing semicolon-separated declarations, each with a property, colon, and value
- **Cascading** is the priority scheme that resolves conflicts when multiple rules match the same element — priority flows from browser defaults (lowest) through user-defined, specificity, inline styles, up to `!important` (highest)
- **Specificity** is a weighted scoring system: inline style = `1,0,0,0`; ID = `0,1,0,0`; class = `0,0,1,0`; element = `0,0,0,1` — values do NOT carry over like decimal (11 classes = specificity 11, not carried)
- **Inheritance** passes text-related properties (color, font, line-height, text-align, etc.) from ancestor to descendant elements; box-related properties (margin, padding, border, width, height, display, position) are NOT inherited
- **Positioning schemes** (CSS 2.1): Normal flow, Floats, and Absolute positioning
- **Position property values**: `static` (default), `relative`, `absolute`, `fixed` — only non-static elements respond to `top`/`bottom`/`left`/`right`
- CSS applies to HTML, XHTML, SVG, MathML, XUL, plain XML, and even the GTK widget toolkit
- MIME type: `text/css`; file extension: `.css`

## Commands and Syntax

**Three ways to apply CSS:**
```html
<!-- Inline style (highest specificity) -->
<h1 style="color: red;">Chapter 1.</h1>

<!-- Internal style sheet -->
<style>
    h1 { color: red; }
</style>

<!-- External style sheet (best practice) -->
<link href="path/to/file.css" rel="stylesheet" type="text/css">
```

**Selector syntax examples:**
| Syntax | Meaning | CSS Level |
|---|---|---|
| `E` | Element type | 1 |
| `.c` | Class | 1 |
| `#id` | ID | 1 |
| `E F` | Descendant | 1 |
| `E > F` | Direct child | 2 |
| `E + F` | Adjacent sibling | 2 |
| `E ~ F` | General sibling | 3 |
| `E:hover` | Pseudo-class | 2 |
| `E::first-line` | Pseudo-element (double colon) | 1 |
| `E:not(s)` | Negation | 3 |
| `E:has(s)` | Relational | **4** |
| `E[foo="bar"]` | Attribute exact match | 2 |
| `E[foo^="bar"]` | Attribute starts with | 3 |

**Value units:**
- Absolute: `cm`, `in`, `mm`, `pc`, `pt`
- Relative: `em`, `ex`, `px`
- CSS3 additions: `ch`, `Q`, `rem`, `vh`, `vw`, `vmax`, `vmin`
- Colors: keywords (`red`), hex (`#FF0000` / `#F00`), `rgb()`, `rgba()`, `hsl()`, `hsla()`

## Relationships

- **HTML/XML**: CSS styles documents written in these markup languages; CSS enables separation of content (HTML) from presentation
- **JavaScript**: Together with CSS and HTML, forms the three pillars of the web platform; JS can dynamically manipulate CSS
- **DOM (Document Object Model)**: CSS inheritance follows the document tree hierarchy
- **Preprocessors** (Sass, Less, Stylus): Extend CSS with variables, nesting, and mixins, then compile to standard CSS
- **Frameworks** (Tailwind, Bootstrap, Foundation): Provide pre-built CSS class systems
- **Browser extensions** (Stylish, Stylus): Allow users to apply custom CSS to websites
- **W3C**: Maintains CSS specifications; CSS3 developed as independent modules rather than a monolithic spec

## Exam-Relevant Points

- **Pseudo-class vs pseudo-element notation**: single colon (`:hover`, `:first-child`) for pseudo-classes; double colon (`::first-line`, `::first-letter`) for pseudo-elements
- **Specificity does NOT use decimal carry**: 11 elements + 11 classes = `0,0,11,11`, NOT `0,0,1,21` or `121`
- **Inheritance split**: text properties inherit; box-model properties do not — know which list is which
- **Cascade priority order** (high to low): `!important` > inline > media type > user-defined > specificity > rule order > parent inheritance > CSS in document > browser default
- **Combinator order matters**: `div .myClass` (descendant) vs `.myClass div` vs `div.myClass` (element + class on same element) are three different selectors
- **`:has()` selector** was introduced in CSS Level **4** — the only Level 4 selector in the reference table
- **`position: static`** elements ignore `top`/`bottom`/`left`/`right` offsets
- **`position: absolute`** positions relative to the nearest **non-static** ancestor
- **Float behavior**: absolutely positioned or fixed items cannot be floated; `clear` forces elements below floated items
- **CSS was first proposed** by Håkon Wium Lie in October 1994; co-created with Bert Bos; CSS1 released December 1996
- **Non-zero numeric values** must include a unit (`200px`, `50vw`, `80%`) — unitless non-zero values are invalid for length properties
