---
source: sources/wiki-Principle_of_least_astonishment.md
source_url: https://en.wikipedia.org/wiki/Principle_of_least_astonishment
---

## Principle of Least Astonishment (POLA)

The Principle of Least Astonishment (POLA), also called the Principle of Least Surprise (POLS), is a fundamental design guideline in user interface and software design stating that a system component should behave the way most users expect it to behave. Originating in the late 1960s in response to confusing behavior in the PL/I programming language, it was first formally published in 1972 and remains a cornerstone of good software and API design.

## Key Concepts

- **Core principle**: Every component should behave exactly as its syntax and appearance suggest; users should never be surprised by system behavior.
- **Corollary**: "If a necessary feature has a high astonishment factor, it may be necessary to redesign the feature." (Cowlishaw, 1984)
- **Textbook formulation**: "People are part of the system. The design should match the user's experience, expectations, and mental models." (Saltzer & Kaashoek, 2009)
- **Audience-dependent**: What counts as "least surprising" varies by audience — end users, programmers, and system administrators may have different expectations.
- **Leverages existing knowledge**: Designs should borrow from functionally similar programs users already know, minimizing the learning curve.
- **Sensible defaults**: Part of POLA involves choosing default values and behaviors that align with common expectations.
- **Conflict resolution**: When two interface elements conflict or are ambiguous, prefer the behavior that surprises the user least — not the behavior that feels natural from knowing the system's internals.

## Commands and Syntax

No specific commands, but illustrative examples of violations and adherence:

- **PL/I violation**: `25 + 1/3` yielded `5.33...` instead of `25.33...` due to precision conversion rules — a canonical POLA failure.
- **JavaScript violation**: `parseInt("010")` originally defaulted to octal (base 8), returning `8` instead of the expected `10`. Fixed in ECMAScript 5 to default to base 10.
- **Convention: keyboard shortcuts**: F1 for help (Windows/Linux), `Cmd+Shift+/` for help (macOS), `?` for shortcut discovery in web apps (Gmail, YouTube, Jira). Repurposing these keys for other functions violates POLA.
- **API design**: Function/method names should intuitively match their behavior (e.g., `ParseInteger(string, radix)` with radix defaulting to 10).

## Relationships

- **DWIM (Do What I Mean)**: Complementary principle — the system should interpret ambiguous input the way the user intended.
- **Convention over Configuration**: Related philosophy where defaults follow established conventions, reducing surprise.
- **Human Interface Guidelines**: Platform-specific codifications of POLA (e.g., Windows keyboard shortcut conventions, Unix CLI switch conventions).
- **Mental Models**: POLA is grounded in cognitive science — designs must align with users' mental models of how systems work.
- **Look and Feel / WYSIWYG**: Visual consistency principles that support POLA by ensuring what users see matches what they get.
- **User Experience Design**: POLA is a foundational UX principle that influences interaction patterns, information architecture, and workflow design.

## Exam-Relevant Points

- **Acronyms**: POLA (Principle of Least Astonishment) and POLS (Principle of Least Surprise) are interchangeable.
- **Origin**: First referenced in the PL/I Bulletin in 1967; first appeared in print formally in 1972.
- **PL/I is the canonical negative example**: Its precision conversion rules made `25 + 1/3` produce incorrect results, violating POLA.
- **JavaScript parseInt is a modern example**: Pre-ECMAScript 5, strings starting with "0" were parsed as octal by default — a well-known POLA violation.
- **The principle applies beyond software**: It extends to writing (hyperlink text should describe the destination), documentation, and any system where users form expectations.
- **Audience matters**: Designing for least surprise requires understanding *whose* expectations to meet (end user vs. developer vs. admin).
- **FreeBSD explicitly uses POLA** as a documented guideline for user experience decisions.
- **High astonishment factor rule**: If a feature is necessary but surprising, the correct response is to redesign the feature, not to document the surprise.
