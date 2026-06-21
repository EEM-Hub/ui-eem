---
source: sources/wiki-Persona_user_experience.md
source_url: https://en.wikipedia.org/wiki/Persona_(user_experience)
---

## User Personas in UX Design and Marketing

User personas are semi-fictional, archetypal representations of target customer segments or end users, synthesized from real data (interviews, surveys, analytics). Originating in software design through Alan Cooper (1983–1999) and in marketing through Angus Jenkinson's "CustomerPrints" (1993–1994), personas humanize abstract data into relatable profiles that guide design decisions, feature prioritization, and marketing strategy.

## Key Concepts

- **Definition:** A persona is a semi-fictional characterization of a typical customer segment or end user, combining real behavioral data with fictional personal details to create a realistic character.
- **Origin in software:** Alan Cooper began prototyping the persona concept in 1983; popularized it in his 1999 book *The Inmates Are Running the Asylum*.
- **Origin in marketing:** Angus Jenkinson developed "CustomerPrints" (1993–94) at OgilvyOne — "day-in-the-life archetype descriptions" of customer communities sharing brand affinity.
- **Data sources:** Personas are typically synthesized from interviews, surveys, and behavioral data collected from real users.
- **Common persona attributes:** Fictional name, photo, demographics (age, gender, education), biography, goals, technology use, accessibility needs, opinions/beliefs, and a summarizing quote.
- **Four core benefits:**
  - **Shared understanding** — aligns the team on who the user is
  - **Guided design decisions** — prioritizes features against persona needs
  - **Empathy building** — puts a human face on data
  - **Focused design** — prevents self-referential or edge-case-driven design
- **Design pitfalls personas prevent:**
  - **Elastic User** — stakeholders redefining "the user" to suit their argument
  - **Self-referential design** — designers projecting their own mental models
  - **Edge-case focus** — designing for unlikely scenarios instead of common ones
- **Proto-personas vs. personas:** Proto-personas capture a team's *assumptions* about users (generative tool); true personas are *rooted in research data* (evaluative tool). They are not interchangeable.
- **Data-driven (quantitative) personas:** Use clustering, factor analysis, PCA, latent semantic analysis, or non-negative matrix factorization to generate "skeletal" personas from numerical data, addressing criticisms of qualitative methods.
- **Hybrid/mixed-method personas:** Quantitative personas enriched with qualitative insights.

## Commands and Syntax

No CLI commands apply. The "procedure" for creating a persona typically involves:

1. **Gather data** — conduct user interviews, surveys, or analyze behavioral analytics.
2. **Identify patterns** — use segmentation techniques (qualitative coding or quantitative clustering).
3. **Draft persona profiles** — assign name, photo, demographics, goals, frustrations, and a quote.
4. **Validate** — cross-check persona attributes against real user data.
5. **Communicate** — share short-form persona documents with engineering, design, and marketing teams.

For data-driven personas, statistical methods include:
- Cluster analysis
- Factor analysis
- Principal component analysis (PCA)
- Latent semantic analysis (LSA)
- Non-negative matrix factorization (NMF)

## Relationships

- **Market segmentation** — personas are an output of segmentation; they give human form to identified segments.
- **User-centered design (UCD)** — personas are a core artifact in UCD methodology.
- **Interaction design** — personas inform interaction patterns and interface decisions.
- **Use cases / scenarios** — personas drive use case specification; a scenario describes what a persona does.
- **Behavioral targeting & personalized marketing** — personas inform targeting strategies.
- **Brainstorming & feature definition** — personas serve as input to ideation and prioritization.
- **Social sustainability in software** — research (Ayoola et al., 2024) shows personas discourage developers from prioritizing antisocial features.

## Exam-Relevant Points

- **Alan Cooper** coined the user persona concept (prototyped 1983, popularized 1999 in *The Inmates Are Running the Asylum*).
- **Angus Jenkinson** independently developed customer archetypes ("CustomerPrints") for marketing at OgilvyOne in 1993–94.
- Personas prevent three specific pitfalls: **Elastic User**, **self-referential design**, and **edge-case focus**.
- **Criticism:** Personas are not scientifically reproducible (Chapman & Milham); they can be reductive/stereotypical (Portigal); gendered/racial depictions may introduce bias; multi-attribute descriptions may match very few real people.
- **Long (2009) study:** Students using personas produced designs with better usability attributes — but the study had significant methodological limitations (non-blinded, non-random, unreplicated).
- **Data-driven personas** address qualitative shortcomings by using statistical dimensionality-reduction techniques (clustering, PCA, NMF) on numerical user data.
- Proto-personas capture **team assumptions**; true personas are **research-based** — a key distinction likely to be tested.
- Personas are used across HCI, sales, advertising, marketing, and system design — not limited to software.
