---
source: sources/wiki-Hyperlink.md
source_url: https://en.wikipedia.org/wiki/Hyperlink
---

## Hyperlinks: Definition, Types, and Implementation

A hyperlink is a digital reference in computing that provides direct access to data when a user clicks or taps on it. This page covers the definition and taxonomy of hyperlink types, their implementation across technologies (HTML, XLink, file-based formats), browser rendering behavior, the history of hyperlink invention from 1965 onward, and legal issues surrounding linking and copyright.

## Key Concepts

- A **hyperlink** (or link) points to a whole document or a specific element within a document; the text linked from is called **anchor text**.
- The document containing a hyperlink is its **source document**; the destination is the **target**.
- **Hypertext** is text that contains hyperlinks; a hypertext system is software for viewing and creating it.
- Links can be **unidirectional** (standard HTML) or **bidirectional** (both ends act as anchors and targets).
- A **webgraph** models web pages as vertices and hyperlinks as directed edges.
- **Link rot** refers to hyperlinks becoming broken over time; a 2013 study found the median lifespan of a web page was 9.3 years, with only 62% archived.
- **HREF** stands for "Hypertext REFerence."

## Link Types

- **Inline link**: Displays remote content (e.g., thumbnails, previews) without embedding the full resource; full content available on demand.
- **Anchor link** (fragment link): Points to a specific portion of a document, marked by an anchor element. In URLs, the `#` character precedes the fragment identifier.
- **Fat link** (extended link, multi-tailed link): A one-to-many link leading to multiple endpoints; a set-valued function.
- **Text hyperlink**: Embedded in a word or phrase, making it clickable.
- **Image hyperlink**: Embedded in an image, making the image clickable.
- **Bookmark hyperlink**: Navigates to another part of the same page.
- **E-mail hyperlink**: Opens a mail client to send a message to the embedded address.
- **Deep link**: Points to content within a site, bypassing the home page or designated entry point.
- **Permalink**: A URL intended to remain unchanged long-term, reducing link rot.

## Commands and Syntax

**HTML anchor element:**
```html
<a href="https://www.w3.org/" title="link title" target="link target" class="link class">link label</a>
```

Five main characteristics of an HTML link: `href` (destination URL), link label (anchor text), `title`, `target`, and `class`/`id`.

**Fragment linking in URLs:**
- HTML fragment: `page.html#section-id`
- PDF page reference: `document.pdf#page=386`

**Special target values:**
- `_blank` / `_new` — open in a new window/tab
- `_top` — clear all frames, load in full window

**Windows .url shortcut file:**
```ini
[InternetShortcut]
URL=https://www.wikipedia.org/
```

**macOS .webloc file (XML plist):**
```xml
<plist version="1.0">
<dict>
  <key>URL</key>
  <string>https://www.wikipedia.org/</string>
</dict>
</plist>
```

**Linux .desktop file:**
```ini
[Desktop Entry]
Encoding=UTF-8
Type=Link
Name=Wikipedia
URL=https://www.wikipedia.org/
```

**Cross-platform link.html (meta-refresh redirect):**
```html
<meta http-equiv="refresh" content="0; url=https://www.wikipedia.org" />
```

**XML anchoring:**
```xml
<anchor id="name" />
```

## Relationships

- **HTML and the `<a>` element**: Hyperlinks are the foundational mechanism of the World Wide Web, implemented via the HTML anchor element.
- **CSS**: Link appearance (color, decoration, hover states) is controlled via Cascading Style Sheets.
- **XLink (W3C)**: Extends linking capabilities beyond HTML with multidirectional and cross-document links in XML.
- **Web crawlers/spiders**: Programs that automatically follow hyperlinks to index web content (e.g., for search engines).
- **Transclusion**: A link behavior where the target fragment replaces the link anchor inline within the source document.
- **PageRank**: Google's algorithm that uses hyperlink structure (the webgraph) to rank pages.
- **Image maps**: Define clickable hot areas in images using coordinate-based boundaries.
- **Digital preservation / Permalinks**: Persistent URLs designed to combat link rot.
- **URI fragments**: The `#identifier` portion of a URL that navigates to a specific anchor within a document.

## Exam-Relevant Points

- Default browser link colors: **unvisited = blue underlined**, **visited = purple underlined**, **active = red underlined**.
- HREF stands for **Hypertext REFerence**.
- The term "link" was coined by **Ted Nelson** in 1965 as part of **Project Xanadu**, inspired by Vannevar Bush's 1945 essay "As We May Think" and the concept of the **Memex**.
- **Douglas Engelbart's** team implemented the first hyperlink for scrolling within a document (1966) and between documents (1968) using **NLS**.
- **Ben Shneiderman** designed the first highlighted link in the **HyperTIES** system (1983).
- **Tim Berners-Lee** cited HyperTIES in his 1989 Web manifesto.
- **HyperCard** (1987, Apple Macintosh) enabled hyperlinking between pages and to external applications.
- The **Gopher protocol** (1991) was the first widely used open protocol with cross-site hyperlinks; eclipsed by HTML after the **Mosaic browser** release (1993).
- A **fat link** leads to multiple endpoints (one-to-many relationship).
- File-based hyperlink formats are platform-specific: `.url` (Windows), `.webloc` (macOS), `.desktop` (Linux); cross-platform via `link.html` using meta-refresh.
- Legal: In U.S. jurisprudence, merely linking to another site (even bypassing ads) is generally **not** copyright or trademark infringement, but linking to **illegal or infringing content** can create legal liability.
- British Telecom's 2000 patent claim over web hyperlinks (U.S. Patent 4,873,662) was ruled **not to cover** web hyperlinks.
