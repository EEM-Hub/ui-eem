---
source: sources/wiki-Card_sorting.md
source_url: https://en.wikipedia.org/wiki/Card_sorting
---

## Card Sorting as a Knowledge Elicitation Technique

Card sorting is a research method where participants organize items into categories according to given criteria. It is used primarily in user experience design, information architecture, and cognitive psychology to understand how users mentally categorize and structure information within a domain. The technique helps designers build navigation structures, menu hierarchies, and content taxonomies that align with users' mental models.

## Key Concepts

- **Card sorting** is a knowledge elicitation technique — it extracts how people naturally categorize items, revealing their mental models
- Produces **dendrograms** (category trees) or **folksonomies** from participant data
- Useful when no accepted taxonomy exists, when items are hard to categorize clearly, or when audience members differ significantly in how they group items
- Analysis divides into **semantic** methods (analyzing labels and descriptions) and **syntactic** methods (analyzing structure and card placement)
- Semantic sub-methods: **gist analysis** (matching equivalent group labels across participants) and **superordinate analysis** (identifying the overall classification rule a participant used)
- Syntactic sub-methods: **structural** (shape of sorts — number of groups, cards per group) and **item-based** (relationships between individual cards)
- **Similarity/dissimilarity matrices** are distance matrices counting how often card pairs were placed together or apart
- **Edit distance** between two sorts = minimum card moves to transform one into the other (computed via the Hungarian algorithm)
- **Orthogonality** measures how distinct a set of card sorts are from each other, using minimum spanning tree of pairwise edit distances

## Commands and Syntax

No CLI commands; this is a manual/facilitated research method. The basic procedure:

1. Identify key concepts; write each on an index card
2. Have a participant group cards logically and name each group
3. Repeat across multiple participants
4. Analyze results for patterns

**Four variants:**

| Variant | Type | Purpose |
|---|---|---|
| **Open** | Generative | Participants create their own category names — discovers classification patterns |
| **Closed** | Evaluative | Participants sort into predetermined categories — tests category effectiveness |
| **Reverse** (Tree Testing) | Evaluative | Participants navigate an existing hierarchy to complete tasks — tests findability |
| **Modified-Delphi** | Iterative | Each participant refines the previous participant's sort — builds consensus faster |

**Analysis tools:**
- Dissimilarity matrices fed into **hierarchical clustering** to produce dendrograms
- **Multidimensional scaling** (MDS) to produce n-dimensional scatter plots as alternative visualization
- **k-neighbourhoods**: sorts within distance k of a probe sort
- **k-cliques**: k-neighbourhoods where no two sorts exceed distance k from each other
- **Jaccard distance** for computing proportion of differing card pairings between sorts

## Relationships

- **Information architecture**: Card sorting is a foundational method for designing IA structures
- **User experience design**: Primary application domain; used to test and validate design decisions
- **Cognitive psychology**: Card sorting reveals categorization behavior and mental models
- **Cluster analysis / Hierarchical clustering**: Statistical methods used to analyze card sort results
- **Tree testing** (reverse card sorting): The evaluative counterpart that validates structures card sorting helped create
- **Delphi method**: Basis for the Modified-Delphi card sorting variant
- **Q methodology** and **group concept mapping**: Related participatory research methods
- **Taxonomy**: Card sorting is most valuable when no standardized taxonomy exists for the domain

## Exam-Relevant Points

- **Open card sorting is generative** (discovers patterns); **closed card sorting is evaluative** (tests existing categories); **reverse card sorting is evaluative** (tests existing hierarchy)
- Reverse card sorting is synonymous with **tree testing** and isolates structure from visual design
- The **Modified-Delphi** variant is iterative — each participant builds on the previous one's sort, reaching consensus with fewer participants
- **Edit distance** uses the **Hungarian algorithm** for efficient computation
- **Orthogonality** = sum of MST edge weights of pairwise edit distances / number of sorts
- Two analysis paradigms: **semantic** (what participants say) vs. **syntactic** (how they arrange)
- Card sorting should be used when the target audience differs significantly in how they view item groupings — it cannot be determined from first principles
- Remote/online card sorting trades **lower cost and larger reach** for **loss of personal interaction** with participants
- Different evaluation methods for card sorts can produce **different results** — method choice matters
