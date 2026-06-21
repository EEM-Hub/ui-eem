---
source: sources/wiki-Slider_computing.md
source_url: https://en.wikipedia.org/wiki/Slider_(computing)
---

## Slider (Track Bar) — GUI Control Element

A slider (also called a track bar) is a graphical control element that lets a user set a value by moving an indicator along a track. Unlike a scrollbar, a slider adjusts a discrete value without changing the display format or other on-screen information. Users may also click directly on a point along the slider to set a value.

## Key Concepts

- **Slider / Track Bar**: A GUI widget for selecting a single input value from a well-defined range by dragging an indicator (threshold bar) along a scale.
- **Distinct from Scrollbar**: A scrollbar navigates content; a slider sets a value. Sliders are not continuous in the same sense — they adjust a parameter rather than scroll a view.
- **Input mechanism**: Users manipulate the indicator with a mouse (or pointer device) to specify a value.
- **Related input tools**: Dials, bars, pointers, gauges, and potentiometers serve similar graphical input functions.
- **Common use case**: Adjusting playback position in media player software.
- **Combined with progress bars**: In streaming media (e.g., YouTube), a colored shaded area is superimposed on the slider to show buffered content vs. current playback position, indicating whether the user can skip forward.

## Commands and Syntax

No commands or configuration syntax — this is a conceptual UI element. Implementation varies by toolkit. Historical examples include:

- **Yahoo! UI Library** — Slider component
- **ASP.NET AJAX Control Toolkit** — Slider control
- **script.aculo.us** — Slider demo widget

## Relationships

- **Parent category**: Graphical control elements (data input-output subcategory).
- **Sibling widgets**: Checkbox, color picker, combo box, radio button, scrollbar, spinner, text box, toggle switch.
- **Often paired with**: Progress bars (in streaming media contexts).
- **Contrast with**: Scrollbar (continuous navigation vs. discrete value selection).
- **Broader context**: Part of the WIMP (Windows, Icons, Menus, Pointer) paradigm and widget toolkits.

## Exam-Relevant Points

- A slider selects a **single value from a defined range** — this is its formal definition (Eick, 1994).
- The key distinction from a scrollbar: sliders **adjust a value** without changing display format; scrollbars **navigate content**.
- In streaming media, sliders are **combined with progress bars** to show buffer state vs. playback position.
- Sliders fall under the **data input-output** category of graphical control elements, alongside checkboxes, spinners, and combo boxes.
