---
source: sources/wiki-Scroll_bar.md
source_url: https://en.wikipedia.org/wiki/Scroll_bar
---

## Scrollbar: GUI Widget for Content Navigation

A scrollbar is a graphical user interface widget that enables scrolling continuous content (text, images, etc.) in a predetermined direction within a window or viewport. It solves the problem of navigating content that exceeds the visible display area. Scrollbars typically consist of a draggable thumb (also called scroller, knob, scroll box, elevator, or grip) within a trough (track), often with arrow buttons at the ends.

## Key Concepts

- **Thumb (scroller/knob/scroll box)**: The draggable element within the scrollbar that controls scroll position and may indicate the visible portion of content relative to the whole.
- **Trough (track)**: The full-length area along which the thumb moves; clicking in the trough jumps to that position or scrolls page-by-page.
- **Proportional thumb**: A thumb whose size reflects the ratio of visible content to total content. Pioneered by Smalltalk (1977), adopted by GEM and AmigaOS (1985), but not added to Windows until Windows 95.
- **Fixed-size thumb**: Earlier implementations (Xerox Star, Apple Lisa, early Mac) used a constant-size thumb regardless of document length.
- **Scrollbar vs. slider**: A slider changes values; a scrollbar changes the visible portion of content. They look similar but are functionally distinct.
- **Natural scrolling**: Introduced by Apple in Mac OS X 10.7 (2011) — content moves in the same direction as finger movement on the trackpad.
- **Disappearing scrollbars**: Scrollbars that hide when not in use (iOS 2007, Mac OS X 10.7, Microsoft Word 2015) to reduce visual clutter.
- **Inertia scrolling**: Flicking fingers on a trackpad causes content to continue scrolling and gradually decelerate.

## Commands and Syntax

**CSS Scrollbar Customization (WebKit browsers):**
```css
::-webkit-scrollbar          /* entire scrollbar */
::-webkit-scrollbar-button   /* arrow buttons */
::-webkit-scrollbar-track    /* trough/track */
::-webkit-scrollbar-track-piece
::-webkit-scrollbar-thumb    /* draggable thumb */
::-webkit-scrollbar-corner
::-webkit-resizer
```
- IE 5.x+ and Opera supported non-standard CSS directives for scrollbar colors.
- WebKit also provides pseudo-classes for conditional styling of scrollbar states.

**Interaction Methods:**
- **Thumb dragging**: Click and hold the thumb, drag to scroll. On Windows, moving the pointer ~100px away from the thumb while dragging resets to prior position.
- **Scroll wheel**: Forward/backward wheel movement scrolls content; some mice support multi-directional scrolling.
- **Arrow keys**: Keyboard arrows scroll slowly; holding a key continues scrolling.
- **Trough clicking**: Click above/below the thumb to jump or page through content.
- **Arrow buttons**: Click on-screen arrows for single-unit increments; hold for continuous scroll.
- **Two-finger trackpad**: Mac gesture for smooth scrolling with inertia support.

## Relationships

- **Scrolling**: The underlying action that scrollbars control — content movement within a viewport.
- **Slider widget**: Visually similar but functionally different; sliders adjust values rather than viewport position.
- **Viewport/Window**: The bounded display area that scrollbars extend beyond.
- **Interaction techniques**: Scrollbars are one of many GUI interaction patterns alongside drag-and-drop, selection, and resizing.
- **Operating system UI frameworks**: Scrollbar behavior and appearance are tightly coupled to the OS (Windows, macOS, RISC OS, BeOS, AmigaOS each have distinct implementations).
- **2D scrolling**: Special scrollbar variants (e.g., GTK+ GtkScrollpane) allow simultaneous horizontal and vertical panning.
- **Scroll Lock key**: Related keyboard feature for controlling scroll behavior.

## Exam-Relevant Points

- The first scrollbar-like interaction appeared in **Bravo (1974)** using cursor position and colored mouse buttons.
- **Smalltalk (1977)** introduced the first **proportional scrollbar**.
- The **Xerox Star (1981-82)** moved the scrollbar from the left to the **right side** of the window.
- **GEM (1985)** produced the first scrollbar with a proportional thumb that is essentially identical to modern scrollbar behavior.
- **Apple's "natural scrolling"** was introduced in **Mac OS X 10.7 (Lion, 2011)**, which also removed arrow buttons from scrollbars.
- Scrollbar accuracy is **linear** — navigation precision degrades as document size increases.
- On **Windows**, dragging the thumb and moving the pointer ~100px away resets to the prior scroll position.
- **RISC OS** uses different mouse buttons for different scroll operations, including right-button drag for simultaneous 2D scrolling.
- **iPhone (2007)** introduced output-only scrollbars (visible but not directly interactive).
- Proportional thumbs that fill the entire trough indicate the **entire document is visible**, and the scrollbar may hide.
