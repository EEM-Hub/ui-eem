# UI Design EEM

An External Epistemic Memory (EEM) for **UI Design for Web Software**, built with [expert-agent-builder](https://github.com/benthomasson/expert-agent-builder). Sourced entirely from Wikipedia (CC BY-SA 4.0).

## What's in this repo

| Component | Count | Description |
|-----------|-------|-------------|
| **Sources** | 103 | Wikipedia articles covering UI components, design principles, accessibility, layout, interaction, and web technologies |
| **Entries** | 103 | Structured summaries of each source article |
| **Beliefs** | 830 | Verified design claims with dependency tracking |
| **Network** | 897 | Total belief nodes (830 IN, 67 OUT/retracted) |

## Use Cases

### UI Review Agent
Review web application UIs for adherence to established design principles — Fitts's law, Hick's law, Gestalt grouping, cognitive load management, progressive disclosure. Every finding traces back to Wikipedia source material.

### Accessibility Audit Agent
Evaluate web interfaces against WCAG guidelines, WAI-ARIA patterns, and screen reader compatibility. The belief network captures the relationships between accessibility requirements, assistive technologies, and UI component design.

### Design System Agent
Guide design system construction with knowledge of Material Design, flat design, skeuomorphism, and Bootstrap conventions. The agent understands component taxonomy (buttons, modals, dropdowns, tabs, accordions) and when each pattern applies.

### UX Consultant Agent
Provide evidence-based UX guidance grounded in usability principles from Nielsen, Norman, Cooper, and Shneiderman. The belief network captures design laws, mental model theory, and user-centered design methodology.

### Frontend Architecture Agent
Advise on web application architecture — SPA vs. MPA trade-offs, responsive design strategies, progressive web apps, lazy loading, perceived performance — with beliefs grounded in web platform fundamentals (HTML, CSS, DOM).

## Quick Start

### Prerequisites

Install the CLI tools using [uv](https://docs.astral.sh/uv/):

```bash
# Install the EEM tools
uv tool install ftl-reasons
uv tool install ftl-expert-build

# Install Claude Code (the AI agent runtime)
npm install -g @anthropic-ai/claude-code
```

This installs the CLI tools: `reasons`, `expert-build`, and `entry`.

### Clone and set up

```bash
git clone git@github.com:EEM-Hub/ui-eem.git
cd ui-eem
```

Sources are included in the repo (Wikipedia content, CC BY-SA 4.0).

### Start Claude Code

```bash
cd ui-eem
claude
```

Claude Code automatically reads the `CLAUDE.md` file in this repo, which configures it as a UI design EEM with access to the belief registry, entries, and knowledge tools.

### Query the EEM

Once inside Claude Code, you can:

```
# Search the knowledge base
> reasons search "responsive design breakpoints"

# Look up a specific belief
> reasons show fitts-law-target-size

# Trace why a belief holds
> reasons explain progressive-disclosure-reduces-cognitive-load

# Check pipeline status
> expert-build status
```

## Extending the EEM

### Add new sources

Add markdown documents to `sources/`, then run:

```bash
expert-build summarize
expert-build propose-beliefs
expert-build accept-beliefs
```

### Derive new beliefs from existing ones

```bash
expert-build derive-review-repair
```

### Export the network

```bash
reasons export -o network.json
reasons export-markdown -o beliefs.md
```

## Architecture

```
sources/          Wikipedia articles (fetched, CC BY-SA 4.0)
    |
    v
entries/          Structured summaries (LLM-generated)
    |
    v
reasons.db        Belief network with dependency tracking
    |
    v
beliefs.md        Markdown export of all beliefs
network.json      JSON export of the full network
```

The pipeline flows from Wikipedia articles through summarization and belief extraction to a queryable knowledge base. Each belief traces back to its source article. Derived beliefs track their justification chains — `reasons explain <id>` shows the full derivation path. The derive-review-repair cycle grew the network from 615 premises to 830 active beliefs across 23 derivation depths.

## Belief Network Statistics

| Metric | Value |
|--------|-------|
| Total nodes | 897 |
| IN (active) | 830 |
| OUT (retracted) | 67 |
| Premises | 615 |
| Derived | 282 |
| Max depth | 23 |
| Sources | 103 Wikipedia articles |

## License

All source content is from [Wikipedia](https://en.wikipedia.org) and licensed under [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/) / [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). This repository and all derived content is distributed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). See [attribution.md](attribution.md) for the full list of source articles.
