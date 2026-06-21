---
source: sources/wiki-Button_computing.md
source_url: https://en.wikipedia.org/wiki/Button_(computing)
---

## GUI Button Controls in Computing

This page covers the **button** graphical control element — its definition, interaction models, visual appearance across major platforms (macOS, Windows, Linux, HTML), and common variants like OK, Cancel, Apply, and toggle/latch buttons.

## Key Concepts

- A **button** (also called command button or push button) is a graphical control element that triggers an event or interacts with dialog boxes.
- Typical shape is a rectangle or rounded rectangle with a descriptive caption; can also be square, round, or icon-based.
- Primary interaction is via mouse/touchpad click, but keyboard input can also activate buttons.
- Any visual element (picture, background area) can be programmed to function as a button — the only requirement is a click-triggered command.
- **Latch button** (latching switch): a toggle-style button that stays visually depressed to indicate on/off state, similar to a checkbox.
- Buttons often display a **tooltip** on hover to explain their purpose.
- Common button types: **OK** (confirm + close), **Cancel** (cancel + close), **Apply** (confirm, stay open), **Close** (close after changes applied).

## Commands and Syntax

- **HTML buttons** are form elements rendered by web browsers, styled via CSS or using the OS-native appearance.
- HTML links can be styled to visually resemble buttons (common in advertising).
- No specific CLI commands — this is a UI design concept. Implementation varies by toolkit and platform.

## Relationships

- Buttons are one type of **graphical control element**, alongside checkboxes, radio buttons, sliders, text boxes, and other widgets.
- Related to **dialog boxes** — buttons are the primary mechanism for confirming or canceling dialog actions.
- Platform-specific rendering depends on the **widget toolkit**: GTK and Qt on Linux, Aqua on macOS, Windows shell on Windows.
- Window management buttons (close, minimize, maximize/zoom) are specialized button instances present across all major OSes.
- Connected to broader **WIMP** (Windows, Icons, Menus, Pointer) interaction paradigm.

## Exam-Relevant Points

- **macOS Aqua**: buttons are rounded-rectangle "crystallized glass"; window controls are top-left, color-coded (red = close, yellow = minimize, green = zoom). Default button animates between shades of blue.
- **Windows**: button style varies by version (rounded corners in XP/Vista/7/11; sharp corners in Windows 8). Window controls are top-right. Default button shown with blue border; in Vista/7 it fades between normal and blue.
- **Linux/Unix**: button appearance depends on the widget toolkit (GTK, Qt, etc.), leading to less visual uniformity across applications. Theming is supported, so no single standard look.
- A button with **keyboard focus** can be activated via spacebar (macOS) or similar key; the **default button** responds to Enter/Return.
- The distinction between a **latch button** (toggle state) and a standard **push button** (single action) is a key UI design concept.
