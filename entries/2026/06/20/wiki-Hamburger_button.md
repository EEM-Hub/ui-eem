---
source: sources/wiki-Hamburger_button.md
source_url: https://en.wikipedia.org/wiki/Hamburger_button
---

## The Hamburger Button: UI Navigation Menu Icon

This page covers the hamburger button (≡), a UI element consisting of three horizontal parallel lines used to toggle the visibility of a navigation menu or sidebar. It traces the icon's origin, its variants, Unicode representations, and usability criticisms.

## Key Concepts

- The **hamburger button** is a toggle control that shows/hides a collapsed menu or navigation bar, typically placed in a top corner of a GUI.
- The **hamburger icon** (three parallel horizontal lines) is designed to visually resemble lines of text in a small menu; it is named for its incidental resemblance to a hamburger.
- The icon is **not a Unicode character** — it is a graphical element, though designers sometimes substitute visually similar Unicode characters.
- The hamburger pattern resurged around **2009** driven by the constraints of mobile screen real estate.
- **Variants** include:
  - **Kebab button**: three vertically stacked dots (⋮) — used to further reduce space consumption.
  - **Meatball/falafel button**: similar dot-based variants.
  - **Waffle button**: a 3×3 grid of squares, used in Microsoft Office 365 and Google apps to display an icon array rather than a text menu.

## Commands and Syntax

- **Unicode substitutes for hamburger icon**: U+2261 (≡ IDENTICAL TO), U+2630 (☰ TRIGRAM FOR HEAVEN), U+11054 (𑁔 BRAHMI NUMBER THREE) — note: not universally supported across browsers/fonts, may render as □ (tofu).
- **Unicode substitutes for kebab icon**: U+22EE (⋮ VERTICAL ELLIPSIS), U+205D (⁝ TRICOLON), U+FE19 (︙).
- **CSS implementation**: W3Schools documents `howto_css_menu_icon` for creating a hamburger icon with CSS (three styled `<div>` bars).

## Relationships

- **Menu bar vs. hamburger menu**: The hamburger menu is a space-saving alternative to a persistent menu bar, trading discoverability for screen real estate.
- **Interaction cost**: Hamburger menus increase interaction cost (extra clicks) compared to visible menu bars.
- Related UI concepts: **navigation bar**, **context menu**, **drop-down list**, **pie menu**, **tab bar**.
- Related symbols: **triple bar** (≡) in application design, **ellipsis** (…) which indicates "more options" rather than a full hidden menu.

## Exam-Relevant Points

- **Origin**: Designed by **Norm Cox** for the **Xerox Star** (1981) with a 16×16 (or possibly 13×13) pixel constraint.
- **Windows history**: Appeared in **Windows 1.0** (1985), removed in **Windows 2.0** (replaced by single line), replaced by program icon in **Windows 95**, returned in **Windows 10 Anniversary Update** (2016).
- **Mobile resurgence**: Started around **2009** due to limited mobile screen space.
- **Usability criticism**: The icon's function is not self-evident to all users, especially older or less tech-savvy users; designers tend to overload it with too much hidden information.
- **Kebab vs. hamburger vs. waffle**: Kebab = vertical dots (overflow/secondary menu), hamburger = three lines (main navigation), waffle = 3×3 grid (app launcher/switcher).
- The hamburger icon is a **graphical element, not a standardized Unicode character** — using Unicode substitutes risks rendering failures across platforms.
