---
source: sources/wiki-Dark_pattern.md
source_url: https://en.wikipedia.org/wiki/Dark_pattern
---

## Dark Patterns (Deceptive Design Patterns) in User Interfaces

Dark patterns are user interface designs deliberately crafted to manipulate users into unintended actions — such as making unwanted purchases, sharing excessive personal data, or subscribing to recurring charges. The term was coined by UX designer Harry Brignull in 2010, and the field has since become a major focus of regulatory enforcement in the US, EU, and UK.

## Key Concepts

- **Dark pattern** — a UI deliberately designed to trick users into actions they did not intend (purchases, subscriptions, data sharing)
- **Bait-and-switch** — advertising a free/cheap product, then steering users to expensive alternatives when the advertised product is "unavailable"
- **Drip pricing** — showing a low headline price, then incrementally revealing additional fees/taxes during checkout
- **Confirmshaming** — wording decline options to shame users into accepting (e.g., "No thanks, I don't want to save money")
- **Misdirection** — using prominent buttons or confusing wording (including double negatives) to trick users into accepting unwanted terms or installing unrelated software
- **Privacy Zuckering** — tricking users into sharing more personal information than intended, named after Mark Zuckerberg; includes obscured opt-out processes
- **Roach motel (trammel net)** — easy to sign up, deliberately difficult to cancel or opt out (e.g., requiring printed mail to cancel)
- A 2019 study of 11,000 shopping sites found **1,818 dark patterns** grouped into **15 categories**
- A 2022 European Commission report found **97% of the most popular websites/apps used by EU consumers deployed at least one dark pattern**

## Commands and Syntax

Not applicable — this is a regulatory/design concept topic, not a technical configuration domain. However, key regulatory instruments function as "rules" in this space:

- **CCPA opt-out test**: Does the interface have "the substantial effect of subverting or impairing a consumer's choice to opt-out"? If yes, it violates California law.
- **GDPR consent test**: Is consent "unambiguous, freely-given, and specific to each usage"? Dark patterns that bundle consent or use confusing defaults violate GDPR.
- **EDPB assessment starting point**: Article 5(1)(a) GDPR — the principle of fair processing is used to evaluate whether a design constitutes a dark pattern.

## Relationships

- **GDPR / Data Protection** — Dark patterns directly violate GDPR consent requirements; the European Data Protection Board uses Article 5(1)(a) fair processing principle as the assessment baseline
- **CCPA (California Consumer Privacy Act)** — Explicitly prohibits dark patterns that subvert opt-out choices; amended in March 2021
- **FTC enforcement** — The US Federal Trade Commission actively pursues dark pattern cases (Intuit/TurboTax $141M settlement; Epic Games/Fortnite $245M fine)
- **EU Digital Services Act / Data Act** — Two of three EU laws that expressly address dark patterns
- **AI model training** — Meta's 2024 attempt to use Facebook/Instagram data for AI training used dark patterns in the opt-out process, leading to NOYB complaints in 11 EU countries
- **Nudge theory** — Dark patterns are the adversarial application of behavioral nudge principles
- **Enshittification** — Dark patterns are a mechanism through which platform quality degrades over time
- **Advertising networks** — SDK documentation often ships with privacy-unfriendly defaults that nudge developers toward dark patterns

## Exam-Relevant Points

- **Harry Brignull** coined the term "dark pattern" on **28 July 2010** via darkpatterns.org (now deceptive.design)
- **Bait-and-switch is a form of fraud** that violates existing US law (16 CFR 238)
- The **DETOUR Act** (introduced April 2019 by Senators Fischer and Warner) targets companies with **100M+ monthly active users**
- **FTC v. Intuit**: $141M settlement (May 2022) for deceptive "free" TurboTax advertising; FTC ordered fix in January 2024; Intuit stopped free service as of March 2024
- **FTC v. Epic Games**: $245M fine (March 2023) — **largest FTC refund in a gaming case**
- **EU standard**: GDPR requires consent that is **unambiguous, freely-given, and specific** — dark patterns violate this
- **Three EU laws** expressly address dark patterns: **Data Act**, **Digital Services Act**, and the **directive on financial services contracts concluded at a distance**
- **UK Age-Appropriate Design Code** (Children's Code): Took effect **2 September 2020**, prohibits "nudges" toward low-privacy settings for minors, enforceable under Data Protection Act 2018
- **97%** of top EU websites/apps deploy at least one dark pattern (2022 European Commission finding)
- **Norwegian Consumer Council** published "Deceived by Design" (2018) examining Facebook, Google, and Microsoft
- **EFF and Consumer Reports** launched a dark patterns tip line in **2021**
- **Fareportal**: Fined $2.6M by New York AG (2022); **Trivago**: Fined A$44.7M by Australian Federal Court (2022)
