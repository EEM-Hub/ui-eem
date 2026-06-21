---
source: sources/wiki-Radio_button.md
source_url: https://en.wikipedia.org/wiki/Radio_button
---

## Radio Buttons (UI Control Element)

Radio buttons are a fundamental graphical user interface control element that allows users to select exactly one option from a predefined set of mutually exclusive choices. This page covers their definition, etymology, HTML implementation, Unicode representation, and relationship to other UI controls.

## Key Concepts

- A radio button (also called an **option button**) enforces **mutual exclusivity** — selecting one option automatically deselects any previously selected option in the same group.
- This mutual exclusivity distinguishes radio buttons from **checkboxes**, which allow multiple simultaneous selections.
- Radio buttons are always arranged in **groups of two or more**; a single radio button alone is not meaningful.
- Visual representation: typically a circular hole that is either empty (unselected) or contains a dot (selected).
- Each radio button should be accompanied by a **label** describing the choice it represents.
- Users can interact via mouse click, touch, or keyboard shortcut. Clicking the label also selects the button.

## Commands and Syntax

**HTML implementation** using `<input type="radio">`:

```html
<form>
    <input type="radio" name="season" value="winter" id="winter" checked>
    <label for="winter">Winter</label>
    <input type="radio" name="season" value="spring" id="spring">
    <label for="spring">Spring</label>
    <input type="radio" name="season" value="summer" id="summer">
    <label for="summer">Summer</label>
    <input type="radio" name="season" value="autumn" id="autumn">
    <label for="autumn">Autumn</label>
</form>
```

- The **`name`** attribute defines the group — all radio buttons sharing the same `name` are mutually exclusive.
- The **`checked`** attribute sets the default selection.
- The **`value`** attribute defines the data submitted with the form.
- The **`id`** and `<label for="">` pairing associates labels with their buttons for accessibility and click targeting.

**Unicode representation:**
- U+1F518 🔘 `RADIO BUTTON` (Miscellaneous Symbols and Pictographs)
- Similar glyphs: U+2299 ⊙ `CIRCLED DOT OPERATOR`, U+25C9 ◉ `FISHEYE`, U+25CE ◎ `BULLSEYE`

## Relationships

- **Checkbox vs. Radio Button**: Checkboxes allow multi-select; radio buttons enforce single-select. This is the core distinction in form design.
- Radio buttons belong to the broader category of **data input-output controls**, alongside checkboxes, combo boxes, sliders, spinners, toggle switches, and text boxes.
- Defined in **RFC 1866** (HTML 2.0 specification) and the **W3C HTML 4.01** specification as a standard form control.
- The name originates from physical **car radio preset buttons**, where pressing one button mechanically pops out the others.

## Exam-Relevant Points

- Radio buttons enforce **mutually exclusive selection** within a group; checkboxes do not.
- In HTML, the **`name` attribute** is what groups radio buttons together — not their position in the DOM or any container element.
- Only **one** radio button per group can be selected at a time.
- Radio buttons should be used for groups of **two or more** options.
- The `checked` attribute sets the **default selected** option.
- Use radio buttons when the user must choose **exactly one** option; use checkboxes when zero or more selections are valid.
- Jakob Nielsen's usability guidance (Nielsen Norman Group) specifically addresses when to use checkboxes vs. radio buttons — a classic UX design consideration.
