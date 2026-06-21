---
source: sources/wiki-Metro_design_language.md
source_url: https://en.wikipedia.org/wiki/Metro_(design_language)
---

## Microsoft Design Language (Metro): Flat Design System for Windows and Mobile

Microsoft Design Language (MDL), commonly known as Metro, is a flat design language created by Microsoft that emphasizes typography, simplified icons, geometric shapes, and a high content-to-chrome ratio. Formally introduced with Windows Phone 7 in 2010, it was adopted across Xbox, Windows 8, and Outlook.com before being succeeded by the Fluent Design System starting in 2017.

## Key Concepts

- **Core principles**: Clean typography, flat design, simplified icons, absence of clutter, "content before chrome" philosophy, basic geometric shapes
- **Rooted in Swiss graphic design** (International Typographic Style) — text-based navigation over icon-based navigation
- **Live Tiles**: Flat colored tiles representing atomic units of information; introduced during early Windows Phone studies
- **Typography-first**: Uses the Segoe font family (variants: Segoe UI, Segoe WP, Zegoe UI for Zune) designed by Steve Matteson at Agfa Monotype
- **Animation and motion**: Transitions, kinetic scrolling, and responsive UI animations are integral — meant to convey an "alive" interface with depth
- **Laterally scrolling canvases**: Larger hubs over smaller buttons; page titles often large and horizontally scrollable
- **MDL2 (Microsoft Design Language 2)**: Evolved alongside Windows 10 — introduced new widgets (date pickers, toggles, switches), thinner borders, and hamburger buttons replacing panorama/carousel navigation
- **Naming history**: "Metro" was always a codename internally; renamed to "Microsoft Design Language" in September 2012, likely due to trademark concerns with German retailer Metro AG

## Commands and Syntax

No CLI commands or configuration syntax — this is a visual design specification. Key implementation guidance:

- **Font usage**: Apply Segoe UI font family; use light/thin font weights for headings
- **Layout pattern**: Full-screen apps, laterally scrolling content areas, large text headings (often lowercase)
- **Tile grid**: Flat-colored rectangular tiles as primary navigation and information display units
- **Motion guidelines**: Animate all transitions and acknowledge user interactions (presses, swipes) with natural motion
- **Chrome reduction**: Minimize window borders, toolbars, and decorative UI elements; let content serve as the interface

## Relationships

- **Predecessor influences**: Windows Media Center (XP era), Zune player interface, MSN 2.0, Encarta 95
- **Successor**: Fluent Design System (introduced 2017), which gradually replaced Metro
- **Peer design systems**: Competes with Apple's iOS Human Interface Guidelines and Google's Material Design (Android)
- **Related Microsoft systems**: Windows Aero (predecessor visual style), Universal Windows Platform apps (app model built on MDL)
- **Broader design movement**: Part of the flat design trend that moved away from skeuomorphism across the industry
- **Products using Metro**: Windows Phone 7/8, Windows 8/8.1, Xbox 360/One dashboards, Outlook.com, Windows Store, Xbox Music/Video

## Exam-Relevant Points

- Metro was **formally introduced with Windows Phone 7 in 2010**, though design principles appeared earlier in Zune (2006) and Windows Media Center
- The design is inspired by **public transport signage systems** and **Swiss graphic design** (International Typographic Style)
- **"Metro" was dropped as a name in August 2012** reportedly due to trademark concerns with Metro AG (Germany); officially became "Microsoft Design Language" in September 2012
- **MDL2** arrived with **Windows 10** and introduced hamburger menus, new widget types, and thinner borders
- **Fluent Design System replaced Metro starting in 2017**
- Key architect: **Joe Belfiore**; Qi Lu coined the interim term "Modern UI"
- Windows Phone 7's Metro UI won **IDSA Gold Interactive, People's Choice, and Best in Show awards** at IDEA 2011
- Windows 8's desktop application of Metro was **widely criticized** as an "awkward hybrid" that undermined multitasking and productivity
- The all-caps text convention in Metro apps drew **significant criticism** for violating platform conventions (especially on macOS)
