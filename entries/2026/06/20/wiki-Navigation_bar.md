---
source: sources/wiki-Navigation_bar.md
source_url: https://en.wikipedia.org/wiki/Navigation_bar
---

## Navigation Bars in User Interfaces

A navigation bar (or navigation system) is a GUI element designed to help users access information. Navigation bars appear across operating systems, file browsers, web browsers, apps, and websites. This page covers the different contexts in which navigation bars are used and their implementation in HTML5.

## Key Concepts
- A navigation bar is a section of a graphical user interface that aids in accessing and traversing information
- Navigation bars exist in multiple contexts: file browsers, web browsers, and web pages
- In file browsers, nav bars show the current path, breadcrumbs, or a list of favorites
- In web browsers, the nav bar includes back/forward buttons and a location (address) bar for URLs
- Google Chrome pioneered merging the toolbar and address bar into a single navigation bar
- Websites typically have a primary navigation bar and sometimes a secondary one across all pages
- Navigation bars are most commonly placed in a page's header but can also appear as a sidebar
- Types include horizontal and vertical navigation bars; JavaScript enables responsive designs

## Commands and Syntax
- HTML5 `<nav>` tag is the semantic element for navigation sections
- Early Netscape used the `<link>` tag for site navigation; the `<nav>` tag replaced this purpose
- Standard pattern: `<nav>` wrapping a `<ul>` with `<li>` items containing `<a>` links:
```html
<nav>
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/blog">Blog</a></li>
    <li><a href="/contact">Contact</a></li>
    <li><a href="/about">About</a></li>
  </ul>
</nav>
```

## Relationships
- **Graphical control elements**: Navigation bars are categorized as "Navigational" controls alongside address bars, bookmark bars, breadcrumb navigation, hyperlinks, and virtual desktops
- **Web design and usability**: Implementation and design of navigation bars is a core concern of web design and usability disciplines
- **Related navigational elements**: Address bar, breadcrumb navigation, bookmark bar
- **Container elements**: Toolbars, menu bars, and ribbons serve related organizational purposes
- **Filesystem concepts**: File browser nav bars relate to paths, breadcrumbs, and filesystem navigation

## Exam-Relevant Points
- The `<nav>` tag is the correct HTML5 semantic element for navigation sections
- Google Chrome introduced the practice of merging the toolbar and address bar
- Navigation bars belong in the "Navigational" category of graphical control elements (distinct from "Containers" like toolbars and menu bars)
- The `<nav>` tag typically contains an unordered list (`<ul>`) of links
- Primary navigation bars appear on all pages of a website; secondary nav bars are optional
- Navigation bars can be horizontal, vertical, or responsive (with JavaScript)
