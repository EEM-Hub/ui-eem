---
source: sources/wiki-Web_Content_Accessibility_Guidelines.md
source_url: https://en.wikipedia.org/wiki/Web_Content_Accessibility_Guidelines
---

## Web Content Accessibility Guidelines (WCAG) — Overview and Legal Framework

WCAG is a set of W3C recommendations for making web content accessible, primarily for people with disabilities. Published by the Web Accessibility Initiative (WAI), WCAG has evolved from informal guidelines in 1995 to an internationally recognized standard (ISO/IEC 40500:2012). The current stable version is WCAG 2.2 (October 2023), while WCAG 3.0 remains under development.

## Key Concepts

- **WCAG** stands for Web Content Accessibility Guidelines, published by W3C's Web Accessibility Initiative (WAI).
- **Four Principles (POUR)** organize WCAG 2.x: content must be **Perceivable**, **Operable**, **Understandable**, and **Robust**.
- **Three conformance levels** exist:
  - **Level A** — minimum accessibility; content *must* meet these criteria.
  - **Level AA** — addresses the most common barriers; the level most laws target.
  - **Level AAA** — highest level; not typically required by law due to difficulty satisfying all criteria for all content.
- **Success Criteria** are testable statements (not technology-specific) used to determine conformance. WCAG 2.0 has 61; WCAG 2.1 adds 17 more; WCAG 2.2 adds 9 more (and deprecates 4.1.1 Parsing).
- Each version is **backwards-compatible** — conforming to 2.2 means conforming to 2.1 and 2.0.
- **WCAG 2.0** became ISO/IEC 40500:2012 in October 2012, giving it international standards status.
- **WCAG 1.0** used 14 guidelines with 65 checkpoints organized by three priority levels. It was technology-specific (HTML-focused), unlike the technology-agnostic 2.x approach.
- **WCAG 3.0** (working draft, not yet a recommendation) is under active development with no defined release date.
- W3C publishes **Techniques** documents that are periodically updated; the principles, guidelines, and success criteria themselves are stable once published.

## Commands and Syntax

No CLI commands — WCAG is a specification, not a tool. Key structural references:

- **Criterion numbering**: `Principle.Guideline.SuccessCriterion` (e.g., `1.4.3` = Perceivable > Distinguishable > Contrast (Minimum))
- **Conformance declaration format**: State the WCAG version and level (e.g., "WCAG 2.1 Level AA conformant")
- **Key Level A criteria to know by number**:
  - `1.1.1` Non-text Content (alt text)
  - `2.1.1` Keyboard accessible
  - `2.4.1` Bypass Blocks (skip navigation)
  - `3.1.1` Language of Page
  - `4.1.2` Name, Role, Value
- **Key Level AA criteria**:
  - `1.4.3` Contrast (Minimum) — 4.5:1 for normal text
  - `1.4.11` Non-Text Contrast (2.1)
  - `2.4.7` Focus Visible
  - `3.3.8` Accessible Authentication (2.2)

## Relationships

- **EN 301 549**: European ICT accessibility standard that incorporates WCAG 2.1 Level AA by reference. Required by EU Directive 2016/2102 and the European Accessibility Act (EAA, applicable June 2025).
- **Section 508 (US)**: Updated in 2017 to adopt 17 WCAG 2.0 success criteria for federal ICT.
- **ADA Title II (US)**: DOJ final rule (April 2024) designates WCAG 2.1 Level AA as the technical standard for state/local government web content and mobile apps.
- **ISO/IEC 40500:2012**: The ISO transposition of WCAG 2.0 — identical content, different publication venue.
- **WCAG 3.0**: Intended successor; expected to change the conformance model significantly but is years from recommendation status.
- **WCAG Techniques & Failures**: Companion documents that explain how to satisfy or fail specific success criteria; updated independently of the normative standard.

## Exam-Relevant Points

- **POUR mnemonic**: Perceivable, Operable, Understandable, Robust — the four principles of WCAG 2.x.
- **Conformance levels are cumulative**: AA conformance requires meeting all A and AA criteria; AAA requires all A, AA, and AAA.
- **WCAG 2.0 = ISO/IEC 40500:2012** — know this equivalence.
- **WCAG 2.2 deprecated criterion 4.1.1 (Parsing)** — the only criterion ever removed. Modern HTML parsers handle malformed markup, making it obsolete.
- **New in WCAG 2.2**: Focus Not Obscured (2.4.11/2.4.12), Focus Appearance (2.4.13), Dragging Movements (2.5.7), Target Size Minimum (2.5.8), Consistent Help (3.2.6), Redundant Entry (3.3.7), Accessible Authentication (3.3.8/3.3.9).
- **New in WCAG 2.1**: Orientation (1.3.4), Reflow (1.4.10), Text Spacing (1.4.12), Character Key Shortcuts (2.1.4), Pointer Gestures (2.5.1), Motion Actuation (2.5.4), Status Messages (4.1.3) — many address mobile/touch accessibility gaps.
- **Most laws reference Level AA**, not AAA. AAA is aspirational, not a blanket legal requirement.
- **US law**: Section 508 references WCAG 2.0; ADA Title II final rule (2024) references WCAG 2.1 Level AA.
- **EU law**: Directive 2016/2102 and the European Accessibility Act both reference WCAG 2.1 Level AA. The EAA extends scope beyond public sector to private-sector products/services (effective June 2025).
- **Timeline milestones**: WCAG 1.0 (1999) → WCAG 2.0 (2008) → ISO 40500 (2012) → WCAG 2.1 (2018) → WCAG 2.2 (2023) → WCAG 3.0 (TBD).
- **WCAG 2.x is technology-agnostic** — applies to any web technology, not just HTML. WCAG 1.0 was HTML-specific.
- **The first web accessibility guideline** was published in January 1995 by Gregg Vanderheiden at the Trace Center, University of Wisconsin-Madison.
