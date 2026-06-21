---
source: sources/wiki-Kinetic_scrolling.md
source_url: https://en.wikipedia.org/wiki/Kinetic_scrolling
---

## Scrolling: Display Navigation Techniques Across Computing, Film, and Games

Scrolling is the technique of sliding text, images, or video across a display surface — vertically or horizontally — to reveal content larger than the visible area. It applies across computing (GUIs, terminals, web), film/television (credits, news tickers), and video games (side-scrollers, parallax effects). Scrolling does not change layout; it pans the user's viewport over a larger underlying image or document.

## Key Concepts

- **Software scrolling** — CPU-driven frame buffer manipulation to shift displayed content.
- **Hardware scrolling** — display offset handled by the graphics processor or display hardware without modifying the frame buffer; common on 8-bit and 16-bit consoles.
- **Smooth scrolling** — continuous pixel-level movement, as opposed to discrete jumps (line-by-line or page-by-page).
- **Kinetic scrolling** — touch-based dragging of content, as with a "hand tool" metaphor.
- **Inertial scrolling** — content continues moving after touch release, decaying over time to simulate physical inertia. First implemented on Sun Microsystems' Star7 PDA (~1991–1992).
- **Infinite scrolling** — web design pattern that dynamically loads new content as the user scrolls, creating an apparently bottomless page. Related to the concept of doomscrolling.
- **Parallax scrolling** — multiple semi-transparent layers scroll at different rates to create a pseudo-3D depth illusion. First featured in *Moon Patrol*.
- **Belt scrolling** — side-scrolling beat-'em-up technique with a downward camera angle allowing up/down and left/right movement.
- **Flip-screen** — predecessor to scrolling; the entire screen changes at once when the player crosses a boundary.
- **Paging** — older terminal approach replacing the full display one screenful at a time; requires fewer resources than scrolling.

## Commands and Syntax

No CLI commands per se, but standard UI input mechanisms:

- **Scrollbar manipulation** — mouse-driven, within WIMP GUIs.
- **Keyboard shortcuts** — arrow keys for line-by-line; Page Up / Page Down for screen-at-a-time; Space bar for page-down in many contexts.
- **Control key combinations** — historical: WordStar used Ctrl-S/E/D/X for directional movement, Ctrl-R/Ctrl-C for page up/down.
- **Scroll wheel / scroll ball / tilt wheel** — hardware peripherals for vertical and horizontal scrolling.
- **Touchscreen gestures** — swipe opposite to the desired scroll direction; multi-touch.
- **Tilt-to-scroll** — device tilting as input (Rekimoto, 1996); useful for one-handed operation.

## Relationships

- **Frame buffer & graphics processors** — hardware scrolling avoids frame buffer writes; software scrolling relies on CPU or GPU compositing.
- **Sprite systems** — Namco Galaxian board (1979) combined animated sprites over scrolling backgrounds; foundational for NES hardware.
- **Kinetic typography** — scrolling text in film (e.g., Star Wars opening crawl) is a specialized form of kinetic typography.
- **Word wrap** — determines whether horizontal scrolling is needed for text; word processors and browsers wrap text to avoid it.
- **Demo culture** — scrolltexts in crack intros drove early demoscene creativity, leveraging deep platform knowledge for visual scrolling effects.
- **Eye tracking / auto-scrolling** — research links scrolling control to gaze patterns, removing manual input.
- **Accessibility & ergonomics** — parallax scrolling may cause nausea in some users.

## Exam-Relevant Points

- Hardware scrolling offsets the displayed image without modifying the frame buffer; software scrolling requires CPU/GPU frame buffer manipulation.
- Parallax scrolling uses multiple layers at different scroll rates to simulate depth — first seen in *Moon Patrol*.
- The Namco Galaxian arcade board (1979) pioneered the sprite-over-scrolling-background architecture that became the basis for Nintendo's NES.
- Inertial scrolling was first implemented on Sun's Star7 PDA (~1991–1992), predating modern smartphones.
- Paging (full-screen replacement) preceded scrolling on older terminals and requires fewer resources.
- Taito's *Speed Race* (1974) is cited as an early example of vertical scrolling in video games; Sega's *Moto-Cross* (1976) introduced forward-scrolling (pseudo-3D).
- Tilt-to-scroll research (Rekimoto, 1996) demonstrated one-handed device operation for field workers.
- Eye-tracking auto-scroll studies (Sharmin et al., 2013) found no statistically significant difference in reading speed or performance compared to manual scrolling.
- Parallax scrolling may cause nausea in some users (Frederick et al.).
