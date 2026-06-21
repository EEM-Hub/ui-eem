---
source: sources/wiki-Usability_testing.md
source_url: https://en.wikipedia.org/wiki/Usability_testing
---

## Usability Testing: Methods, Participants, and Limitations

Usability testing is a user-centered interaction design technique that evaluates a product by observing real users attempting to use it for its intended purpose. Unlike usability inspection (expert-only) or market research (opinion gathering), usability testing involves systematic observation under controlled conditions. It originated in 1940s studies of machine use (e.g., WWII airplane controls), became standard practice with the rise of HCI in the 1980s, and expanded to web and mobile platforms through the 2000s–2010s.

## Key Concepts

- **Definition**: Measuring a product's capacity to meet its intended purpose by observing real users performing tasks — not gathering opinions.
- **Distinction from market/qualitative research**: Usability testing requires watching people *use* the product, not asking if they understand it.
- **Usability vs. HCI**: Usability testing measures ease of use of a specific product; HCI studies formulate universal principles.
- **Usability labs**: Dedicated spaces with controlled environments (desk, chair, computer, test-specific equipment) for conducting tests, as opposed to field or remote testing.
- **Think aloud protocol**: Participants verbalize thoughts while performing tasks — a primary data-gathering technique.
- **Co-discovery learning**: Pairs of users work together, revealing interaction insights.
- **Eye tracking**: Captures where users look during tasks.
- **Curb-cut effect**: Designing for users with disabilities (extreme/edge users) often improves usability for all users.
- **WEIRD sampling bias**: Over-reliance on Western, Educated, Industrialised, Rich, Democratic participants (12% of global population = 96% of behavioral research participants), limiting generalizability.

## Commands and Syntax

No CLI commands. Key procedural frameworks:

**Standard usability test process:**
1. Create a realistic scenario with specific tasks
2. Recruit representative participants
3. Observe users performing tasks (record clicks, time, body language, errors)
4. Analyze data and iterate on design

**Nielsen/Landauer problem discovery formula:**
```
U = 1 - (1 - p)^n
```
- `U` = proportion of usability problems uncovered
- `p` = probability one participant finds a specific problem
- `n` = number of participants/sessions

**Nielsen's 10 Usability Heuristics (for expert/heuristic evaluation):**
1. Visibility of system status
2. Match between system and real world
3. User control and freedom
4. Consistency and standards
5. Error prevention
6. Recognition rather than recall
7. Flexibility and efficiency of use
8. Aesthetic and minimalist design
9. Help users recognize, diagnose, and recover from errors
10. Help and documentation

## Relationships

- **User-centered design / Interaction design**: Usability testing is a core technique within these disciplines.
- **Usability inspection**: The expert-only counterpart (no real users); includes heuristic evaluation.
- **Heuristic evaluation**: An expert review method using Nielsen's 10 heuristics — complements but does not replace user testing.
- **A/B testing**: Quantitative method comparing two versions; commonly used alongside usability testing in web development.
- **Accessibility testing**: Testing with users with disabilities; distinct from but overlapping with usability testing — compliance with accessibility guidelines alone does not guarantee usability.
- **Cognitive pretesting / Pilot testing**: Complementary pretesting methods in survey research.
- **Qualitative research / Market research**: Gathers opinions/motivations; often combined with usability testing but is not usability testing itself.

## Exam-Relevant Points

- **Five users is enough (Nielsen)**: Five users per iterative round (not total) uncover ~85% of problems on average — but the range varies from 55%–100%, and the model assumes uniform detection probability, which critics dispute.
- **Iterative testing over large single tests**: Nielsen advocates many small tests (3–5 users, weekly) over one large test. Total participants across a project typically reach 50–100.
- **Guerrilla/hallway testing**: Quick, cheap, informal testing in public spaces; uses convenience sampling (potentially biased); best for early-stage design to catch obvious problems.
- **Remote testing types**: Synchronous (moderated, real-time via video/screen sharing) vs. asynchronous (unmoderated, auto-logged clicks/time/pages). Asynchronous allows larger sample sizes and natural environments.
- **Expert review vs. user testing**: Expert review uses trained evaluators applying heuristics; user testing uses actual users. Both are needed — they catch different categories of issues.
- **Automated expert review**: Programs apply design rules/heuristics; faster and more consistent than human reviewers but less detailed.
- **Disability inclusion**: ~16% of global population has significant disability; testing with disabled users identifies more issues (including issues affecting all users) than testing with non-disabled users alone.
- **A/B testing**: Compares two variants (A vs. B) differing in one element; multivariate/bucket testing compares more than two versions simultaneously.
- **Body language observation** (Apple 1982 example): 95% of stumbling blocks found by watching body language — users often won't report confusion, assuming the fault is their own.
