---
source: sources/wiki-Breadcrumb_navigation.md
source_url: https://en.wikipedia.org/wiki/Breadcrumb_navigation
---

## Breadcrumb Navigation in User Interfaces

Breadcrumb navigation is a graphical control element that provides a secondary navigational aid in user interfaces and web pages. It helps users track their location within a site hierarchy or their browsing path, and is named after the trail of bread crumbs in the fairy tale of Hansel and Gretel. Breadcrumbs appear in both web and desktop software contexts, typically as a horizontal series of linked labels separated by delimiters.

## Key Concepts

- A **breadcrumb trail** displays either the user's browsing path or the hierarchical position of the current page within a site structure.
- Breadcrumbs are typically placed **horizontally below the masthead or main navigation** of a website.
- The **greater-than sign (>)** is the most common hierarchy separator; other glyphs (`, >) and icons are also used.
- Three distinct types of breadcrumbs exist:
  - **Path (history):** Dynamic; shows the sequence of pages the user visited to reach the current page.
  - **Location:** Static; shows where the current page sits in the site's structural hierarchy.
  - **Attribute:** Describes metadata or categories that apply to the current page.
- Location breadcrumbs are **not ideal for content-rich sites** where a single category cannot fully describe a page; **tags** may be more appropriate in those cases.
- Breadcrumbs may include **drop-down menus** at each level and support **drag and drop** (e.g., Windows Explorer).
- "Cookie crumb" is an informal synonym; unrelated to HTTP cookies.
- In French/Spanish, the concept is sometimes called **Ariadne's thread** (*fil d'Ariane*), referencing a LIFO (stack) traversal metaphor rather than the FIFO (queue) implied by the Hansel and Gretel metaphor.

## Commands and Syntax

No CLI commands. Typical rendering patterns:

**Path-based breadcrumb (history):**
```
Home page > Services > About Us > Home page > Latest Newsletter > Current Page
```

**Hierarchy-based breadcrumb (location):**
```
Home page > Section page > Subsection page
```

## Relationships

- **Navigation patterns:** Breadcrumbs complement primary navigation (nav bars, menus) as a secondary aid; they do not replace primary navigation.
- **Address bars:** In desktop file managers (Dolphin, Nautilus, Windows Explorer, Finder, Thunar, Nemo, Caja), breadcrumbs often replace or extend the traditional address bar.
- **Tags / metadata:** For highly categorized or multi-category content, tags serve a similar wayfinding purpose and may be preferred over or used alongside breadcrumbs.
- **Other navigational controls:** Breadcrumbs belong to the broader family of navigational UI elements alongside address bars, bookmark bars, hyperlinks, and virtual desktops.
- **Data structures:** Path breadcrumbs follow a FIFO (queue) model; the Ariadne's thread metaphor follows LIFO (stack) backtracking.

## Exam-Relevant Points

- Know the **three types** (path, location, attribute) and the difference between dynamic (path) and static (location) breadcrumbs.
- Location breadcrumbs are **static and hierarchy-based**; path breadcrumbs are **dynamic and history-based**.
- Breadcrumbs are a **secondary** navigation mechanism, not a replacement for primary navigation.
- The default separator is **>** (greater-than sign).
- Location breadcrumbs are **inappropriate when content belongs to multiple categories**; attribute breadcrumbs or tags are better in that scenario.
- Desktop file managers across all major platforms (Windows, macOS, Linux/KDE/GNOME/Xfce/MATE) implement breadcrumb navigation in their address bars.
- "Cookie crumb" is a synonym for breadcrumb navigation and is **not related to HTTP cookies**.
