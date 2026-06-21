---
source: sources/wiki-Tab_interface.md
source_url: https://en.wikipedia.org/wiki/Tab_(interface)
---

## Tabbed Interfaces in GUI Design

This page covers the **tab** as a graphical user interface element — a navigational widget that allows multiple documents or panels to be contained within a single window. It traces the history of tabbed interfaces from early 1980s word processors through modern web browsers, discusses implementation across widget toolkits and CSS frameworks, and examines the behavioral phenomenon of "tab hoarding."

## Key Concepts

- A **tab** is a GUI object modeled after physical card tabs (desktop metaphor) that enables switching between multiple documents/panels within one window.
- Tabs can be oriented **horizontally** (including multi-row) or **vertically**, and may support drag-and-drop reordering, range-selection, and separation into new windows.
- Tab behavior is determined by the underlying **widget toolkit** (e.g., GTK, Qt), and lack of standardization can cause inconsistent behavior across applications.
- **Tab hoarding** is a form of digital hoarding where users accumulate browser tabs as task reminders, leading to stress, information overload, distraction, and reduced performance.
- Tab hoarding is driven by anxiety, FOMO, procrastination, and poor personal information management.
- Browser vendors have responded to tab hoarding with features like **tab grouping**, collapsing, converting tabs to hyperlink lists, and task-oriented paradigms.

## Commands and Syntax

No CLI commands. Implementation references for developers:

- **CSS Frameworks**: Bootstrap (`navs-tabs/#tabs`), Tailwind CSS (Tailwind UI tab components), Foundation (`tabs.html`)
- **GTK**: `Gtk.Notebook` widget for tabbed containers
- **GTK/Adwaita**: `Adw.TabBar` widget
- **Qt**: `QTabWidget` class (`qtabwidget.html`)

## Relationships

- **Desktop metaphor**: Tabs derive from the physical card-tab metaphor used broadly in GUI design.
- **Widget toolkits**: Tab behavior depends on the toolkit (GTK, Qt) — connects to broader widget toolkit and look-and-feel topics.
- **Container elements**: Tabs are categorized alongside accordions, panels, ribbons, toolbars, and window decorations as GUI container widgets.
- **Multiple Document Interface (MDI)**: Tabs are an evolution of MDI, replacing child windows with a tab bar (IDE-style interface).
- **Browser extensions**: Tab management tools (e.g., MultiZilla) connect to the browser extension ecosystem.
- **Digital hoarding / information overload**: Tab hoarding links to broader UX and cognitive psychology topics.

## Exam-Relevant Points

- **First tabbed product**: WordVision word processor for IBM PC (1982) — possibly the first commercial tabbed interface.
- **Key timeline**: Quattro Pro popularized spreadsheet tabs (1992); Microsoft Word used tabs for submenus (1993); Internet Explorer 7 (2006) made all major browsers tabbed.
- **2009 usage study**: Users switched tabs in 57% of tab sessions; 36% opened search results in new tabs.
- **Standardization gap**: Tab behavior varies across applications because it is determined by the widget toolkit, not a universal standard.
- **Tab hoarding mitigations**: Tab grouping, collapsing, hyperlink conversion, and task-based browsing paradigms.
- **Implementation widgets**: GTK uses `Notebook`, Adwaita uses `TabBar`, Qt uses `QTabWidget`.
