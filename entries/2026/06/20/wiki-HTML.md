---
source: sources/wiki-HTML.md
source_url: https://en.wikipedia.org/wiki/HTML
---

## HTML (HyperText Markup Language) — Web Document Structure and Standards

HTML is the standard markup language for creating web pages. Originally proposed by Tim Berners-Lee at CERN in 1989–1990, it defines the content and structure of web documents using a system of nested elements delimited by tags. HTML is extended from SGML and is now maintained by WHATWG as a "Living Standard." It works alongside CSS (presentation) and JavaScript (behavior) to produce modern web pages.

## Key Concepts

- **HTML elements** are the building blocks — they consist of a start tag, content, and an end tag (e.g., `<p>...</p>`), or are self-closing/empty (e.g., `<br>`, `<img>`)
- **Attributes** provide additional information on elements (e.g., `href`, `src`, `type`), placed inside the start tag
- **Document Type Declaration** (`<!DOCTYPE html>`) triggers standards-mode rendering; omitting it causes browsers to fall back to **quirks mode**
- **Three types of markup**: structural (semantic purpose, e.g., `<h1>`), presentational (appearance, e.g., `<b>`, mostly deprecated), and hypertext (links via `<a>`)
- **Semantic vs. presentational elements**: `<strong>` and `<em>` are preferred over `<b>` and `<i>` because they convey meaning, not just visual style
- **Character references** encode special characters: named (`&amp;`), decimal (`&#38;`), or hexadecimal (`&#x26;`)
- **HTML is not case-sensitive** for tag and attribute names, unlike XHTML
- **Empty elements** (void elements) like `<br>`, `<img>`, `<input>` cannot have content or closing tags
- HTML documents follow a required structure: `<!DOCTYPE>`, `<html>`, `<head>`, `<body>`

## Commands and Syntax

**Minimal valid HTML5 document:**
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Page Title</title>
  </head>
  <body>
    <p>Hello world!</p>
  </body>
</html>
```

**Headings** — six levels, `<h1>` (highest) through `<h6>` (lowest):
```html
<h1>Main Heading</h1>
<h2>Subheading</h2>
```

**Links** — anchor element with `href` attribute:
```html
<a href="https://www.example.com/">Link text</a>
```

**Images** — empty element with `src` attribute:
```html
<img src="example.com/photo.jpg">
```

**Inputs** — various types via the `type` attribute:
```html
<input type="text">
<input type="file">
<input type="checkbox">
```

**Comments:**
```html
<!-- This is a comment -->
```

**Character references:**
- Named: `&amp;` renders `&`
- Decimal: `&#38;` renders `&`
- Hexadecimal: `&#x26;` renders `&`

## Relationships

- **SGML** — HTML was originally defined as an SGML application; HTML5 abandoned strict SGML conformance
- **XHTML** — a reformulation of HTML 4.01 in XML; XHTML enforces stricter syntax (lowercase tags, quoted attributes, all tags closed). XHTML 2.0 was abandoned in favor of HTML5
- **CSS** — separates presentation from structure; W3C has encouraged CSS over presentational HTML tags since 1997
- **JavaScript** — embedded via `<script>` to add interactivity and dynamic behavior
- **DOM (Document Object Model)** — the programmatic interface browsers build from parsed HTML, manipulated via JavaScript
- **W3C vs. WHATWG** — W3C formerly maintained HTML; since May 2019, WHATWG is the sole publisher of the HTML Living Standard. W3C publishes periodic snapshots as Recommendations

## Exam-Relevant Points

- **HTML5 doctype** is simply `<!DOCTYPE html>` — no DTD URL required (unlike HTML 4.01/XHTML)
- **HTML 2.0** (1995) was the first specification treated as a formal standard (RFC 1866)
- **HTML 4.01** (1999) introduced three variants: **Strict**, **Transitional**, and **Frameset**
- **HTML5** became a W3C Recommendation on **28 October 2014**; it added `<canvas>`, `<video>`, `<audio>` elements
- **WHATWG** became the sole publisher of HTML and DOM standards on **28 May 2019**
- HTML is now a **Living Standard** — continuously updated, never versioned as "complete"
- **Quirks mode** is triggered when the DOCTYPE declaration is missing or malformed
- **Semantic elements** (`<strong>`, `<em>`, `<article>`, `<nav>`) are preferred over presentational elements (`<b>`, `<i>`, `<font>`) for accessibility and standards compliance
- **Tim Berners-Lee** created HTML at CERN; the first public description ("HTML Tags", 1991) listed **18 elements**, 11 of which survived to HTML 4
- HTML file extensions: `.html` and `.htm`; MIME type: `text/html`
- **XHTML 1.0** required well-formed XML: all tags closed, lowercase element names, attribute values quoted
