---
source: sources/wiki-Single-page_application.md
source_url: https://en.wikipedia.org/wiki/Single-page_application
---

## Single-Page Applications (SPAs)

A single-page application is a web application that dynamically rewrites the current page with new data from the server rather than loading entirely new pages. The goal is faster transitions that feel more like a native app. All necessary HTML, JavaScript, and CSS is either retrieved in a single page load or dynamically loaded in response to user actions — a full page refresh never occurs.

## Key Concepts

- **Core principle**: The browser never performs a full page reload; the DOM is updated dynamically via JavaScript.
- **Thin server architecture**: Logic shifts from server to client; the server becomes a pure data API/web service.
- **Thick stateful server**: Server maintains client page state in memory and sends delta changes (HTML/JS) to update the client DOM. Simplifies development but requires more server resources.
- **Thick stateless server**: Client sends its current state to the server with each request; server reconstructs state, computes changes, and returns them. More scalable (no per-client state on server) but higher per-request computational cost.
- **Data transport**: Server responses are typically raw data (XML/JSON) that client-side JS translates to HTML, or pre-rendered HTML fragments that are inserted into the DOM.
- **SPAs can run locally** using the `file://` URI scheme with browser-based Web Storage for persistence, requiring no server connectivity.
- **Page lifecycle**: The SPA loads fully on initial request, then progressively downloads page fragments or screen modules on demand. "States" in a SPA are analogous to "pages" in a traditional site.

## Commands and Syntax

- **Document hashes technique**: Use HTML element IDs with the CSS `:target` pseudo-class selector to show/hide sections without JavaScript.
- **Ajax**: Use `XMLHttpRequest` or `fetch()` for asynchronous server requests returning XML/JSON data.
- **Browser history management**:
  - Hash fragment identifiers (`window.location.hash`) for backward compatibility.
  - `history.pushState()` and `history.replaceState()` for programmatic URL and history manipulation (HTML5 History API).
- **WebSockets**: Bidirectional real-time client-server communication; superior to Ajax for real-time use cases.
- **Server-Sent Events (SSE)**: Server-initiated data push over standard HTTP; supports automatic reconnection, event IDs, and arbitrary events (features WebSockets lack by design).

## Relationships

- **JavaScript frameworks**: Angular, React, Vue.js, Svelte, Ember.js, Knockout.js, Meteor.js, ExtJS — all adopt SPA principles with varying architectural patterns (MVC, MVVM, component-based).
- **WebAssembly frameworks**: Blazor (C#/.NET), Flutter Web (Dart), Avalonia, Uno Platform, OpenSilver — extend the SPA model beyond JavaScript.
- **Newer hybrid frameworks**: Astro, Fresh, enhance.dev — emphasize server-side rendering and progressive enhancement while minimizing client-side JS; Astro hydrates only interactive parts, Fresh has zero runtime overhead.
- **Progressive Web Applications (PWA)**: Related concept for native-like web experiences.
- **Server-side rendering (SSR)**: Complementary technique where the first page load is rendered on the server, subsequent updates on the client; addresses SEO and initial load performance.
- **Rich web applications**: Earlier term for the same concept.

## Exam-Relevant Points

- **SEO challenge**: Search engine crawlers historically couldn't execute JavaScript. Google's deprecated "hash-bang" (`#!`) AJAX crawling scheme (2009–2015) was replaced by recommendations for SSR, static rendering, or hydration. As of 2024, Google no longer recommends dynamic rendering.
- **Browser history problem**: SPAs break the back/forward button by default. Solutions: hash fragment identifiers (legacy) or the HTML5 History API (`pushState`/`replaceState`).
- **Analytics integration**: SPAs don't trigger native page loads, so analytics tools like Google Analytics require explicit function calls on state changes. The HTML History API can add synthetic page load events.
- **Security considerations**: SPAs face traditional risks (XSS) plus unique vulnerabilities: data exposure via APIs, client-side logic exposure, and client-side enforcement of server-side security. DAST scanners struggle with JS-heavy SPAs.
- **Performance trade-off**: Initial load is heavier (must download framework + app code + API data). Mitigation strategies: selective prerendering, caching, code splitting, lazy loading. Subsequent navigation is faster.
- **Svelte's differentiator**: Compiles components to efficient JS DOM manipulations at build time — no virtual DOM, no framework bundle shipped to the client.
- **Architectural patterns by framework**: AngularJS/Ember = MVC, Knockout = MVVM, React = component + unidirectional data flow (often with Redux), Meteor = full-stack with DDP and pub/sub.
- **Server architecture scalability**: Thick stateless > thick stateful for horizontal scaling because no per-client session state requires sharing or server affinity.
