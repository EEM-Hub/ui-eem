---
source: sources/wiki-Tooltip.md
source_url: https://en.wikipedia.org/wiki/Tooltip
---

## Tooltips: GUI Hover Information Elements

This page covers tooltips — a common graphical user interface element that displays contextual information (text box) when a user hovers over or long-presses a screen element. The article traces the origin of the term, platform-specific variants, and implementation methods.

## Key Concepts

- A **tooltip** (also called infotip, hint, mouseover, or hover text) is a text box that appears when hovering over a UI element, providing descriptions, abbreviations, timestamps, etc.
- On **desktop**, tooltips activate on pointer hover without clicking.
- On **touch-screen devices**, tooltips appear on **long-press** (tap and hold); some devices with a stylus support hover-triggered tooltips.
- Tooltips can **nest**: hovering within a tooltip's text box can activate another tooltip, to arbitrary depth.
- The tooltip remains visible continuously as long as the user hovers over the element or its text box.
- An older variant displayed tool descriptions in a **status bar** rather than a floating text box.
- **Platform-specific names**:
  - Microsoft: **ScreenTips**
  - Apple (developer docs): **help tags**
  - Classic Mac OS: **balloon help**
- Some applications (e.g., GIMP) allow users to **disable tooltips**, but this is developer-discretionary and often not implemented.

## Commands and Syntax

- In **HTML**, the `title` attribute on an element causes most graphical browsers to render a tooltip on hover.
  ```html
  <a href="https://example.com" title="Visit Example">Example Link</a>
  ```
- Tooltips can be customized using **CSS**, **HTML**, and **JavaScript**.
- The **ARIA `tooltip` role** provides accessible tooltip semantics:
  ```html
  <span role="tooltip">Helpful description</span>
  ```
- **WCAG 2.2 Success Criterion 1.4.13** ("Content on Hover or Focus") governs tooltip accessibility requirements.

## Relationships

- **Mouseover / Hoverbox**: The interaction pattern that triggers tooltips on desktop.
- **Dialog box / Popover**: Related but distinct UI patterns; tooltips are non-interactive informational overlays, while dialogs and popovers may accept input.
- **Status bar**: An older alternative location for displaying the same contextual information tooltips show.
- **Balloon help**: Apple's Classic Mac OS predecessor to modern tooltips.
- **Toolbar**: The original context where tooltips appeared (describing toolbar button functions), giving the element its name.
- Falls under the **Informational** category of graphical control elements, alongside icons, progress bars, toasts, labels, and sidebars.

## Exam-Relevant Points

- The term "tooltip" originated from **Microsoft Word 95**-era applications describing toolbar icon functions.
- **WCAG 2.2 SC 1.4.13** is the relevant accessibility criterion for tooltip-like content appearing on hover or focus.
- On mobile/touch devices, the equivalent interaction is **long-press**, not hover (unless a stylus with hover capability is available).
- The HTML `title` attribute is the standard mechanism for browser-native tooltips.
- Microsoft calls tooltips **ScreenTips**; Apple calls them **help tags** (developer docs) or **balloon help** (Classic Mac OS).
- Tooltips are classified as **informational** GUI elements, not command-input or navigational elements.
- Material Design provides specific tooltip component guidelines (material.io).
