---
source: sources/wiki-Drop-down_list.md
source_url: https://en.wikipedia.org/wiki/Drop-down_list
---

## Drop-Down List (GUI Control Element)

A drop-down list (DDL) is a graphical control element that allows users to select a single value from a list. When inactive, it displays only the currently selected value; when activated, it expands to reveal all available options. After selection, it collapses back to show the chosen value. It is a fundamental widget in GUI and web design.

## Key Concepts

- **Also known as**: drop-down menu, drop menu, pull-down list, picklist
- **Behavior**: Inactive state shows one value; activated state "drops down" to show all options; reverts to inactive after selection
- **Similar to**: List box, but differs in that it collapses when not in use
- **Platform terminology varies**: Called "pop-up menu" on macOS/Macintosh; elsewhere "pop-up menu" refers to context menus
- **Mac distinction**: Pop-up menu title shows the last-selected item; pull-down menu shows a static title (like a menu bar item)
- **Use case distinction**: Pop-up menus select a single option; pull-down menus issue commands or allow multiple selections

## Commands and Syntax

**HTML implementation** using `<select>` and `<option>` elements:
```html
<select>
  <option>option1</option>
  <option>option2</option>
  <option>option3</option>
</select>
```

**GTK 4** provides the `Gtk.DropDown` widget for this purpose.

## Relationships

- **Combo box**: Combines a drop-down list with a text field, allowing both selection and free-text input
- **List box**: Displays multiple items simultaneously without collapsing; drop-down is a space-saving alternative
- **Context menu**: Shares the "pop-up" interaction pattern but serves a different purpose (contextual commands vs. value selection)
- **Belongs to the "command input" category** of GUI control elements, alongside buttons, hamburger buttons, and pie menus

## Exam-Relevant Points

- The HTML elements for creating a drop-down are `<select>` (container) and `<option>` (individual items)
- A drop-down list allows selection of **one** value (single-select by default)
- On macOS, the equivalent is called a "pop-up menu" — terminology differs from other platforms where "pop-up menu" means context menu
- The key differentiator from a list box is that a drop-down **collapses** when inactive, saving screen space
- GTK 4 uses `Gtk.DropDown` as its drop-down widget class
