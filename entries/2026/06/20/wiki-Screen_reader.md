---
source: sources/wiki-Screen_reader.md
source_url: https://en.wikipedia.org/wiki/Screen_reader
---

## Screen Readers: Assistive Technology for Non-Visual Display Access

Screen readers are assistive technology (AT) software applications that convert on-screen text and image content into speech (via text-to-speech) or braille output using refreshable braille displays. They are essential for blind users and beneficial for visually impaired, illiterate, or learning-disabled users. Screen readers work by interacting with accessibility APIs, querying operating system features (inter-process communication, UI properties), and employing hooking techniques to intercept display information.

## Key Concepts

- **Screen reader** — software that conveys visual display content through non-visual means: text-to-speech, earcons (auditory icons), or braille devices.
- **Off-screen model** — a technique where the screen reader intercepts OS-level drawing messages to build an internal text representation of the GUI, since graphical interfaces lack a purely textual display buffer.
- **Accessibility APIs** — standardized interfaces provided by operating systems and applications that let screen readers query what is displayed and receive change notifications, eliminating the need for an off-screen model.
- **Verbosity** — a configurable setting (low/medium/high) controlling how much structural and formatting detail the screen reader announces (frames, tables, lists, graphics, regions).
- **Scripting** — the ability to customize screen reader behavior for specific applications; scripts can be shared among users to improve accessibility collectively.
- **Multi-language support** — screen readers can switch speech language if the content's language is encoded in metadata.

## Commands and Syntax

No CLI commands per se, but key accessibility APIs that screen readers interact with:

| API | Platform |
|---|---|
| Android Accessibility Framework | Android |
| Apple Accessibility API | macOS, iOS, tvOS |
| AT-SPI | Linux/Unix |
| IAccessible2 | Cross-platform (Windows-focused) |
| Microsoft Active Accessibility (MSAA) | Windows |
| Microsoft UI Automation (UIA) | Windows |
| Java Access Bridge | Java applications |

**Major screen readers by platform:**

- **Windows:** JAWS (commercial, Freedom Scientific), NVDA (free/open-source, NV Access), Microsoft Narrator (built-in since Windows 2000), ZoomText (screen magnifier)
- **macOS/iOS/tvOS:** VoiceOver (built-in, Apple)
- **Android:** TalkBack (Google), VoiceView (Amazon devices)
- **ChromeOS:** ChromeVox
- **Linux:** Orca, Speakup

## Relationships

- **Assistive technology** — screen readers are a subcategory; related AT includes screen magnifiers and speech recognition.
- **Accessibility APIs** — the bridge between applications/OS and screen readers; compliance determines whether content is accessible.
- **Web accessibility standards** — applications that fail to comply with platform accessibility standards cause screen reader failures (relates to WCAG, WAI-ARIA).
- **Text-to-speech / speech synthesis** — the output engine most screen readers rely on.
- **Refreshable braille displays** — hardware output alternative to speech.
- **GUI vs. CLI** — screen readers evolved from simple screen-buffer reading (CLI era) to complex off-screen models and API-driven approaches (GUI era).

## Exam-Relevant Points

- The term "screen reader" originated from IBM's 1984 product "IBM Screen Reader," developed by Jim Thatcher and Jesse Wright from an earlier prototype called SAID (~1978) and PC-SAID.
- Two core techniques for GUI screen reading: **off-screen models** (intercept OS draw messages) and **accessibility APIs** (query structured representations directly). APIs are easier for developers but require application compliance.
- **NVDA** is free/open-source; **JAWS** is the most popular commercial screen reader on Windows; **VoiceOver** is built into all Apple platforms.
- Verbosity settings let users control the granularity of feedback — critical for constructing mental models of web pages.
- Screen readers use **earcons** (non-speech audio cues) in addition to speech and braille.
- Applications that do not comply with accessibility APIs remain inaccessible regardless of screen reader quality — accessibility is a shared responsibility between AT and application developers.
- Microsoft Narrator has been included in Windows since **Windows 2000**.
