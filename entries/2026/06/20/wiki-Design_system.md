---
source: sources/wiki-Design_system.md
source_url: https://en.wikipedia.org/wiki/Design_system
---

## Design Systems in UI Development

A design system is a comprehensive framework of standards, reusable components, and documentation that guides consistent development of digital products within an organization. It serves as a single source of truth for designers and developers, encompassing pattern libraries, style guides, design languages, coded components, brand languages, and documentation. This page covers the definition, advantages, historical origins, distinction from related concepts (pattern languages, UI kits), and the emerging concept of design tokens.

## Key Concepts

- **Design system** — a unified framework containing component libraries, style guides (font, color, spacing, dimensions, placement), design languages, coded components, brand guidelines, and documentation
- **Purpose** — establishes common understanding between design, engineering, and product teams to ensure consistent user experience
- **Design tokens** — named variables storing specific design attributes (color, typography, spacing); serve as single source of truth for design decisions expressed in code
- **Pattern language** — allows patterns to exist in many shapes/forms (e.g., a login form is a pattern regardless of button color); patterns share a configuration (relationship) while differing in exact appearance
- **Design language** — always includes specific visual guidelines with defined colors and typography (more prescriptive than a pattern language)
- **UI kit** — simply a set of UI components with no explicit usage rules (least structured of the three)
- **Atomic Design** — a methodology (Brad Frost, 2016) for designing digital products in a component-based way; helped popularize the term "design system"
- **BEM** — a systematic CSS methodology from the 2010s addressing large-scale web project challenges

## Commands and Syntax

No CLI commands or code syntax are defined in this topic. The key "syntax" is the structure of **design tokens**:

- A design token is a **named variable** that stores a design attribute
- Example conceptual structure: `color-primary: #0052CC`, `spacing-medium: 16px`, `font-body: 'Inter', sans-serif`
- The **W3C Design Tokens Community Group** is developing open standards for token format and interoperability

## Relationships

- **Notable implementations**: Material Design (Google), Lightning Design System (Salesforce), Carbon Design System (IBM), Fluent Design System (Microsoft), Adobe Spectrum, Atlassian Design System, Amazon Style Dictionary
- **Historical lineage**: Christopher Alexander's "A Pattern Language" (1977) → Software Design Patterns (1980s) → first wiki (WikiWikiWeb) → Yahoo! Design Pattern Library (2006) + YUI Library → Google Material Design (2014, first called a "design language") → Atomic Design book (2016, popularized "design system")
- **Connects to**: User interface design, user experience design, digital product design, brand design, software design patterns, web design
- **Standardization**: W3C Design Tokens Community Group working on open standards

## Exam-Relevant Points

- A design system is **not** the same as a UI kit (UI kit = components only, no rules) or a pattern language (pattern language = abstract configurations, no specific visual guidelines)
- **Design tokens** provide abstraction, flexibility, scalability, and consistency; they are "design decisions expressed in code"
- Christopher Alexander's "A Pattern Language" (1977) is the foundational origin of design systems thinking
- The term "design system" was popularized by Brad Frost's **Atomic Design** book in **2016**
- Google's **Material Design (2014)** was the first system its creator called a "design language"
- Yahoo! Design Pattern Library (**2006**) reignited mainstream interest in UI pattern languages
- The simultaneous release of Yahoo!'s pattern library and YUI component library was intentional — patterns + components together enable more systematic design than components alone
- Key advantages: streamlined workflows, unified cross-team language, faster builds via reuse, reduced design/technical debt, improved scalability
- Design systems require proper implementation and maintenance — poorly maintained systems become disorganized and reduce efficiency
