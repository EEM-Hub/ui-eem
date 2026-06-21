---
source: sources/wiki-Bootstrap_front-end_framework.md
source_url: https://en.wikipedia.org/wiki/Bootstrap_(front-end_framework)
---

## Bootstrap CSS Framework Overview

Bootstrap is a free, open-source CSS framework for building responsive, mobile-first front-end web interfaces. Originally developed at Twitter by Mark Otto and Jacob Thornton in 2010, it provides HTML, CSS, and JavaScript-based design templates for typography, forms, buttons, navigation, and other UI components. The current stable release is v5.3.8 (August 2025), licensed under MIT.

## Key Concepts

- **Purpose**: Applies consistent color, size, font, and layout choices across a web project; provides uniform appearance for prose, tables, and forms across browsers.
- **Container**: The foundational layout component — all other elements are placed inside it. Two types: fixed-width (uses one of six predefined breakpoints) and fluid-width (always fills page width).
- **Breakpoints** (six tiers): <576px, 576–768px, 768–992px, 992–1200px, 1200–1400px, >1400px.
- **CSS Flexbox layout**: Rows and columns are implemented via Flexbox within containers.
- **JavaScript components**: Dialog boxes, tooltips, progress bars, navigation dropdowns, carousels — no jQuery dependency required (as of v5).
- **Distribution forms**: Precompiled (one CSS file + three JS files) or raw/modular (Sass source, allowing removal of unneeded components and theme customization).
- **Adoption**: Used by ~19.2% of all websites (W3Techs); 17th most starred GitHub project with 164,000+ stars.

## Commands and Syntax

No CLI commands per se, but key integration patterns:

- **Include precompiled**: Add the single CSS file and three JS files to any HTML project.
- **Customize via Sass**: Use the raw modular source to compile only needed components and apply custom themes.
- **CSS classes**: Use Bootstrap-defined classes to customize appearance (e.g., light/dark tables, pull quotes, highlighted text).
- **Layout structure**: `Container` > `Row` > `Column` hierarchy using CSS Flexbox.

## Relationships

- **Preprocessors**: v3 used Less; v4+ switched to Sass.
- **jQuery**: Required through v4; removed in v5 in favor of vanilla JavaScript.
- **Alternatives**: Tailwind CSS (utility-first approach), jQuery Mobile, Foundation.
- **Web frameworks**: Integrations exist for Flask (Bootstrap-Flask), Django (django-bootstrap-v5), and others.
- **Related concepts**: CSS frameworks, responsive web design, mobile-first design, CSS Flexbox, flat design.
- **Documentation tooling**: Migrated from Jekyll to Hugo in v5.
- **Testing**: Migrated from QUnit to Jasmine in v5.

## Exam-Relevant Points

- **Version history and key changes**:
  - **v2 (2012)**: Added responsive web design support and Glyphicons.
  - **v3 (2013)**: Adopted flat design and mobile-first approach; dropped IE7/Firefox 3.6 support; moved to `twbs` GitHub org.
  - **v4 (2018)**: Replaced Less with Sass; added Flexbox support; switched from px to rem units; increased base font from 14px to 16px; dropped IE8/IE9/iOS 6; removed Glyphicons, panels, thumbnails, pagers, wells.
  - **v5 (2021)**: Removed jQuery dependency; dropped all IE support; added offcanvas component, RTL support, dark mode, CSS custom properties, custom SVG icon set.
- **License**: MIT (Apache 2.0 prior to v3.1.0).
- **Origin**: Created internally at Twitter in 2010 as "Twitter Blueprint" to enforce UI consistency across internal tools; open-sourced August 19, 2011.
- **Mobile-first**: Core design philosophy since v3.
- **Modular architecture**: Developers can include only the components they need to reduce file size.
