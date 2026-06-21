---
source: sources/wiki-Text_box.md
source_url: https://en.wikipedia.org/wiki/Text_box
---

## Text Box (GUI Control Element)

A text box (also called input box, text field, or text entry box) is a fundamental GUI control element that allows users to enter and edit text. This page covers its visual characteristics, standard keyboard/mouse interactions, editing modes, and an alternative meaning in typography and print design.

## Key Concepts

- A text box is a rectangular control element within a graphical user interface for text input
- Typically displays a text cursor (blinking vertical line) indicating the active edit position
- Mouse cursor usually changes shape when hovering over a text box
- Two editing modes exist: **insert mode** (new characters push existing text right) and **overwrite mode** (new characters replace existing text), toggled via the Insert key
- Text boxes may include scrollbars (horizontal and/or vertical) for content that exceeds the visible area
- Some simplified implementations (e.g., in video games) omit standard functionality
- The term "text box" also has a separate meaning in typography/print design: a bordered or shaded region used for callouts, pull quotes, or sidebars

## Commands and Syntax

**Mouse operations:**
- Click to reposition the caret
- Click-and-drag to select a range of text

**Keyboard navigation (Windows / Mac):**
- Arrow keys: move caret one character or line
- `Home` / `End` (Win) or `Cmd+Left` / `Cmd+Right` (Mac): jump to line start/end
- `Ctrl+Arrow` (Win) or `Option+Arrow` (Mac): move by word or paragraph
- `Ctrl+Home` / `Ctrl+End` (Win) or `Cmd+Up` / `Cmd+Down` (Mac): jump to document start/end
- `Page Up` / `Page Down`: move caret by one visible page (Win) or scroll without moving caret (Mac)
- `Shift` + any navigation: extend selection from original caret position
- `Ctrl+A` (Win): select all text

**Editing:**
- `Delete`: remove character to the right of caret
- `Backspace`: remove character to the left of caret
- `Ctrl+Delete` / `Ctrl+Backspace` (or `Cmd` equivalents): remove one word
- `Ctrl+Z` / `Ctrl+Y` (Win) or `Cmd+Z` / `Cmd+Shift+Z` (Mac): undo/redo
- Standard clipboard operations (cut, copy, paste)
- Typing while text is selected replaces the selection

## Relationships

- **Parent category:** Graphical control elements (data input-output)
- **Sibling controls:** Checkbox, combo box, radio button, slider, spinner, list box, search box, color picker
- **Related concepts:** Scrollbar (often embedded in text boxes), text cursor, clipboard operations, undo/redo
- **Container context:** Text boxes appear within windows, dialogs, panels, forms, and toolbars
- **Print design overlap:** The term also applies to bordered content regions in desktop publishing — callouts, pull quotes, sidebars, and infoboxes

## Exam-Relevant Points

- A text box is classified as a **data input-output** control, not purely input or purely informational
- Insert vs. overwrite mode distinction and the Insert key toggle
- Platform differences matter: `Page Up`/`Page Down` behavior differs between Windows (moves caret) and Mac (scrolls without moving caret)
- Windows uses `Ctrl` as the modifier for word-level and document-level navigation; Mac splits this between `Option` (word/paragraph) and `Command` (line/document)
- Selecting text with the keyboard always involves holding `Shift` in combination with navigation keys
- Typing over a selection replaces it — this is standard across platforms
- The caret (blinking line) and the mouse cursor (pointer shape change) are two distinct visual indicators associated with text boxes
