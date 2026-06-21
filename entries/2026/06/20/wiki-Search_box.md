---
source: sources/wiki-Search_box.md
source_url: https://en.wikipedia.org/wiki/Search_box
---

## Search Box (UI Control Element)

A search box (also called search field or search bar) is a graphical control element used in software applications and websites that accepts user input for querying a database. It is typically a single-line text box or expandable search icon dedicated to search functionality. On websites, search boxes submit queries to server-side scripts that check a search engine index for matching entries.

## Key Concepts

- **Definition**: A graphical control element — specifically a single-line text box — dedicated to accepting search queries
- **Search button**: Often accompanies the search box (sometimes shown as a magnifying glass icon), but may be omitted if Enter key or automatic real-time search is supported
- **Site search**: The broader functionality that the search box enables; critical for content-rich websites
- **E-commerce usage**: Search boxes serve as a primary navigation tool on e-commerce sites, not just a secondary feature
- **Real-time results**: Some implementations update results as the user types (incremental search), but this increases load and may cause browser crashes on smaller sites
- **Classification**: Falls under the "Data input-output" category of graphical control elements, alongside checkboxes, sliders, text boxes, combo boxes, etc.

## Commands and Syntax

No specific commands or configuration syntax — this is a UI pattern rather than a technical specification. Key implementation considerations:

- **Autocomplete / search suggestions**: Often implemented via dropdown lists showing past searches or predicted queries
- **Spelling checker integration**: Can be built into the search box to correct user input
- **Scope restriction**: Drop-down menus or additional controls can let users filter what type of content to search
- **Persistent connections (e.g., WebSocket)**: Used in modern implementations for low-latency autocomplete; a single WebSocket server instance has been benchmarked handling 240,000 autocomplete requests/sec from 1 million concurrent users at ~12ms round-trip latency

## Relationships

- **Parent category**: Graphical control elements (alongside buttons, sliders, checkboxes, text boxes)
- **Related elements**: Text box (search box is a specialized form), drop-down list (for suggestions), search suggest drop-down list
- **Depends on**: Web search engine indexing (server-side), incremental search (for real-time results)
- **Part of**: Site search systems, web navigation patterns
- **Technology connections**: WebSocket for persistent connections, server-side scripting for query processing

## Exam-Relevant Points

- A search box is classified as a **data input-output** graphical control element
- The search button can be **omitted** when Enter key submission or automatic real-time search is available
- Real-time search result updating is **not recommended for small/medium websites** due to performance concerns (slow loading, unresponsiveness, browser crashes)
- Modern implementations use **persistent connections** (e.g., WebSocket) for low-latency search and bandwidth efficiency
- Search boxes are a **primary navigation tool** in e-commerce, not merely supplementary
- Common companion features: autocomplete, search suggestions, spelling correction, scope-restriction controls
