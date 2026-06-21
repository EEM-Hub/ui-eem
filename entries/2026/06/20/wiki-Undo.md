---
source: sources/wiki-Undo.md
source_url: https://en.wikipedia.org/wiki/Undo
---

## Undo/Redo Interaction Models and Implementation Patterns

This page covers the undo/redo interaction technique in computer programs — its history, theoretical models (linear, non-linear, selective), implementation patterns (command and memento), and the architectural components that make undo systems work. It spans from the 1968 origins at Brown University through modern multi-user applications.

## Key Concepts

- **Undo** erases the last change to a document, reverting to an older state; **redo** reverses an undo or advances to a more recent state.
- Not all actions are undoable — *save file* is logged but not reversible; *scrolling* and *selection* are typically not stored at all.
- Four core components: **commands** (user actions), **history buffer(s)** (completed action storage), **undo/redo manager** (controls the buffer), and **user interface**.
- **Linear undo** uses a LIFO stack — only the most recent command can be undone.
- **Non-linear undo** allows undoing commands in arbitrary order (not just most recent).
- **Flip undo model**: simplistic single-edit undo where undo itself is an undoable action, toggling between two states. Standard before multi-level undo became widespread in the early 1990s.
- **Selective undo**: undo any action in the history buffer; independent actions are left untouched; no command is auto-discarded without user request.
- **Multi-user undo**: *global* reverts the latest action regardless of author; *local* reverts only the local user's actions (requires non-linear undo).
- Making a new edit usually clears the redo list; a **branching redo model** creates a new branch instead.

## Commands and Syntax

- **Undo shortcuts**: Ctrl+Z (Windows/Linux), Cmd+Z (macOS)
- **Redo shortcuts**: Ctrl+Y or Ctrl+Shift+Z (Windows/Linux), Cmd+Shift+Z (macOS)
- Both accessible via the **Edit menu** on all platforms.

**Undo model properties** (formal definitions used in academic literature):
- *Stable execution property*: a command is always undone in the state reached after its original execution.
- *Weakened stable execution*: undoing a command also undoes all dependent younger commands.
- *Stable result property*: like stable execution but the ordered list includes execution context.
- *Commutative*: undoing/redoing two commands in either order yields the same state.
- *Minimalistic undo*: undoing command C only undoes C and dependent younger commands.

**Implementation strategies for reverse operations:**
- *Full checkpoint*: save complete state after each command (simplest, least efficient).
- *Complete rerun*: save initial state; replay commands from the beginning to reach any state.
- *Partial checkpoint*: save only changed state; most commonly used.
- *Inverse function*: compute the reverse operation without storing state (e.g., move back by the same offset).

## Relationships

- **Command pattern** (GoF design pattern): encapsulates actions as objects with execute/unexecute methods; history list enables multi-level undo.
- **Memento pattern** (GoF design pattern): stores internal object state via an originator; a caretaker manages mementos without inspecting their contents.
- Closely related to **version control** — undo is essentially local, in-memory version control.
- Connects to **reversible computing** and **database rollback** as broader applications of the same principle.
- History evolved alongside text editors (FRESS, Bravo, EMACS) and was standardized through the Apple Lisa/Macintosh "Edit" menu convention.

## Exam-Relevant Points

- The **File Retrieval and Editing System (FRESS)** at Brown University (1968) is the first known computer system with undo.
- **Xerox PARC Bravo** (1974) had undo; Xerox PARC originated the **Ctrl+Z** shortcut.
- **Larry Tesler** and **Bill Atkinson** standardized undo on the Apple Lisa; the Macintosh mandated "Undo" as the first item in the Edit menu.
- Linear undo uses a **stack (LIFO)**; restricted linear model clears history when a new command is added.
- Three non-linear sub-models: **script model** (as-if-never-executed semantics), **US&R model** (skip/branch support), **triadic model** (adds rotate operation to reorder the redo list).
- **Command pattern** stores action objects with execute/unexecute; **memento pattern** stores state snapshots via originator/caretaker.
- **Partial checkpoint** is the most commonly used reverse strategy in practice.
- Selective undo has three requirements: undo any action, redo any undone action, no auto-discard without user request.
- Undo history sizes vary by application (e.g., Photoshop defaults to 20, Windows 7 Paint increased to 50).
