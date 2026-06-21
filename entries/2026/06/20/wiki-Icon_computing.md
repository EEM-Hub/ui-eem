---
source: sources/wiki-Icon_computing.md
source_url: https://en.wikipedia.org/wiki/Icon_(computing)
---

## Icons in Computing: Visual Symbols for User Interface Navigation

This page covers the concept of icons in computing — graphic symbols displayed on screens to help users navigate computer systems. It traces the history, semiotic classification, types, design constraints, and creation tools for computer icons, from early pixel art to modern photorealistic designs.

## Key Concepts

- **Icon definition**: A graphic symbol on a computer screen that helps users navigate; can serve as a hyperlink or file shortcut, activated by mouse, pointer, finger, or voice commands.
- **Semiotic classification** (three types):
  - **Icon (Pictogram)**: Resembles its referent directly (e.g., a printer icon looks like a printer)
  - **Index**: Associated with its referent by relationship (e.g., scissors icon means "cut")
  - **Symbol**: Related to its referent only by convention (e.g., power symbol, USB icon)
- **Encoding methods**: Icons primarily use **metonymy** (part represents related whole, e.g., light bulb for power settings), **synecdoche** (part stands for whole, e.g., speaker driver for audio system), and **metaphor** (familiar object transposed to unfamiliar context).
- **Skeuomorphism**: Using visual representations of obsolete physical objects (e.g., floppy disk for "save") because they remain widely recognized.
- **Desktop metaphor**: Icons based on 1970s physical office objects (files, folders, trashcan, inbox) enabling intuitive navigation; originated at Xerox and adopted across personal computing.
- **Design constraints**: Icons are thumbnail-sized, frequently scalable, and may include multiple optimized versions for different sizes, color depths, and background types (e.g., Apple Icon Image format).
- **David Canfield Smith** coined the term "icon" in computing context in his 1975 PhD thesis "Pygmalion: A Creative Programming Environment."
- **Xerox Star** (1981): First commercially available personal computing system based on the desktop metaphor.

## Commands and Syntax

- **Icon file formats**:
  - `.ICO` — Windows and web page icons
  - `.ICNS` — macOS icons (Apple Icon Image format)
  - `.CUR` — Cursor files (Windows/Mac)
  - `.ANI` — Animated cursor files
- **Icon creation tools**:
  - **Commercial**: Axialis IconWorkshop, IcoFX, IconBuilder (Photoshop plug-in), Microangelo Toolset, Visual Studio
  - **Open source**: GIMP (reads/writes ICO/CUR/ANI/PNG), ImageMagick/GraphicsMagick (command-line conversion)
  - **Freeware/other**: IrfanView (format conversion), ResEdit (classic Mac OS resources)
- **Resource editing**: Tools like Resource Hacker and Resource Tuner can extract or replace icons embedded in Windows executable files.
- **Assigning icons to programs**: Typically done within the IDE, or by adding a line to the program's resource script before compilation (Windows API).

## Relationships

- **GUI history**: Icons are part of the WIMP paradigm (Windows, Icons, Menus, Pointer) — a core element of the graphical user interface.
- **Semiotics**: Icon design draws on semiotic theory (Peirce's icon/index/symbol trichotomy).
- **Desktop metaphor → Cloud computing**: The desktop metaphor (files, folders, trashcan) is giving way to cloud-based models where data is stored remotely rather than locally.
- **Brand identity**: Commercial software icons double as company branding, subject to trademark protection.
- **Overlay icons**: Secondary icons layered over primary icons to indicate object status (e.g., padlock for locked files in Windows).
- **Standards bodies**: IEC (IEC 417 standard for graphical symbols on equipment) and ICT organizations publish icon guidelines.
- **Related formats/technologies**: Favicon, Font Awesome, The Noun Project, Unicode symbols, XPM.

## Exam-Relevant Points

- Icons serve three semiotic functions: **pictogram** (resemblance), **index** (association), and **symbol** (convention) — know examples of each.
- The **floppy disk save icon** is the canonical example of **skeuomorphism** in UI design.
- **David Canfield Smith** introduced the term "icon" to computing (1975); the **Xerox Star** (1981) was the first commercial desktop-metaphor system.
- Desktop metaphor components evolved across decades: data files (1950s), hierarchical file system (1960s), full desktop metaphor with trashcan (1970s).
- Standard icon formats: **ICO** (Windows/web), **ICNS** (macOS), **CUR/ANI** (cursors).
- Icons use **alpha channels** for transparency effects in modern rendering.
- **IEC 417** is the standard for graphical symbols on electronic equipment.
- Microsoft MSDN defines standard icon types: **error, warning, information, question mark**.
- iOS and Android **regulate icon design** through human interface guidelines to maintain UI consistency.
- The **cloud metaphor** is replacing the desktop metaphor in modern computing paradigms.
