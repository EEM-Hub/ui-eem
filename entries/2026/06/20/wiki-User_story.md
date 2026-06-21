---
source: sources/wiki-User_story.md
source_url: https://en.wikipedia.org/wiki/User_story
---

## User Stories in Agile Software Development
User stories are informal, natural language descriptions of software system features, written from the perspective of an end user. They originated in Extreme Programming (XP) and are now central to most agile methodologies. This page covers their history, templates, usage patterns, limitations, and how they relate to larger organizational constructs like epics, themes, and initiatives.

## Key Concepts
- A user story is a **boundary object** that facilitates sensemaking and communication between stakeholders, not a formal specification.
- **Three Cs** (Ron Jeffries, 2001): **Card** (physical token holding the concept), **Conversation** (verbal discussion among stakeholders), **Confirmation** (verifying objectives were met — i.e., acceptance criteria).
- User stories are written by or for users/customers; in Scrum, the **Product Owner** is typically responsible for writing and organizing them into the **product backlog**.
- **Acceptance criteria** define the boundaries of a story and must all be met for a story to be considered done. Formats include Given-When-Then, bullet points, or predecessor criteria.
- Stories are **estimated** using **story points**, often from the Fibonacci sequence (1, 2, 3, 5, 8, 13).
- Stories are intentionally brief and informal — they are "a promise for a conversation" (Alistair Cockburn), not a complete specification.
- No strong evidence that user stories increase software success or developer productivity, but they facilitate **sensemaking without undue problem structuring**, which is linked to success.

## Commands and Syntax

**Connextra Template** (most common):
```
As a <role> I can <capability>, so that <receive benefit>
```
- The "so that" clause is optional (Mike Cohn).

**Feature Injection Template** (Chris Matts — value-first):
```
In order to <receive benefit> as a <role>, I can <goal/desire>
```

**Five Ws Template:**
```
As <who> <when> <where>, I want <what> because <why>
```

**Evil/Abuse User Story** (security-focused):
```
As a <malicious actor>, I want to <attack action> to <damage goal>
```

**Example stories:**
- "As the HR manager, I want to create a screening quiz so that I can understand whether I want to send possible recruits to the functional manager." (epic)
- "As a user, I can indicate folders not to back up so that my backup drive is not filled up with things I do not need to be saved."

## Relationships

- **Hierarchy**: Stories < Epics < Themes < Initiatives (though definitions vary by framework and tool)
  - **Epic**: Large story requiring multiple sprints; groups related stories by ontology/semantics
  - **Theme**: Groups of closely related epics or large stories; also used as cross-cutting labels for tracking
  - **Initiative/Program**: Groups of themes or epics at the highest organizational level
- **Story Maps** (Jeff Patton): Two-dimensional visualization — horizontal axis = product coverage (epics/activities), vertical axis = priority/sophistication. Top row is the "walking skeleton" (minimum viable flow).
- **User Journey Maps**: Focus on a single user persona's chronological experience; map emotions and friction points across phases.
- **vs. Use Cases**: User stories are small, informal, and conversation-starting. Use cases are detailed, structured with numbered steps and extensions, and intended to stand alone. Stories use "As a... I want... so that..." template; use cases use title, main success scenario, and extensions.
- Connected to: **Product Backlog**, **Planning Game** (XP), **Scrum**, **Personas**, **Kanban boards**.

## Exam-Relevant Points
- **Three Cs**: Card, Conversation, Confirmation — know these by name and author (Ron Jeffries).
- The **Connextra template** ("As a... I can... so that...") is the most widely used format; originated at Connextra in London (2001).
- **Mike Cohn's** *User Stories Applied* (2004) is the standard reference; he considers the "so that" clause optional.
- **Kent Beck** introduced user stories in 1997 at the Chrysler C3 project.
- **Acceptance criteria** must all be met for a story to be "done"; can use **Given-When-Then** format.
- **Story points** use the **Fibonacci sequence** for estimation.
- **Limitations** to know: scale-up problems with physical cards, vagueness/incompleteness, lack of non-functional requirements, technical implementation may exceed story scope.
- **Story mapping** provides a two-dimensional view of the backlog (coverage x priority); developed by **Jeff Patton** (2005–2014).
- **Evil user stories** are used for security analysis (thinking like an attacker).
- User stories vs. use cases is a common comparison topic: stories are informal and brief; use cases are formal and detailed with defined steps and extensions.
- In **Jira's hierarchy**: User Story (level 1) → Epic (level 2) → Initiative (level 3), with Themes as cross-cutting labels.
