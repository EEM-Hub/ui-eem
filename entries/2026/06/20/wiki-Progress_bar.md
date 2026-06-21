---
source: sources/wiki-Progress_bar.md
source_url: https://en.wikipedia.org/wiki/Progress_bar
---

## Progress Bars: Types, History, and Perception

A progress bar is a graphical control element used to visualize the progression of extended computer operations such as downloads, file transfers, or installations. This page covers the two main types (determinate and indeterminate), the historical origins of progress visualization, and research into how humans perceive progress bar behavior.

## Key Concepts

- A **progress bar** is a graphical control element that visualizes progression of an extended operation, often accompanied by a percentage text representation.
- **Determinate progress bars** fill proportionally to the amount of work completed, using a linear function.
- **Indeterminate progress bars** indicate activity is occurring without expressing a percentage — used when the extent of the task is unknown. They use motion or patterns (e.g., barber's pole) and function more like a **throbber**.
- Progress bars are classified under **informational** graphical control elements (alongside icons, tooltips, status bars, loading screens, etc.).
- **Playback bars** in media players are a related concept, tracking current position within media duration.
- Dual progress bars are sometimes used for compound operations (e.g., overall installation progress + individual file copy progress).

## Commands and Syntax

No commands or configuration syntax — this is a UI concept rather than an implementation specification.

## Relationships

- **Parent category**: Graphical control element (informational subtype).
- **Related elements**: Progress indicator (broader category), throbber (similar to indeterminate progress bars), loading screen.
- **Historical predecessor**: Gantt chart (Karol Adamiecki's harmonogram, 1896) — the concept of visualizing task progression over time predates computing.
- **Peer elements in the informational group**: Label, icon, tooltip, toast, status bar, sidebar, splash screen, balloon help, HUD.

## Exam-Relevant Points

- First graphical progress bar appeared in **Mitchell Model's 1979 Ph.D. thesis** (*Monitoring System Behavior in a Complex Computational Environment*, Xerox PARC).
- **Brad Myers' 1985 CHI paper** on "percent-done progress indicators" demonstrated that progress bars **reduce user anxiety** and make waits feel more efficient.
- Progress bars typically use a **linear function**, but real-world factors (disk, memory, CPU, bandwidth) cause **non-linear behaviors** (acceleration, deceleration, pauses).
- Humans have **non-linear perception of time**, meaning progress bar design can be manipulated to make operations "feel" faster (Harrison et al., 2007 and 2010).
- Karol Adamiecki invented the harmonogram in **1896** but published only in **1931** in Polish; it is now known as the **Gantt chart** after Henry Gantt (1910–1915).
- Indeterminate progress bars are distinct from determinate ones and are functionally closer to **throbbers** than to traditional progress bars.
