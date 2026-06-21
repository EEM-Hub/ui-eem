---
source: sources/wiki-WAI-ARIA.md
source_url: https://en.wikipedia.org/wiki/WAI-ARIA
---

## WAI-ARIA (Web Accessibility Initiative – Accessible Rich Internet Applications)

WAI-ARIA is a W3C technical specification that defines how to make dynamic web content and UI components accessible to users with disabilities. It addresses the gap where native HTML semantics are insufficient — particularly for rich internet applications built with Ajax, JavaScript, and related technologies — by providing a framework of roles, properties, and states that communicate widget behavior to assistive technologies like screen readers.

## Key Concepts

- **Purpose**: Bridges the accessibility gap for dynamic/interactive web content that cannot be made accessible with HTML alone
- **Mechanism**: Adds semantic metadata (roles, properties, states) to HTML elements so assistive technologies can interpret custom UI controls
- **Scope**: Allows pages or page regions to declare themselves as *applications* rather than static documents
- **Not HTML-only**: Can also be applied to other markup languages such as SVG
- **Primary audiences**: Web developers, browser vendors, assistive technology developers, and accessibility evaluation tool makers
- **Current version**: WAI-ARIA 1.2 (W3C Recommendation, June 6, 2023)
- **History**: Started 2006; 1.0 became W3C Recommendation March 2014; 1.1 released December 2017

## The 5 Rules of ARIA

1. **Prefer native HTML** — Don't use ARIA if a native HTML element or attribute provides the same semantics
2. **Don't override native semantics** — Do not change native HTML semantics unless absolutely necessary
3. **Keyboard accessibility required** — All interactive ARIA controls must be operable via keyboard
4. **Don't hide focusable elements** — Never use `role="presentation"` or `aria-hidden="true"` on focusable elements
5. **Accessible names required** — Every interactive element must have an accessible name (exposed via the Accessibility API)

## Commands and Syntax

ARIA is applied via HTML attributes, not CLI commands. Core attribute categories:

- **Roles**: Define what an element *is* (e.g., `role="navigation"`, `role="menu"`, `role="alert"`)
- **Properties**: Describe characteristics (e.g., `aria-label="Close"`, `aria-required="true"`)
- **States**: Describe current conditions that change (e.g., `aria-expanded="false"`, `aria-hidden="true"`)

Example — marking a nav menu:
```html
<ul role="menu" aria-expanded="true">
  <li role="menuitem"><a href="/home">Home</a></li>
</ul>
```

## Relationships

- **HTML/Semantic HTML**: ARIA supplements HTML when native elements lack sufficient semantics; native HTML is always preferred (Rule 1)
- **WCAG (Web Content Accessibility Guidelines)**: ARIA is a *mechanism* for meeting WCAG success criteria; WCAG defines *what* must be accessible, ARIA helps achieve *how*
- **Assistive Technologies**: Screen readers, switch devices, and other AT consume ARIA roles/states/properties via the browser's Accessibility API
- **JavaScript/Ajax**: ARIA exists largely because dynamic JS-driven interfaces break the static-document accessibility model
- **SVG**: SVG Tiny 1.2 added ARIA support (2008), extending accessibility beyond HTML
- **WAI (Web Accessibility Initiative)**: ARIA is one specification within the broader WAI portfolio under W3C

## Key Documents in the WAI-ARIA Suite

- **WAI-ARIA Specification**: Normative spec for browser/AT implementers
- **WAI-ARIA Overview**: Technical introduction describing problems, concepts, and business case
- **WAI-ARIA Authoring Practices**: Developer-facing best practices for building accessible widgets, keyboard nav, drag-and-drop, alerts, dialogs, and reusable component libraries

## Exam-Relevant Points

- The 5 Rules of ARIA are heavily tested — especially Rule 1 (prefer native HTML) and Rule 3 (keyboard operability required)
- ARIA does **not** change element behavior — it only changes what is communicated to assistive technologies; developers must still implement keyboard handling and visual state changes in code
- `role="presentation"` and `aria-hidden="true"` must **never** be applied to focusable elements
- WAI-ARIA became a full W3C Recommendation in **March 2014** (version 1.0); current version is **1.2 (2023)**
- ARIA is a **last resort** — the first question on any accessibility problem should be "can a native HTML element do this?"
- ARIA applies to more than HTML — SVG is explicitly in scope
- The spec targets four audiences: web app developers, browser implementers, AT vendors, and evaluation tool developers
