---
source: sources/wiki-Pagination.md
source_url: https://en.wikipedia.org/wiki/Pagination
---

## Pagination: Dividing Content into Discrete Pages

Pagination (also called paging) is the process of dividing a document into discrete pages, whether electronic or printed. Historically, pagination referred to consecutive page numbering to indicate proper page order in books — a practice that became common around 1550, replacing foliation (which numbered only the front sides of folios). In modern usage, pagination encompasses both the physical division of content into pages and the algorithms, UI patterns, and database techniques used to manage paged content across print, desktop publishing, and web applications.

## Key Concepts

- **Pagination vs. foliation**: Foliation numbered only recto (front) sides of leaves; pagination numbers every page sequentially. Pagination became standard c. 1550.
- **Automated pagination**: Word processors, desktop publishing, and digital typesetting tools use algorithms to decide page breaks, word wrapping, and paragraph endings — all of which can be manually overridden.
- **Manual overrides**: Soft hyphens, manual line breaks, hard returns, and manual page breaks allow human control over automated pagination decisions.
- **Widows and orphans**: Cultural/typographic rules that influence where page breaks fall — pagination systems vary in sophistication for handling these.
- **Electronic pages**: Paginated content in documents or presentations that exist as visual electronic documents; size may be fixed (like a Word doc) or dynamic (like HTML).
- **Client-side pagination**: All records are pre-loaded in HTML source; JavaScript or CSS handles page display. Best for small data sets.
- **Server-side pagination**: Each page is individually requested from the server upon navigation. More common; better for large data sets.
- **Hybrid (AJAX) pagination**: JavaScript requests subsequent pages from the server via AJAX and inserts them into the DOM — combines benefits of both approaches.
- **Infinite scrolling vs. pagination**: Pagination allows skipping pages and supports permanent links (e.g., `offset` URL parameter); infinite scrolling displays content continuously and dynamically.
- **Database pagination**: Limits query results to a subset of rows (e.g., 10 at a time), reducing load and wait times — especially important in stateless web architectures with no dedicated client-server connection.

## Commands and Syntax

- **Page break control in markup**: Manual page breaks can be inserted via CSS (`page-break-before`, `page-break-after`, `break-before`, `break-after`) or word processor controls.
- **URL-based pagination**: Common pattern uses an `offset` parameter (e.g., `?offset=20`) to create permanent links to specific pages — as used in MediaWiki.
- **SQL pagination** (see `SELECT` with `LIMIT`/`OFFSET`):
  ```sql
  SELECT * FROM table LIMIT 10 OFFSET 20;
  ```
- **Separation of content and presentation**: Use semantic markup (XML, HTML, SGML) with transformation technologies (XSLT, XSL, CSS) to separate content from pagination/presentation decisions.

## Relationships

- **Page numbering**: Pagination is closely related to and often synonymous with page numbering in print contexts.
- **Widows and orphans**: Typographic rules that constrain pagination algorithms.
- **Separation of presentation and content**: Modern best practice — content is tagged semantically (XML/HTML/SGML), and pagination is applied downstream via stylesheets (CSS/XSLT), reducing manual pagination needs.
- **Word processing / desktop publishing / digital typesetting**: Technologies that automate pagination for print-oriented output.
- **Search engines and forums**: Primary web use cases where server-side pagination divides large result sets.
- **AJAX and DOM**: Enable hybrid pagination patterns in web applications.
- **Infinite scrolling**: The primary alternative to pagination in web UIs, with different trade-offs around navigation, deep linking, and performance.
- **SQL SELECT with LIMIT/OFFSET**: The database-level mechanism underpinning server-side pagination.

## Exam-Relevant Points

- Pagination replaced foliation c. 1550; foliation numbered only front sides of folios.
- **Three pagination approaches in web**: client-side (pre-loaded, JS/CSS driven), server-side (per-page requests), and hybrid AJAX (JS requests + DOM insertion).
- Server-side pagination is preferred for **large data sets** — faster initial load, accessibility without JavaScript, supports complex business logic.
- Client-side pagination is appropriate only when there are **very few records**.
- Pagination supports **permanent links** (via URL parameters like `offset`); infinite scrolling does not.
- The **separation of presentation and content** principle means the same content can be paginated differently for print vs. screen using semantic markup + stylesheets.
- Database pagination limits rows returned per query, critical in **stateless web architectures** where there is no persistent client-server connection.
- Usability considerations for pagination controls: whether to include previous/next links, how many page links to show, whether to link first/last pages, and allowing users to set records per page.
