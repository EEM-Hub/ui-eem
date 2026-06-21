---
source: sources/wiki-Graphical_user_interface.md
source_url: https://en.wikipedia.org/wiki/Graphical_user_interface
---

## Graphical User Interface (GUI) — Concepts, History, and Components

A graphical user interface (GUI) is a form of user interface that enables interaction with electronic devices through graphical icons, visual indicators, and widgets rather than text-based commands. This page covers the definition, design principles, core components (WIMP paradigm), historical development from Xerox PARC through modern touchscreens, comparisons with CLIs, and 3D GUI innovations.

## Key Concepts

- **GUI** — interface using graphical elements (icons, windows, menus, pointers) for human-computer interaction, replacing typed command labels
- **WIMP paradigm** — Windows, Icons, Menus, Pointer — the dominant interaction model for personal computers
- **Direct manipulation** — users perform actions by interacting directly with on-screen graphical elements rather than issuing abstract commands
- **Desktop metaphor** — the display simulates a physical desktop with documents and folders, managed by a desktop environment
- **Post-WIMP** — newer interaction paradigms (e.g., multi-touch pinch/rotate on iOS, Android) that go beyond single-pointer WIMP for touchscreen devices
- **Chrome** — the visible graphical interface features of an application (also called "GUI" colloquially)
- **Model-View-Controller (MVC)** — architectural pattern that decouples the interface from application logic, enabling skins/themes
- **Usability** — the design discipline focused on enhancing efficiency and ease of use of stored programs
- **GUI wrappers** — graphical front-ends built on top of CLI applications to lower the learning curve
- **Widgets** — visual interactive elements (buttons, checkboxes, radio buttons, text fields, canvases) that support user actions appropriate to the data they hold
- **Windowing system** — handles hardware devices (pointing devices, graphics hardware) and pointer positioning; a window manager facilitates interactions between windows, applications, and the windowing system
- **Vertical market GUIs** — application-specific interfaces such as ATMs, POS terminals, self-service kiosks, and industrial control screens (often on RTOS)

## Commands and Syntax

No CLI commands per se, but relevant technical details:

- **CSS layout patterns for GUIs on the web:**
  - "Shelf" layout (fixed height, variable width): `display: inline-block;`
  - "Waterfall" layout (fixed width, variable height): `column-width: <value>;`
- **Inter-process communication for GUI events:** `inotify` (filesystem events), `D-Bus` (message bus between programs)
- **Display server protocols:** X Window System (X11), Wayland — the layers beneath desktop environments

## Relationships

- **CLI vs. GUI** — GUIs were introduced to reduce the learning curve of CLIs; most modern OSes provide both; CLIs remain more lightweight, scriptable, and efficient for expert users
- **Desktop environments** — GNOME, KDE Plasma, Xfce, Cinnamon, MATE, Enlightenment — sit atop windowing systems to provide full GUI experiences on Linux/Unix
- **Human-Computer Interaction (HCI)** — GUI design is a subdiscipline of HCI, applying user-centered design methods
- **Windowing system hierarchy** — hardware → windowing system → window manager → desktop environment → application GUI
- **Touch UIs** — overlay visual output onto visual input; extend GUI concepts to mobile (iOS, Android)
- **3D GUIs and compositing** — Windows Aero, macOS Aqua, Compiz; related to augmented/virtual reality interfaces
- **Natural User Interface (NUI)** — evolution beyond GUI toward gesture, voice, and other organic interaction styles

## Exam-Relevant Points

- **First graphical CAD program:** Sketchpad by Ivan Sutherland (1963), used a light pen
- **Mouse invention context:** Douglas Engelbart's On-Line System (NLS) at Stanford Research Institute, demonstrated in 1968 ("The Mother of All Demos")
- **First computer with a GUI:** Xerox Alto (1973), developed at Xerox PARC; never commercially produced
- **First commercially available GUI computer:** PERQ workstation (1979) by Three Rivers Computer Corporation
- **Xerox Star (8010):** 1981, commercial version of Alto ideas
- **Apple Lisa:** 1983, introduced menu bar and window controls concepts; commercially unsuccessful
- **Apple Macintosh 128K:** 1984, popularized the GUI for consumers
- **Key figures:** Ivan Sutherland (Sketchpad), Douglas Engelbart (mouse/NLS), Alan Kay (Smalltalk GUI on Xerox Alto), David Canfield Smith (icons concept)
- **IBM Common User Access (CUA):** formed the basis for GUIs in Microsoft Windows, OS/2 Presentation Manager, and Unix Motif
- **Windows 95:** major marketplace success, became most popular desktop OS at launch
- **iPhone (2007) / iPad (2010):** popularized post-WIMP multi-touch interaction
- **Visi On (1983):** GUI for IBM PC compatibles, failed due to high hardware demands but influenced Microsoft Windows development
- **WIMP acronym:** Windows, Icons, Menus, Pointer (or Pointing device)
- **GUI vs. CLI tradeoffs:** GUIs lower learning curve but are harder to script; CLIs are lightweight and efficient but require memorizing commands; GUIs use modes extensively (meaning of keys/clicks changes by context)
