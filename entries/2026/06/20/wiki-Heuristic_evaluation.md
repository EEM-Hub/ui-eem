---
source: sources/wiki-Heuristic_evaluation.md
source_url: https://en.wikipedia.org/wiki/Heuristic_evaluation
---

## Heuristic Evaluation: Usability Inspection Method

Heuristic evaluation is a usability inspection method where expert evaluators examine a user interface and judge its compliance with recognized usability principles ("heuristics"). Developed by Rolf Molich and Jakob Nielsen, it is one of the most informal and cost-effective methods in human-computer interaction for identifying UI design problems. It does not require end users, making it practical for early-stage design on limited budgets. However, results are highly dependent on the expertise of the reviewers, and the method produces qualitative observations rather than hard data.

## Key Concepts

- **Definition**: Evaluators examine an interface against established usability principles to identify design problems, often within the context of use cases (typical user tasks).
- **Optimal evaluator count**: 3-5 evaluators recommended; more than five adds cost without proportional benefit.
- **Individual-first process**: Evaluators must work independently before group discussion to reduce confirmation bias.
- **Observer trade-off**: Sessions without observers require written reports (more evaluator effort, lower cost); sessions with observers allow verbal analysis with transcription (less evaluator effort, higher cost).
- **Severity rating**: Usability problems found are typically categorized on a numeric scale by estimated impact on user performance or acceptance.
- **Limitation**: Results are influenced by reviewer expertise; heuristic evaluation and performance testing uncover different problem sets, so neither alone is sufficient.
- **No hard data**: Findings are expert observations, not empirical measurements — a key distinction from user-based testing.
- **Domain/culture gap**: General heuristics may miss domain-specific or culture-specific usability issues, prompting the development of specialized heuristic sets.

## Commands and Syntax

No commands or code syntax apply. The method is procedural:

1. **Select 3-5 evaluators** with usability expertise.
2. **Each evaluator independently** examines the interface against a chosen heuristic set.
3. **Evaluators rate severity** of each identified problem (typically on a numeric scale).
4. **Aggregate findings** in a group session after individual reviews are complete.
5. **Compile report** of unique problems with severity ratings and heuristic violations cited.

## Relationships

- **Parent method**: Usability inspection (heuristic evaluation is one type).
- **Complements**: User-based testing and software performance testing — each uncovers different problem categories; heuristic evaluation is often used *before* user testing to eliminate obvious issues.
- **Related frameworks**: Cognitive walkthrough (another inspection method), cognitive dimensions (evaluation framework for notations and UIs), progressive disclosure (related to minimalist design heuristic).
- **Foundational field**: Human-computer interaction (HCI) and usability engineering.

## Exam-Relevant Points

- **Nielsen's 10 Heuristics** (know all by name and definition):
  1. Visibility of system status
  2. Match between system and the real world
  3. User control and freedom (undo/redo, "emergency exit")
  4. Consistency and standards
  5. Error prevention (eliminate error-prone conditions or confirm before commit)
  6. Recognition rather than recall (minimize memory load)
  7. Flexibility and efficiency of use (accelerators for experts)
  8. Aesthetic and minimalist design (no irrelevant information)
  9. Help users recognize, diagnose, and recover from errors (plain language, constructive suggestions)
  10. Help and documentation (searchable, task-focused, concrete steps)

- **Gerhardt-Powals' 10 Cognitive Engineering Principles**: Focus on reducing cognitive load — automate unwanted workload, reduce uncertainty, fuse data, use meaningful names, group data consistently, limit data-driven tasks, show only needed info, multiple data codings, judicious redundancy.

- **Shneiderman's 8 Golden Rules**: Consistency, shortcuts for frequent users, informative feedback, dialog closure, simple error handling, easy reversal, internal locus of control, reduce short-term memory load.

- **Weinschenk & Barker Classification**: 20 categories consolidating heuristics from multiple providers — covers user control, human limitations, modal integrity, accommodation, linguistic clarity, aesthetic integrity, simplicity, predictability, interpretation, accuracy, technical clarity, flexibility, fulfillment, cultural propriety, suitable tempo, consistency, user support, precision, forgiveness, responsiveness.

- **3-5 evaluators** is the recommended number (Nielsen); individual evaluators are "mostly quite bad" alone.
- **Individual before group** to avoid confirmation bias.
- Heuristic evaluation produces **qualitative findings, not empirical data**.
- General heuristics have **limitations for domain-specific and culture-specific applications**.
