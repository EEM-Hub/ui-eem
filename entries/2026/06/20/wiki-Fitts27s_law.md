---
source: sources/wiki-Fitts27s_law.md
source_url: https://en.wikipedia.org/wiki/Fitts%27s_law
---

## Fitts's Law: Predictive Model of Human Pointing Movement

Fitts's law is a foundational predictive model in human–computer interaction (HCI) and ergonomics that quantifies the time required to move to and select a target as a function of the target's distance and size. Originally proposed by Paul Fitts in 1954, it models pointing tasks — both physical (touching objects) and virtual (clicking with a mouse) — and has been validated across diverse limbs, input devices, environments, and populations.

## Key Concepts

- **Index of Difficulty (ID):** Quantifies task difficulty in bits using the ratio of distance (D) to target width (W), based on an information-theoretic analogy where D is signal and W is noise.
- **Index of Performance / Throughput (IP/TP):** Measures human motor performance in bits per second; computed as ID divided by movement time (MT).
- **Two movement phases:** A pointing movement consists of (1) a fast, imprecise initial ballistic movement toward the target, and (2) a slower, precise corrective movement to acquire the target.
- **Distance vs. width impact:** Distance has a greater effect on overall task completion time than target size, even when two tasks have the same ID.
- **Speed-accuracy tradeoff:** Aggressive users can reduce MT at the cost of higher error rates; the effective target width (We) adjustment captures this tradeoff.
- **Effective target width (We):** Replaces nominal W with a value computed from the standard deviation of actual selection coordinates (We = 4.133 × SDx), spanning 96% of the distribution. If error rate equals 4%, We = W.
- **Eye tracking controversy:** Fitts's law does not straightforwardly apply to saccadic eye movements because users are blind during fast saccades, unlike conscious target acquisition in standard pointing.
- **Temporal pointing:** Extension where targets are defined on the time axis (e.g., blinking targets), with temporal distance (Dt) and temporal width (Wt) replacing spatial parameters.

## Commands and Syntax

**Original Fitts Formulation (1954):**
- ID = log₂(2D / W)
- MT = a + b · log₂(2D / W)
  - *a* = y-intercept (delay constant), *b* = slope (acceleration), determined empirically via regression
  - D = distance to target center, W = target width along axis of motion

**Shannon Formulation (MacKenzie, most widely used in HCI):**
- ID = log₂(D/W + 1)
- Adopted in ISO 9241-9 as the standard for interface evaluation

**Effective Width Adjustment (Crossman, 1956):**
- We = 4.133 × SDx (from actual selection coordinate distributions)
- IDe = log₂(D/We + 1)
- IP = IDe / MT

**Welford's Two-Factor Model (1968):**
- MT = a + b₁·log₂(D) + b₂·log₂(W)
- Separates distance and width into independent terms for improved prediction

**Shannon-Welford with Angle Parameter (Kopper et al., 2010):**
- MT = a + b·log₂((D + W) / W^k)
- k parameter accounts for angular direction; reduces to Shannon form when k = 1
- Directly comparable to Shannon form via F-test of nested models

**Temporal Pointing Model:**
- IDt = log₂(Dt / Wt)
- Predicts error rate as a function of temporal index of difficulty

## Relationships

- **Information theory:** Fitts's law draws an analogy from the Shannon-Hartley theorem (signal/noise ratio maps to distance/width ratio), though no formal mathematical connection has been established.
- **Hick's law:** Companion model in HCI that predicts decision time based on number of choices (often paired with Fitts's law in interface design analysis).
- **Accot-Zhai steering law:** Derived from Fitts's law for constrained trajectory tasks (e.g., navigating hierarchical pull-down menus).
- **ISO 9241-9:** International standard for evaluating pointing devices that codifies the Shannon formulation and throughput calculation using effective width.
- **Input device comparison:** Card, English, and Burr (1978) used Fitts's law to compare mouse, joystick, and step keys — results favoring the mouse contributed to its commercial adoption by Xerox.
- **2D extensions:** Multiple models exist for extending 1D Fitts's law to 2D targets (status quo/horizontal width, sum model, area model, smaller-of model, W-model, angle-specific convolution).

## Exam-Relevant Points

- **The three formulations and when each applies:** Original (log₂(2D/W)), Shannon (log₂(D/W + 1), preferred in HCI/ISO), Welford (separate D and W terms, better prediction).
- **Parameters a and b** are determined empirically via regression; *b* (or 1/b as throughput) is used to compare input devices.
- **We = 4.133 × SDx** is the effective target width formula; if error rate = 4%, We = W exactly.
- **Movement has two phases:** fast ballistic + slow corrective. Distance dominates overall completion time.
- **UI design principles derived from Fitts's law:**
  - Make targets as large as possible (optimize W).
  - Cluster related functions to minimize travel distance (optimize D).
  - **Infinite edges rule:** Targets on screen edges are effectively infinite in one dimension (e.g., macOS menu bar at top edge).
  - **Magic corners:** Screen corners are effectively infinite in two dimensions (e.g., Windows Start button, Office menu button).
  - **Magic/prime pixel:** Context menus at cursor position eliminate D entirely.
  - Radial menus equalize distance but directional difficulty varies (right-most items easiest for right-handed users).
- **Model limitation:** Predictive power degrades when both D and W are varied simultaneously over a wide range, because ID depends only on their ratio (implies arbitrary rescaling doesn't affect MT, which is false).
- **Shannon-Welford with k parameter** is empirically the best model for virtual pointing tasks; it is more robust when control-display gain varies.
- **Temporal pointing** extends the model to time-domain targets (blinking/moving targets), first presented to HCI in 2016.
