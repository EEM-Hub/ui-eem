---
source: sources/wiki-Check_box.md
source_url: https://en.wikipedia.org/wiki/Check_box
---

## Checkbox (GUI Element)

A checkbox is a graphical widget that allows users to make a binary choice (checked/unchecked). This page covers checkbox states, behavior conventions, tri-state variants, HTML implementation, and related Unicode characters.

## Key Concepts

- **Binary choice widget**: Checkbox represents a yes/no (checked/unchecked) selection
- **Visual states**: Empty box = unchecked; box with tick or cross = checked
- **Activation methods**: Click on box, click on caption/label, or keyboard shortcut (typically space bar)
- **Multiple selection**: Unlike radio buttons, multiple checkboxes in a group can be independently selected — they are non-mutually-exclusive
- **Disabled state**: Checkboxes can be "greyed out" to indicate existence but temporary unavailability
- **Tri-state checkbox**: A third "indeterminate" state (shown as square or dash) indicates mixed state in a collection — e.g., a parent folder where only some children are selected
- **Indeterminate behavior**: Usually not directly selectable by users; clicking cycles between checked (all) and unchecked (none)
- **Not actionable principle**: Toggling a checkbox should only change its state, with no other side-effects — violating this confuses users accustomed to the configure-then-submit pattern
- **Exception**: Enabling/displaying dependent input elements based on checkbox state is acceptable
- **Toggle switch distinction**: For actions with immediate side-effects, a toggle switch widget is preferred over a checkbox

## Commands and Syntax

- **HTML**: `<input type="checkbox">` renders a checkbox in web forms
- **Unicode characters**:
  - U+2610 `☐` — BALLOT BOX (unchecked)
  - U+2611 `☑` — BALLOT BOX WITH CHECK (checked)
  - U+2612 `☒` — BALLOT BOX WITH X (crossed)

## Relationships

- **Radio button**: Mutually exclusive single-selection from a group — contrasted with checkbox's independent multi-selection
- **Toggle switch**: Used instead of checkbox when the state change triggers an immediate action
- **Boolean data type**: Checkbox maps directly to a boolean value (true/false)
- **Tree view**: Often combined with tri-state checkboxes for hierarchical selection (e.g., file/folder selection)
- **Combo box / List box**: Other data input-output controls in the same GUI widget family
- **Form controls**: Checkbox sits alongside text boxes, radio buttons, and sliders as data-entry controls, distinct from action controls like push buttons

## Exam-Relevant Points

- Checkboxes allow **independent, non-mutually-exclusive** selections; radio buttons enforce **mutually exclusive** single selection
- The tri-state/indeterminate checkbox has three states: checked, unchecked, and indeterminate — the indeterminate state is typically **not directly selectable** by the user
- The "not actionable" guideline means checkbox state changes should **not trigger side-effects** — users expect to configure first, then invoke an action separately
- HTML checkbox syntax is `<input type="checkbox">`
- When immediate action on toggle is needed, use a **toggle switch** instead of a checkbox
- Disabled/greyed-out checkboxes communicate that an option **exists but is currently unavailable**
