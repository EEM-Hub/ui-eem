---
source: sources/wiki-Scrolling.md
source_url: https://en.wikipedia.org/wiki/Scrolling
---

## Scrolling: Display Navigation via Sliding Content

Scrolling is the technique of sliding text, images, or video across a display surface — vertically or horizontally — to reveal portions of content larger than the visible area. It appears across computing, film/television, and video games. Scrolling does not change content layout; it pans or tilts the user's view across a larger image. It can be user-controlled, automatic (e.g., film credits), or a hybrid triggered by user action then continuing autonomously.

## Key Concepts

- **Software scrolling** — CPU-driven; the frame buffer is manipulated each frame to reposition content.
- **Hardware scrolling** — display hardware offsets the image without frame buffer manipulation; common on 8-bit and 16-bit consoles.
- **Smooth scrolling** — continuous pixel-level movement, as opposed to discrete jumps (line-by-line or page-by-page).
- **Paging** — older terminals replaced the entire screen contents one "page" at a time; less resource-intensive than scrolling.
- **Kinetic scrolling** — touch-driven dragging of content (the "hand tool" paradigm applied to touchscreens).
- **Inertial scrolling** — content continues moving after touch release, decelerating as if affected by friction; first implemented on Sun Microsystems' Star7 PDA (~1991–1992).
- **Infinite scrolling** — web design pattern that dynamically loads new content as the user scrolls, creating an apparently bottomless page. Related to the behavioral concept of **doomscrolling**.
- **Parallax scrolling** — multiple semi-transparent layers scroll at different rates to create a pseudo-3D depth illusion; first featured in *Moon Patrol*.
- **Belt scrolling** — side-scrolling technique in beat-em-up games with a downward camera angle, allowing movement on both axes (left/right and up/down).
- **Frame rate** constrains scrolling smoothness — content position can only update as fast as the display refreshes. Motion blur is used to mask "jumping" at low frame rates.

## Commands and Syntax

No CLI commands or configuration syntax. Relevant **input methods** for scrolling:

- **Keyboard**: Arrow keys for line-by-line; Page Up / Page Down or Space Bar for page-at-a-time; Ctrl-key combinations on older systems (e.g., WordStar used Ctrl-R / Ctrl-C for page up/down).
- **Mouse**: Scroll wheel (vertical), scroll ball or tilt wheel (vertical + horizontal), middle-click drag (omni-directional scrolling in some software).
- **Touchscreen**: Swipe gesture in the direction *opposite* to desired scroll direction (multi-touch gesture).
- **Tilt/motion**: Tilting a device to scroll or select (Rekimoto, 1996); moving a spatially-aware device to pan content as if it were fixed in space (Fitzmaurice, 1993).

## Relationships

- **Scrollbar** — the primary GUI widget for controlling scroll position in WIMP interfaces.
- **Word wrap** — eliminates the need for horizontal scrolling by fitting text to screen/column width.
- **Sprite systems** — the Namco Galaxian arcade board's sprite-over-scrolling-background architecture influenced the NES and early console hardware design.
- **Flip-screen** — the predecessor technique to scrolling in video games, where the entire background swaps rather than sliding.
- **Flip page** — a distinct visual navigation metaphor (page-turning) as an alternative to scrolling in digital publications.
- **Demo scene / crack intros** — scrolling text ("scrollers") was a foundational display technique in early computer demo culture, born from software crackers showcasing platform knowledge.

## Exam-Relevant Points

- Hardware scrolling offsets the displayed image without modifying the frame buffer; software scrolling requires CPU-driven buffer manipulation.
- Inertial scrolling originated with Sun Microsystems' Star7 PDA (1991–1992), not with the iPhone.
- Parallax scrolling was first featured in *Moon Patrol* and uses multiple layers scrolling at different speeds for pseudo-3D depth.
- The Namco Galaxian board (1979) pioneered the sprite-over-scrolling-background system that became the basis for NES hardware.
- Taito's *Speed Race* (1974) is cited as an early example of vertical-scrolling gameplay; Sega's *Moto-Cross* (1976) as an early forward-scrolling (2.5D) example.
- Eye-tracking-based auto-scrolling (Sharmin et al., 2013) showed no statistically significant difference in reading speed or performance versus manual scrolling.
- Parallax scrolling may cause nausea in some users (Frederick et al.).
- Paging (full-screen replacement) predates scrolling and requires fewer resources.
