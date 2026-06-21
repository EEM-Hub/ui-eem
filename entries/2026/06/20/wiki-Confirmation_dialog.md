---
source: sources/wiki-Confirmation_dialog.md
source_url: https://en.wikipedia.org/wiki/Confirmation_dialog
---

## Confirmation Dialog Boxes in User Interfaces

A confirmation dialog is a type of dialog box that asks the user to explicitly approve a requested operation before it proceeds. It is primarily used as a safeguard before potentially dangerous or irreversible actions such as program termination, file deletion, or data-altering operations. It is a subtype of alert dialog box, sometimes called a "warning alert box."

## Key Concepts

- A confirmation dialog **requires explicit user consent** before executing a potentially destructive operation.
- Typical button configurations:
  - **Two-button**: Yes/No or Confirm/Cancel
  - **Three-button**: Save/Discard/Cancel
- Some human interface guidelines (e.g., Microsoft) recommend **avoiding unnecessary confirmation dialogs** — overuse leads to dialog fatigue where users click through without reading.
- **Button ordering convention** (BlackBerry, Sun Java HIG): the confirmation/action button should appear **before** (to the left of) the cancellation button.
- **Default button rule**: the default (pre-focused) button should **not** be associated with a major destructive action — this prevents accidental destructive operations from a careless Enter keypress.

## Commands and Syntax

No commands or code syntax provided in this source. Implementation is platform-specific (e.g., `JOptionPane.showConfirmDialog()` in Java Swing, `window.confirm()` in browsers, `MessageBox` with `MB_YESNO` in Win32).

## Relationships

- **Alert dialog box** — the parent category; confirmation dialogs are a specialized subtype used specifically for approval flows.
- **Error-tolerant design** — confirmation dialogs are one mechanism for achieving error tolerance by giving users a chance to cancel before irreversible actions.
- **Human interface guidelines** — platform-specific HIG documents (Microsoft, BlackBerry, Sun Java) govern when and how confirmation dialogs should be used, including button placement and defaults.
- **Dialog box** — the general UI pattern that confirmation dialogs inherit from.

## Exam-Relevant Points

- A confirmation dialog is specifically for **approving operations**, not for displaying information (that's an alert) or collecting input (that's a form dialog).
- The **default/focused button must not trigger a destructive action** — this is a cross-platform HIG best practice.
- Confirmation button should be placed **before** the cancel button (per Java and BlackBerry HIG).
- Overuse of confirmation dialogs is an **anti-pattern** — guidelines recommend using them only when the action is genuinely dangerous or irreversible.
- Three-button dialogs (Save/Discard/Cancel) are used when the user has **unsaved changes** and the system needs to distinguish between saving, discarding, and aborting the operation entirely.
