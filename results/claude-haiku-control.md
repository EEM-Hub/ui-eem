# Exam Results: ui-design-practice.md

**Date:** 2026-06-22 15:07
**Model:** claude:haiku
**Score:** 48/50 (96%)

## Per-Question Results

- **Q1**: CORRECT — What does Fitts's law predict?
- **Q2**: CORRECT — What does Hick's law predict?
- **Q3**: CORRECT — What is Miller's law (7±2)?
- **Q4**: CORRECT — What is progressive disclosure?
- **Q5**: CORRECT — Why is progressive disclosure theoretically grounded?
- **Q6**: CORRECT — What is the Principle of Least Astonishment?
- **Q7**: CORRECT — What is an affordance in UI design?
- **Q8**: CORRECT — What is cognitive load in the context of UI design?
- **Q9**: CORRECT — Which Gestalt principle explains why items near each other are perceived as related?
- **Q10**: CORRECT — What is the semantic difference between a radio button and a checkbox?
- **Q11**: CORRECT — When should you use a slider control?
- **Q12**: CORRECT — What distinguishes a modal window from a non-modal dialog?
- **Q13**: CORRECT — What type of navigation do breadcrumbs provide?
- **Q14**: CORRECT — What is the purpose of a tooltip?
- **Q15**: CORRECT — What is the hamburger button?
- **Q16**: CORRECT — What is ARIA Rule 1?
- **Q17**: CORRECT — What does ARIA change about an element?
- **Q18**: CORRECT — What is the correct treatment of decorative images for accessibility?
- **Q19**: WRONG — What is the semantic HTML accessibility pipeline?
  - Expected: b
  - Got: c
- **Q20**: CORRECT — What ISO standard did WCAG 2.0 achieve?
- **Q21**: WRONG — Why is accessibility a shared responsibility?
  - Expected: b
  - Got: a
- **Q22**: CORRECT — What is responsive web design?
- **Q23**: CORRECT — What is visual hierarchy?
- **Q24**: CORRECT — What role does the typographic grid play in web design?
- **Q25**: CORRECT — What is the relationship between Swiss Style and modern web design?
- **Q26**: CORRECT — What distinguishes a single-page application (SPA) from a traditional web page?
- **Q27**: CORRECT — What are the three install criteria for a Progressive Web App (PWA)?
- **Q28**: CORRECT — How did CSS Flexbox and Grid improve over table-based layouts?
- **Q29**: CORRECT — What is the term coined by Harry Brignull in 2010 for deceptive UI patterns?
- **Q30**: CORRECT — What is confirmshaming?
- **Q31**: CORRECT — What is a roach motel pattern?
- **Q32**: CORRECT — What percentage of EU websites used at least one dark pattern according to a 2022 European Commission report?
- **Q33**: CORRECT — What is Privacy Zuckering?
- **Q34**: CORRECT — What is user-centered design (UCD)?
- **Q35**: CORRECT — What is the purpose of a heuristic evaluation?
- **Q36**: CORRECT — According to Nielsen, how many users are needed to find approximately 85% of usability problems?
- **Q37**: CORRECT — What is card sorting used for?
- **Q38**: CORRECT — What is a design system?
- **Q39**: CORRECT — What design language did Google introduce in 2014?
- **Q40**: CORRECT — What is skeuomorphism in UI design?
- **Q41**: CORRECT — What did Fitts's law contribute to hardware adoption?
- **Q42**: CORRECT — Who coined the term "user experience" and where?
- **Q43**: CORRECT — What catastrophic event informed Don Norman's design principles?
- **Q44**: CORRECT — What are Norman's four design principles?
- **Q45**: CORRECT — What did the Nielsen Norman Group, cofounded in 1998, bring together?
- **Q46**: CORRECT — What is perceived performance?
- **Q47**: CORRECT — What is lazy loading?
- **Q48**: CORRECT — What is above the fold in web design?
- **Q49**: CORRECT — What key event demonstrated that mobile had surpassed desktop as the dominant web platform?
- **Q50**: CORRECT — How did the scrollbar evolve from 1974 to 2007?

## Wrong Answers (Detail)

### Q19: What is the semantic HTML accessibility pipeline?
- a) HTML → JavaScript → CSS → Screen reader
- b) Semantic HTML → ARIA → WCAG → Legal compliance **<--**
- c) HTML → DOM → Render tree → Accessibility tree
- d) Source code → Build step → Deployed page → User
- **Expected:** b
- **Got:** c
- **Objective:** Accessibility

**Model response:**

```
```json
{"answer": "c", "explanation": "The semantic HTML accessibility pipeline describes how browsers process HTML source code into three parallel outputs: the DOM (Document Object Model) tree, the visual render tree for display, and the accessibility tree consumed by assistive technologies like screen readers. Semantic HTML provides the foundation for an accurate and complete accessibility tree, which is the technical pipeline that delivers content to users with disabilities. Options a, b, and d describe related but distinct concepts—rendering order, standards hierarchy, and deployment workflow respectively—rather than the specific technical processing pipeline."}
```
```

### Q21: Why is accessibility a shared responsibility?
- a) Both frontend and backend developers must write accessible code
- b) Applications that do not comply with accessibility APIs remain inaccessible regardless of screen reader quality **<--**
- c) Accessibility requires both automated and manual testing
- d) Both designers and developers must follow WCAG
- **Expected:** b
- **Got:** a
- **Objective:** Accessibility

**Model response:**

```
```json
{"answer": "a", "explanation": "Accessibility is a shared responsibility because it requires contributions across the entire technology stack. Frontend developers must implement accessible HTML, ARIA, and semantic markup; backend developers must ensure data structures, APIs, and services support accessible consumption; and various other roles (designers, QA, product managers) must integrate accessibility throughout their work. No single developer or discipline can create truly accessible applications in isolation—the responsibility is inherently distributed across all technical and non-technical team members who touch the product."}
```
```


## By Objective

- **Accessibility**: 4/6 (66%)
- **Design Principles**: 9/9 (100%)
- **UI Components**: 6/6 (100%)
- **Layout & Visual Design**: 4/4 (100%)
- **Web Concepts**: 5/5 (100%)
- **Ethics & Dark Patterns**: 5/5 (100%)
- **Design Process**: 4/4 (100%)
- **Design Systems**: 3/3 (100%)
- **HCI History**: 6/6 (100%)
- **Performance**: 2/2 (100%)
