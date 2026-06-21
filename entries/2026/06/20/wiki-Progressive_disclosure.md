---
source: sources/wiki-Progressive_disclosure.md
source_url: https://en.wikipedia.org/wiki/Progressive_disclosure
---

## Progressive Disclosure (Interaction Design Pattern)

Progressive disclosure is an interaction design pattern that simplifies user interfaces by deferring advanced or rarely-used features to secondary screens and revealing information only when it becomes relevant to the user's current task. The goal is to make applications easier to learn and less error-prone.

## Key Concepts

- **Core principle**: Show only the most common/essential options initially; hide advanced features behind an explicit user action (e.g., "Show Details" button).
- **Purpose**: Reduces cognitive load, lowers the learning curve, and minimizes errors by not overwhelming users with all options at once.
- **Disclosure widget**: A UI control (e.g., expander, toggle, "Show Details" button) that reveals hidden content on demand.
- **Physical-world analogy**: Theme parks hide the full length of waiting lines, showing only small segments at a time to make waits feel more bearable.
- **Classic digital example**: The macOS print dialog, which initially shows a small subset of printing options and reveals advanced settings only when requested.

## Commands and Syntax

No commands or code syntax — this is a design principle, not a technical specification. Implementation involves:
- Placing primary actions/options on the initial screen.
- Providing a clear mechanism (button, link, expander) to reveal secondary options.
- Designing workflows so information appears contextually as the user progresses through a task.

## Relationships

- **Interaction design**: Progressive disclosure is a sub-pattern within the broader field of interaction design.
- **Disclosure widget**: The specific UI component used to implement progressive disclosure (expanders, collapsible sections, "more options" toggles).
- **Chunking (writing)**: Related concept of breaking information into manageable pieces, applied to content rather than UI controls.
- **Apple Human Interface Group**: The seminal idea traces back to Kristina Hooper Woolsey (1985), connecting it to Apple's early HCI research and Donald Norman's *User Centered System Design* (1986).

## Exam-Relevant Points

- Progressive disclosure **defers** advanced features to secondary screens — it does not remove them.
- The pattern serves two goals: **easier learning** and **fewer errors**.
- The concept originates from Kristina Hooper Woolsey's 1985 work at the Apple Human Interface Group.
- Jakob Nielsen (Nielsen Norman Group) is a key authority who documented this pattern.
- Not to be confused with **responsible disclosure** (a security concept).
- The pattern applies beyond digital interfaces — the theme park line example illustrates progressive disclosure in physical environments.
