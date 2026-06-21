---
source: sources/wiki-Web_application.md
source_url: https://en.wikipedia.org/wiki/Web_application
---

## Web Applications: Architecture, History, and Security

A web application (web app) is application software built with web technologies that runs in a web browser. This page covers the definition, historical evolution, multi-tier architecture, security considerations, and development practices of web applications, from early server-side dynamic pages through modern SPAs and PWAs.

## Key Concepts

- **Web application** — application software that runs via a web browser, delivered over a web server, as opposed to native installed software
- **Dynamic vs. static** — web apps emerged in the late 1990s to dynamically generate server responses, unlike static web pages
- **Single-Page Applications (SPAs)** — architectural approach where the app loads a single HTML page and dynamically updates content without full page reloads, providing a native-app-like experience
- **Progressive Web Apps (PWAs)** — term coined in 2015 by Frances Berriman and Alex Russell; apps that leverage modern browser features to run offline and launch without entering a URL (behave like installed apps)
- **Three-tier architecture** — the most common web app structure:
  - **Presentation tier** — the web browser (client/UI)
  - **Application tier** — server-side logic engine (ASP, CGI, Node.js, PHP, Python, Ruby on Rails, Java Servlets, etc.)
  - **Storage tier** — the database
- **N-tier architecture** — extends three-tier by decomposing business logic into finer-grained layers; may add an integration tier to abstract data access (e.g., calling `list_clients()` instead of raw SQL)
- **Two-tier architecture** — "smart client / dumb server" or "dumb client / smart server"; simpler but limited scalability
- **Ajax** — technique named in 2005 for asynchronous client-server communication without full page reloads; later succeeded by Web APIs using JSON
- **Cloud hosting** — web apps often run entirely on cloud services, enabling SaaS billing models, vendor lock-in, and thin-client access
- **Browser sandboxing** — modern browsers (e.g., Chrome) sandbox each tab, restricting access to local resources and improving security
- **Responsive web design** — allows the same codebase to work across devices and operating systems by targeting browser standards
- **Web application frameworks** — facilitate rapid development by handling common concerns (e.g., user management), letting teams focus on unique business logic

## Commands and Syntax

No specific CLI commands or configuration syntax are described. Key technologies referenced for the application tier include:

- **Server-side engines**: ASP, CGI, ColdFusion, Dart, JSP/Java Servlets, Node.js, PHP, Python, Ruby on Rails
- **Client-side**: JavaScript (introduced by Netscape in 1995), XMLHttpRequest (introduced in IE5 as ActiveX)
- **Data interchange**: XML (early), JSON (modern standard via Web APIs)
- **Protocols**: HTTP (v2, v3), WebSocket, CGI, SCGI, FCGI
- **Server APIs**: WSGI (Python), ASGI (Python), Rack (Ruby), JSGI (JavaScript), PSGI (Perl), OWIN (.NET), Jakarta Servlet

## Relationships

- **SaaS** — web apps are the delivery mechanism for Software as a Service
- **Web frameworks** — tools like Rails, Django, Express that accelerate web app development
- **Ajax / Web APIs** — communication patterns that enable rich client-side interactivity
- **Internet security** — web app security is a subset of broader internet security concerns
- **Client-server model** — web apps evolved from traditional client-server architectures where both sides required platform-specific installation
- **Web standards (W3C, WHATWG)** — HTML5, DOM APIs, WebSocket, WebAssembly, and other standards that web apps rely on
- **Cloud services** — infrastructure layer enabling web app hosting, scaling, and billing
- **Browser APIs** — Canvas, IndexedDB, Web Storage, Service Workers, WebRTC, WebAssembly enable increasingly capable client-side functionality

## Exam-Relevant Points

- The term "web application" was first introduced in the **Java Servlet Specification v2.2 (1999)**
- **JavaScript** was introduced by **Netscape in 1995** for client-side scripting
- **XMLHttpRequest** was first introduced in **Internet Explorer 5** as an ActiveX object
- The term **Ajax** was coined in **2005**
- **PWA** term coined in **2015** by Frances Berriman and Alex Russell (Google Chrome)
- The three-tier model: **Presentation (browser) → Application (server logic) → Storage (database)**
- N-tier's key benefit: **finer-grained business logic decomposition** and the ability to **replace the database without affecting other tiers** via an integration/abstraction layer
- Key security areas for web apps: **authentication, authorization, asset handling, input validation, logging, and auditing**
- Web apps eliminate per-client installation, reducing **support costs** and improving **portability** across operating systems
- Web apps shifted from XML-based Ajax to **JSON-based Web APIs** accessed asynchronously via JavaScript
- Early web app milestones: Myspace (2003), Gmail (2004), Digg (2004), Google Maps (2005)
