---
source: sources/wiki-Hick27s_law.md
source_url: https://en.wikipedia.org/wiki/Hick%27s_law
---

## Hick's Law: Logarithmic Relationship Between Choice Count and Decision Time

Hick's law (also Hick–Hyman law) is a principle from experimental psychology stating that the time a person takes to make a decision increases logarithmically with the number of available choices. Named after W. E. Hick (1952) and Ray Hyman (1953), the law connects human decision-making to information theory. The key practical implication: doubling the number of choices does *not* double decision time — the marginal cost of each additional option decreases as options increase.

## Key Concepts

- **Logarithmic relationship**: Decision time grows as log2 of the number of choices, not linearly. People implicitly perform a binary-search-like subdivision of options, eliminating roughly half the remaining choices at each cognitive step.
- **Rate of gain of information**: The amount of time taken to process a certain number of bits; this is the core metric the law quantifies.
- **Historical lineage**: Donders (1868) first reported the relationship between multiple stimuli and reaction time. Merkel (1885) showed response time increases with set size. Hick (1952) formalized the logarithmic model; Hyman (1953) extended it to unequal probabilities.
- **Information-theoretic entropy (H)**: When choices have unequal probabilities, H replaces log2(n+1) in the formula, weighting each alternative by its probability.
- **Stimulus–response compatibility**: Decision time is also affected by how naturally the response maps to the stimulus (e.g., turning a wheel to steer). Compatible mappings reduce reaction time.
- **IQ correlation (Roth, 1964)**: Information processing speed (reciprocal of the slope in the Hick function) correlates with IQ — faster processing speed corresponds to higher IQ scores.

## Commands and Syntax

**Equal-probability formula:**

```
T = b * log2(n + 1)
```
- `T` = average reaction time
- `b` = empirically fitted constant (slope)
- `n` = number of equally probable choices
- The `+1` accounts for uncertainty about whether to respond at all

**Unequal-probability (generalized) formula:**

```
T = b * H

where H = Σ pi * log2(1/pi + 1)
```
- `H` = information-theoretic entropy of the decision
- `pi` = probability of the i-th alternative

**IQ-related formulation (Roth):**

```
Reaction Time = Movement Time + log2(n) / Processing Speed
```

## Relationships

- **Fitts's Law**: Similar logarithmic form but governs motor movement (time to reach a target based on distance and size). Hick's law governs the *cognitive decision* phase; Fitts's law governs the *motor execution* phase. Together they model the full choice-and-act cycle in HCI.
- **Information Theory (Shannon)**: The entropy measure H directly borrows from Shannon's information theory. The law treats human cognition as an information channel with measurable capacity.
- **Power Law of Practice**: Related principle about how task performance improves with repetition.
- **The Paradox of Choice**: Broader behavioral concept that more options can reduce satisfaction — Hick's law provides the quantitative, reaction-time dimension of this problem.
- **Menu Design / HCI**: Frequently cited in interface design — but applies only when users can subdivide options (e.g., alphabetically sorted menus), not when linear scanning is required (e.g., random-order lists).

## Exam-Relevant Points

- The formula uses **log base 2**, reflecting binary subdivision of the choice space.
- The **+1 in log2(n+1)** accounts for the go/no-go uncertainty (whether to respond at all), not just which response to make.
- Hick's law does **not** apply to linear search tasks (e.g., scanning a randomly ordered word list — that's linear time, not logarithmic).
- **Exceptions exist**: Verbal responses to familiar stimuli show no increase or only subtle increases with more options. Saccadic eye movements can show an *anti-Hick's effect* (faster with more alternatives).
- The relationship between predictability and reaction time in structured sequences is **sigmoid, not linear** — a more recent finding (Pavao et al., 2016) that challenges naive generalization of Hick's law.
- For **unequal probabilities**, you must use the entropy-based generalization (H), not the simple log2(n+1) form.
- Hick's law justifies **hierarchical/categorized menu structures** over flat lists — subdividing mirrors the cognitive strategy the law describes.
- The law measures **cognitive information capacity** in choice reaction experiments, bridging psychology and information theory.
