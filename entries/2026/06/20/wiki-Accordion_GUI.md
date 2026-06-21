---
source: sources/wiki-Accordion_GUI.md
source_url: https://en.wikipedia.org/wiki/Accordion_(GUI)
---

## Accordion (GUI Control Element)

The accordion is a graphical control element used in user interfaces that presents a vertically stacked list of items — such as labels or thumbnails — where each item can be expanded or collapsed to reveal associated content. The name derives from the musical accordion, whose bellows sections expand outward. This page covers the definition, behavior, and classification of the accordion widget within the broader taxonomy of GUI control elements.

## Key Concepts

- An accordion is a **vertically stacked list** where each item can be independently expanded or collapsed to show/hide its content.
- Expansion behavior is configurable: **zero, exactly one, or multiple** items may be expanded simultaneously.
- The accordion is classified as a **container** control element (alongside tree views, panels, tabs, toolbars, and windows).
- It is functionally similar to a **tabbed interface**, but uses inline expand/collapse rather than separate panels.
- The "shaded window" metaphor applies: all items show only their headers (captions); clicking one "unshades" it, displacing others.

## Commands and Syntax

No standardized commands or configuration syntax — implementation varies by framework. Historical implementations include:

- **jQuery UI**: `jqueryui.com/demos/accordion` — a widely used accordion widget.
- **MooTools**: referred to the effect as a "sliding shelf."
- General pattern: a Show/Hide toggle operation applied to multiple stacked sections.

## Relationships

- **Tabbed interface**: similar purpose (show one panel at a time), but tabs use horizontal navigation while accordions stack vertically; tabs enforce exactly-one-visible, accordions optionally allow multiple.
- **Disclosure widget**: a single expand/collapse control; an accordion is essentially multiple disclosure widgets stacked together.
- **Code folding**: analogous technique applied to text/code rather than UI content.
- **Tree view**: another container that uses expand/collapse, but in a hierarchical parent-child structure rather than a flat list.
- **Panel / Frame**: the expanded content area of each accordion item is essentially a panel.

## Exam-Relevant Points

- The accordion belongs to the **Containers** category in the GUI control element taxonomy (not Navigational or Informational).
- Key differentiator from tabs: accordion items stack **vertically** and may allow **zero or multiple** expanded items; tabs typically enforce **exactly one** active panel.
- The accordion pattern is a **Show/Hide operation extended to multiple sections** in a list — this is the canonical definition.
- Configuration variants to remember: **zero expanded**, **single expanded** (exclusive), or **multiple expanded** (non-exclusive).
