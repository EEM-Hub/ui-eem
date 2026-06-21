---
source: https://en.wikipedia.org/wiki/Single-page_application
fetched: 2026-06-20
---

Web application that interacts with the user by dynamically rewriting a web page 

A **single-page application** (**SPA**) is a [web application](./Web_application) or [website](./Website) that interacts with the user by dynamically rewriting the current [web page](./Web_page) with new data from the [web server](./Web_server), instead of the default method of loading entire new pages. The goal is faster transitions that make the website [feel](./User_experience) more like a [native](./Native_(computing)) [app](./Application_software).

 

In a SPA, a page refresh never occurs; instead, all necessary [HTML](./HTML), [JavaScript](./JavaScript), and [CSS](./CSS) code is either retrieved by the browser with a single page load,[[1]](./Single-page_application#cite_note-Flanagan2006-1) or the appropriate resources are dynamically loaded and added to the page as necessary, usually in response to user actions.

 

## History

 

The origins of the term *single-page application* are unclear, though the concept was discussed at least as early as 2003 by technology evangelists from Netscape.[[2]](./Single-page_application#cite_note-2) Stuart Morris, a programming student at Cardiff University, Wales, wrote the [self-contained](./Self-contained_system_(software)) website at slashdotslash.com with the same goals and functions in April 2002,[[3]](./Single-page_application#cite_note-3) and later the same year Lucas Birdeau, Kevin Hakman, Michael Peachey and Clifford Yeh described a single-page application implementation in US patent 8,136,109.[[4]](./Single-page_application#cite_note-4) Earlier forms were called [rich web applications](./Rich_web_application).

 

JavaScript can be used in a web browser to display the [user interface](./User_interface) (UI), run application logic, and communicate with a web server. Mature [free](./Free_software) libraries are available that support the building of a SPA, reducing the amount of JavaScript code developers have to write.

 

## Technical approaches

 

There are various techniques available that enable the browser to retain a single page even when the application requires server communication.

 

### Document hashes

 

HTML authors can leverage element IDs to show or hide different sections of the HTML document.  Then, using CSS, authors can use the `:target` pseudo-class selector to only show the section of the page which the browser navigated to.

 

### JavaScript frameworks

 

Web browser JavaScript frameworks and libraries, such as [Angular](./Angular_(web_framework)), [Ember.js](./Ember.js), [ExtJS](./ExtJS), [Knockout.js](./Knockout.js), [Meteor.js](./Meteor_(web_framework)), [React](./React_(JavaScript_library)), [Vue.js](./Vue.js), and [Svelte](./Svelte) have adopted SPA principles. Aside from ExtJS, all of these are free. 

 
- [AngularJS](./AngularJS) is a discontinued fully client-side framework. AngularJS's templating is based on bidirectional [UI data binding](./UI_data_binding). Data-binding is an automatic way of updating the view whenever the model changes, as well as updating the model whenever the view changes. The HTML template is compiled in the browser. The compilation step creates pure HTML, which the browser re-renders into the live view. The step is repeated for subsequent page views. In traditional server-side HTML programming, concepts such as controller and model interact within a server process to produce new HTML views. In the AngularJS framework, the controller and model states are maintained within the client browser. Therefore, new pages are capable of being generated without any interaction with a server.
- [Angular 2+](./Angular_(web_framework)) is a SPA Framework developed by Google after AngularJS. There is a strong community of developers using this framework. The framework is updated twice every year. New features and fixes are frequently added in this framework.
- [Ember.js](./Ember.js) is a client-side JavaScript web application framework based on the [model–view–controller](./Model–view–controller) (MVC) software architectural pattern. It allows developers to create scalable single-page applications by incorporating common idioms and best practices into a framework that provides a rich object model, declarative two-way data binding, computed properties, automatically updating templates powered by Handlebars.js, and a router for managing application state.
- [ExtJS](./ExtJS) is also a client-side framework that allows creating MVC applications. It has its own event system, window and layout management, state management (stores) and various UI components (grids, dialog windows, form elements etc.). It has its own class system with either dynamic or static loader. The application built with ExtJS can either exist on its own (with state in the browser) or with the server (e.g. with [REST](./REST) API that is used to fill its internal stores). ExtJS has only built in capabilities to use localStorage so larger applications need a server to store state.
- [Knockout.js](./Knockout.js) is a client-side framework which uses templates based on the [model–view–viewmodel](./Model–view–viewmodel) (MVVM) pattern.
- [Meteor.js](./Meteor_(web_framework)) is a full-stack (client-server) JavaScript framework designed exclusively for SPAs. It features simpler data binding than Angular, Ember or ReactJS,[[5]](./Single-page_application#cite_note-5) and uses the [Distributed Data Protocol](./Distributed_Data_Protocol)[[6]](./Single-page_application#cite_note-6) and a [publish–subscribe pattern](./Publish–subscribe_pattern) to automatically propagate data changes to clients in real-time without requiring the developer to write any synchronization code. Full stack reactivity ensures that all layers, from the database to the templates, update themselves automatically when necessary. Ecosystem packages such as *Server-Side Rendering*[[7]](./Single-page_application#cite_note-7)[[8]](./Single-page_application#cite_note-8) address the problem of search engine optimization.
- [React](./React_(JavaScript_library)) is a [JavaScript library](./JavaScript_library) for building [user interfaces](./User_interfaces). It is maintained by [Facebook](./Facebook), [Instagram](./Instagram) and a community of individual developers and corporations. React uses a syntax extension for JavaScript, named [JSX](./JSX_(JavaScript)), which is a mix of JS and HTML (a subset of HTML). Several companies use React with [Redux (JavaScript library)](./Redux_(JavaScript_library)) which adds state management capabilities, which (with several other libraries) lets developers create complex applications.[[9]](./Single-page_application#cite_note-9)
- [Vue.js](./Vue.js) is a JavaScript framework for building user interfaces. Vue developers also provide Pinia for state management.
- [Svelte](./Svelte) is a framework for building user interfaces that compiles Svelte code to JavaScript DOM (Document Object Model) manipulations, avoiding the need to bundle a framework to the client, and allowing for simpler application development syntax.

 

#### Capabilities and trade-offs in modern frameworks

 

JavaScript-based web application frameworks, such as React and Vue, provide extensive capabilities but come with associated trade-offs. These frameworks often extend or enhance features available through native web technologies, such as routing, component-based development, and state management. While native web standards, including Web Components, modern JavaScript APIs like Fetch and ES Modules, and browser capabilities like Shadow DOM, have advanced significantly, frameworks remain widely used for their ability to enhance developer productivity, offer structured patterns for large-scale applications, simplify handling edge cases, and provide tools for performance optimization.[[10]](./Single-page_application#cite_note-:0-10)[[11]](./Single-page_application#cite_note-:1-11)[[12]](./Single-page_application#cite_note-:2-12)

 

Frameworks can introduce abstraction layers that may contribute to performance overhead, larger bundle sizes, and increased complexity. Modern frameworks, such as React 18 and Vue 3, address these challenges with features like concurrent rendering, tree-shaking, and selective hydration. While these advancements improve rendering efficiency and resource management, their benefits depend on the specific application and implementation context. Lightweight frameworks, such as Svelte and Preact, take different architectural approaches, with Svelte eliminating the virtual DOM entirely in favor of compiling components to efficient JavaScript code, and Preact offering a minimal, compatible alternative to React. Framework choice depends on an application’s requirements, including the team’s expertise, performance goals, and development priorities.[[10]](./Single-page_application#cite_note-:0-10)[[11]](./Single-page_application#cite_note-:1-11)[[12]](./Single-page_application#cite_note-:2-12)

 

A newer category of web frameworks, including enhance.dev, Astro, and Fresh, leverages native web standards while minimizing abstractions and development tooling.[[13]](./Single-page_application#cite_note-13)[[14]](./Single-page_application#cite_note-14)[[15]](./Single-page_application#cite_note-15) These solutions emphasize [progressive enhancement](./Progressive_enhancement), [server-side rendering](./Server-side_rendering), and optimizing performance. Astro renders static HTML by default while hydrating only interactive parts. Fresh focuses on server-side rendering with zero runtime overhead. Enhance.dev prioritizes progressive enhancement patterns using Web Components. While these tools reduce reliance on client-side JavaScript by shifting logic to build-time or server-side execution, they still use JavaScript where necessary for interactivity. This approach makes them particularly suitable for performance-critical and content-focused applications.[[10]](./Single-page_application#cite_note-:0-10)[[11]](./Single-page_application#cite_note-:1-11)[[12]](./Single-page_application#cite_note-:2-12)

 

### WebAssembly-based frameworks

 

The following frameworks utilize [WebAssembly](./WebAssembly) or can build single-page applications (SPAs) with WebAssembly as a core technology or support mechanism. These frameworks enable high-performance and interactive client-side development, extending the SPA paradigm across languages and ecosystems.

 
- [Avalonia](./Avalonia_(software_framework)) is primarily a cross-platform desktop [UI](./User_interface) framework, but experimental support for [WebAssembly](./WebAssembly) allows it to be used for SPA development. It has an XAML-based UI design and native-style application features.
- [Blazor WebAssembly](./Blazor) is a .NET-based framework that allows developers to build SPAs using [C#](./C_Sharp_(programming_language)) and [Razor](./ASP.NET_Razor) syntax. It runs [.NET](./.NET) code in the browser via WebAssembly, enabling a full-stack .NET development experience without relying on JavaScript.
- [Flutter on the Web](./Flutter_(software)) extends Flutter’s cross-platform development capabilities to web-based SPAs. Using Dart and its Skia graphics engine, Flutter allows developers to create visually rich SPAs that run in the browser.
- [OpenSilver](./OpenSilver) is another open-source reimplementation of Silverlight but targeted toward SPAs developed with C# and [XAML](./Extensible_Application_Markup_Language). It uses WebAssembly to run the .NET code in the browser, so it's fitted for highly interactive client-side applications.
- [Uno Platform](./Uno_Platform) is a cross-platform framework that supports SPA development through WebAssembly. It allows developers to use XAML and C# to build applications that run on the Web, mobile, and desktop platforms, with UI components rendered directly in the browser.

 

### Ajax

 

As of 2006, the most prominent technique used was [Ajax](./Ajax_(programming)).[[1]](./Single-page_application#cite_note-Flanagan2006-1) Ajax involves using asynchronous requests to a server for [XML](./XML) or [JSON](./JSON) data, such as with JavaScript's [XMLHttpRequest](./XMLHttpRequest) or more modern `fetch()` (since 2017), or the deprecated [ActiveX Object](./ActiveX_Data_Objects). In contrast to the [declarative](./Declarative_programming) approach of most SPA frameworks, with Ajax the website directly uses JavaScript or a JavaScript library such as [jQuery](./JQuery) to manipulate the [DOM](./Document_Object_Model) and edit HTML elements. Ajax has further been popularized by libraries like [jQuery](./JQuery), which provides a simpler syntax and normalizes Ajax behavior across different browsers which historically had varying behavior.

 

### WebSockets

 

[WebSockets](./WebSocket) are a bidirectional real-time client-server communication technology that are part of the HTML specification. For real-time communication, their use is superior to Ajax in terms of performance[[16]](./Single-page_application#cite_note-16) and simplicity.

 

### Server-sent events

 

[Server-sent events](./Server-sent_events) (SSEs) is a technique whereby servers can initiate data transmission to browser clients. Once an initial connection has been established, an event stream remains open until closed by the client. SSEs are sent over traditional HTTP and have a variety of features that WebSockets lack by design such as automatic reconnection, event IDs, and the ability to send arbitrary events.[[17]](./Single-page_application#cite_note-17)

 

### Browser plugins

 

Although this method is outdated, asynchronous calls to the server may also be achieved using browser plug-in technologies such as [Silverlight](./Microsoft_Silverlight), [Flash](./Adobe_Flash), or [Java applets](./Java_applet).

 

### Data transport (XML, JSON and Ajax)

 

Requests to the server typically result in either raw data (e.g., [XML](./XML) or [JSON](./JSON)), or new [HTML](./HTML) being returned. In the case where HTML is returned by the server, JavaScript on the client updates a partial area of the DOM ([Document Object Model](./Document_Object_Model)). When raw data is returned, JavaScript on the client translates it into HTML using [XSL](./XSL) or a JSON [template](./Web_template_system#Client-Side_Systems) before updating the DOM.

 

### Server architecture

 

#### Thin server architecture

 

A SPA moves logic from the server to the client, with the role of the web server evolving into a pure data API or web service. This architectural shift has, in some circles, been coined "Thin Server Architecture" to highlight that complexity has been moved from the server to the client, with the argument that this ultimately reduces overall complexity of the system.

 

#### Thick stateful server architecture

 

The server keeps the necessary state in memory of the client state of the page. In this way, when any request hits the server (usually user actions), the server sends the appropriate HTML and/or JavaScript with the concrete changes to bring the client to the new desired state (usually adding/deleting/updating a part of the client DOM). At the same time, the state in server is updated. Most of the logic is executed on the server, and HTML is usually also rendered on the server. In some ways, the server simulates a web browser, receiving events and performing delta changes in server state which are automatically propagated to client.

 

This approach needs more server memory and server processing, but the advantage is a simplified development model because a) the application is usually fully coded in the server, and b) data and UI state in the server are shared in the same memory space with no need for custom client/server communication bridges.

 

#### Thick stateless server architecture

 

This is a variant of the stateful server approach. The client page sends data representing its current state to the server, usually through Ajax requests. Using this data, the server is able to reconstruct the client state of the part of the page which needs to be modified and can generate the necessary data or code (for instance, as JSON or JavaScript), which is returned to the client to bring it to a new state, usually modifying the page DOM tree according to the client action that motivated the request.

 

This approach requires that more data be sent to the server and may require more computational resources per request to partially or fully reconstruct the client page state in the server. At the same time, this approach is more easily scalable because there is no per-client page data kept in the server and, therefore, Ajax requests can be dispatched to different server nodes with no need for session data sharing or server affinity.

 

## Running locally

 

Some SPAs may be executed from a local file using the [file URI scheme](./File_URI_scheme). This gives users the ability to download the SPA from a server and run the file from a local storage device, without depending on server connectivity. If such a SPA wants to store and update data, it must use browser-based [Web Storage](./Web_Storage). These applications benefit from advances available with [HTML](./HTML).[[18]](./Single-page_application#cite_note-18)

 

## Challenges with the SPA model

 

Because the SPA is an evolution away from the stateless page-redraw model that browsers were originally designed for, some new challenges have emerged. Possible solutions (of varying complexity, comprehensiveness, and author control) include:[[19]](./Single-page_application#cite_note-spimanifesto-19)

 
- client-side JavaScript libraries
- server-side web frameworks that specialize in the SPA model[[20]](./Single-page_application#cite_note-20)[[21]](./Single-page_application#cite_note-21)[[22]](./Single-page_application#cite_note-22)
- the evolution of browsers and the HTML specification,[[23]](./Single-page_application#cite_note-23) designed for the SPA model

 

### Search-engine optimization

 

Because of the lack of JavaScript execution on crawlers of some popular [Web search engines](./Web_search_engines),[[24]](./Single-page_application#cite_note-24) SEO ([search engine optimization](./Search_engine_optimization)) has historically presented a problem for public facing websites wishing to adopt the SPA model.[[25]](./Single-page_application#cite_note-doogledevelopers-25)

 

Between 2009 and 2015, [Google Webmaster Central](./Google_Webmaster_Tools) proposed and then recommended an "AJAX crawling scheme"[[26]](./Single-page_application#cite_note-26)[[27]](./Single-page_application#cite_note-27) using an initial exclamation mark in fragment identifiers for stateful [AJAX](./AJAX) pages (`#!`).  Special behavior must be implemented by the SPA site to allow extraction of relevant metadata by the search engine's crawler. For search engines that do not support this [URL hash](./URI_fragment) scheme, the hashed URLs of the SPA remain invisible.  These "hash-bang" URIs have been considered problematic by a number of writers including Jeni Tennison at the W3C because they make pages inaccessible to those who do not have [JavaScript](./JavaScript) activated in their browser. They also break [HTTP referer](./HTTP_referer) headers as browsers are not allowed to send the fragment identifier in the Referer header.[[28]](./Single-page_application#cite_note-Tennison2-28) In 2015, Google deprecated their hash-bang AJAX crawling proposal.[[29]](./Single-page_application#cite_note-29)

 

Alternatively, applications may render the first page load on the server and subsequent page updates on the client. This is traditionally difficult, because the rendering code might need to be written in a different language or framework on the server and in the client. Using logic-less templates, cross-compiling from one language to another, or using the same language on the server and the client may help to increase the amount of code that can be shared.

 

In 2018, Google introduced dynamic rendering as another option for sites wishing to offer crawlers a non-JavaScript heavy version of a page for indexing purposes.[[30]](./Single-page_application#cite_note-DynamicRendering-30) Dynamic rendering switches between a version of a page that is rendered client-side and a pre-rendered version for specific user agents. This approach involves your web server detecting crawlers (via the user agent) and routing them to a renderer, from which they are then served a simpler version of HTML content. As of 2024, Google no longer recommends dynamic rendering,[[31]](./Single-page_application#cite_note-DynamicRenderingWorkaround-31) suggesting "[server-side rendering](./Server-side_rendering), [static rendering](./Static_rendering), or [hydration](./Hydration_(web_development))" instead.

 

Because SEO compatibility is not trivial in SPAs, SPAs are commonly not used in a context where search engine indexing is either a requirement, or desirable. Use cases include applications that surface private data hidden behind an [authentication](./Authentication) system. In the cases where these applications are consumer products, often a classic "page redraw" model is used for the applications landing page and marketing site, which provides enough meta data for the application to appear as a hit in a search engine query. Blogs, support forums, and other traditional page redraw artifacts often sit around the SPA that can seed search engines with relevant terms.

 

As of 2021 and Google specifically, SEO compatibility for a plain SPA is straightforward and requires just a few simple conditions to be met.[[32]](./Single-page_application#cite_note-32)

 

One way to increase the amount of code that can be shared between servers and clients is to use a logic-less template language like [Mustache](./Mustache_(template_system)) or [Handlebars](./Handlebars_(template_system)). Such templates can be rendered from different host languages, such as [Ruby](./Ruby_(programming_language)) on the server and [JavaScript](./JavaScript) in the client. However, merely sharing templates typically requires duplication of [business logic](./Business_logic) used to choose the correct templates and populate them with data. Rendering from templates may have negative performance effects when only updating a small portion of the page—such as the value of a text input within a large template. Replacing an entire template might also disturb a user's selection or cursor position, where updating only the changed value might not. To avoid these problems, applications can use [UI data bindings](./UI_data_binding) or granular [DOM](./Document_Object_Model) manipulation to only update the appropriate parts of the page instead of re-rendering entire templates.[[33]](./Single-page_application#cite_note-Holmes2015-33)

 

### Browser history

 

With a SPA being, by definition, "a single page", the model breaks the browser's design for page history navigation using the "forward" or "back" buttons. This presents a usability impediment when a user presses the back button, expecting the previous screen state within the SPA, but instead, the application's single page unloads and the previous page in the browser's history is presented.

 

The traditional solution for SPAs has been to change the browser URL's hash [fragment identifier](./Fragment_identifier) in accord with the current screen state. This can be achieved with JavaScript, and causes URL history events to be built up within the browser. As long as the SPA is capable of resurrecting the same screen state from information contained within the URL hash, the expected back-button behavior is retained.

 

To further address this issue, the HTML specification has introduced [pushState](http://www.w3.org/html/wg/drafts/html/master/browsers.html#dom-history-pushstate) and [replaceState](http://www.w3.org/html/wg/drafts/html/master/browsers.html#dom-history-replacestate) providing programmatic access to the actual URL and browser history.

 

### Analytics

 

Analytics tools such as [Google Analytics](./Google_Analytics) rely heavily upon entire new pages loading in the browser, initiated by a new page load. SPAs do not work this way.

 

After the first page load, all subsequent page and content changes are handled internally by the application, which should simply call a function to update the analytics package. Failing to call such a function, the browser never triggers a new page load, nothing gets added to the browser history, and the analytics package has no idea who is doing what on the site.

 

### Security scanning

 

Similarly to the problems encountered with search engine crawlers, [DAST tools](./Dynamic_application_security_testing) may struggle with these JavaScript-rich applications. Problems can include the lack of hypertext links, memory usage concerns and resources loaded by the SPA typically being made available by an [Application Programming Interface](./Application_Programming_Interface) or API. Single-page applications are still subject to the same security risks as traditional web pages such as [Cross-Site Scripting (XSS)](./Cross-site_scripting), but also a host of other unique vulnerabilities such as data exposure via API and client-side logic and client-side enforcement of server-side security.[[34]](./Single-page_application#cite_note-34) In order to effectively scan a single-page application, a DAST scanner must be able to navigate the client-side application in a reliable and repeatable manner to allow discovery of all areas of the application and interception of all requests that the application sends to remote servers (e.g. API requests).

 

### Adding page loads to a SPA

 

It is possible to add page load events to a SPA using the HTML History API; this will help integrate analytics. The difficulty comes in managing this and ensuring that everything is being tracked accurately – this involves checking for missing reports and double entries.
Some frameworks provide free analytics integrations addressing most of the major analytics providers. Developers can integrate them into the application and make sure that everything is working correctly, but there is no need to do everything from scratch.[[33]](./Single-page_application#cite_note-Holmes2015-33)

 

### Speeding up the page load

 

There are some ways of speeding up the initial load of a SPA, such as selective prerendering of the SPA landing/index page, caching and various code splitting techniques including lazy-loading modules when needed. But it's not possible to get away from the fact that it needs to download the framework, at least some of the application code; and will hit an API for data if the page is dynamic.[[33]](./Single-page_application#cite_note-Holmes2015-33) This is a "pay me now, or pay me later" trade-off scenario. The question of performance and wait-times remains a decision that the developer must make.

 

## Page lifecycle

 
|  | This sectionneeds additional citations forverification.Please helpimprove this articlebyadding citations to reliable sourcesin this section. Unsourced material may be challenged and removed.Find sources:"Single-page application"–news·newspapers·books·scholar·JSTOR(October 2020)(Learn how and when to remove this message) |
| --- | --- |

 

A SPA is fully loaded in the initial page load and then page regions are replaced or updated with new page fragments loaded from the server on demand. To avoid excessive downloading of unused features, a SPA will often progressively download more features as they become required, either small fragments of the page, or complete screen modules.

 

In this way an analogy exists between "states" in a SPA and "pages" in a traditional website. Because "state navigation" in the same page is analogous to page navigation, in theory, any page-based web site could be converted to single-page replacing in the same page only the changed parts.

 

The SPA approach on the web is similar to the [single-document interface](./Multiple-document_interface) (SDI) presentation technique popular in [native](./Native_(computing)) desktop applications.

 

## See also

 
- [Progressive web application (PWA)](./Progressive_web_application)
- [Server-side scripting](./Server-side_scripting)

 

## References

 
1. [1](./Single-page_application#cite_ref-Flanagan2006_1-0) [2](./Single-page_application#cite_ref-Flanagan2006_1-1) Flanagan, David, "[JavaScript - The Definitive Guide](https://books.google.com/books?id=2weL0iAfrEMC&q=%22single-page%22)", 5th ed., *O'Reilly, Sebastopol, CA, 2006*, p.497
2. [↑](./Single-page_application#cite_ref-2) ["Inner-Browsing: Extending Web Browsing the Navigation Paradigm"](https://web.archive.org/web/20030810102320/http://devedge.netscape.com/viewsource/2003/inner-browsing). Archived from [the original](http://devedge.netscape.com/viewsource/2003/inner-browsing) on August 10, 2003. Retrieved May 16, 2003.
3. [↑](./Single-page_application#cite_ref-3) ["Slashdotslash.com: A self contained website using DHTML"](http://www.slashdotslash.com/scws/index.html). Retrieved July 6, 2012.
4. [↑](./Single-page_application#cite_ref-4) ["US patent 8,136,109"](https://patents.google.com/patent/US8136109).
5. [↑](./Single-page_application#cite_ref-5) ["Meteor Blaze"](https://github.com/meteor/blaze). *[GitHub](./GitHub)*. 6 May 2022. Blaze is a powerful library for creating user interfaces by writing reactive HTML templates.
6. [↑](./Single-page_application#cite_ref-6) [Introducing DDP](http://meteor.com/blog/2012/03/21/introducing-ddp), March 21, 2012
7. [↑](./Single-page_application#cite_ref-7) Ćwirko, Julian (2017-09-07). ["Server-side rendering (SSR) in Meteor"](http://web.archive.org/web/20191004124221/https://blog.meteor.com/meteor-platform-is-still-alive-5f6426644555). *Medium*. Archived from [the original](https://blog.meteor.com/meteor-platform-is-still-alive-5f6426644555) on 2019-10-04. Retrieved 2026-06-10.
8. [↑](./Single-page_application#cite_ref-8) ["Server Side Rendering for Meteor"](https://web.archive.org/web/20150320063111/https://meteorhacks.com/server-side-rendering.html). Archived from [the original](https://meteorhacks.com/server-side-rendering.html) on March 20, 2015. Retrieved January 31, 2015.
9. [↑](./Single-page_application#cite_ref-9) ["Single-page applications vs. multiple-page applications: pros, cons, pitfalls - BLAKIT - IT Solutions"](https://blak-it.com/blog/spa-advantages/). *blak-it.com*. BLAKIT - IT Solutions. October 17, 2017. Retrieved October 19, 2017.
10. [1](./Single-page_application#cite_ref-:0_10-0) [2](./Single-page_application#cite_ref-:0_10-1) [3](./Single-page_application#cite_ref-:0_10-2) Uzayr, Sufyan bin; Cloud, Nicholas; Ambler, Tim (November 2019). *JavaScript Frameworks for Modern Web Development: The Essential Frameworks, Libraries, and Tools to Learn Right Now*. Apress. [ISBN](./ISBN_(identifier)) [978-1484249949](./Special:BookSources/978-1484249949).
11. [1](./Single-page_application#cite_ref-:1_11-0) [2](./Single-page_application#cite_ref-:1_11-1) [3](./Single-page_application#cite_ref-:1_11-2) Rojas, Carlos (13 November 2020). *Building Native Web Components: Front-End Development with Polymer and Vue.js*. Apress. [ISBN](./ISBN_(identifier)) [978-1484259047](./Special:BookSources/978-1484259047).
12. [1](./Single-page_application#cite_ref-:2_12-0) [2](./Single-page_application#cite_ref-:2_12-1) [3](./Single-page_application#cite_ref-:2_12-2) *Hands-On JavaScript High Performance: Build faster web apps using Node.js, Svelte.js, and WebAssembly*. [ISBN](./ISBN_(identifier)) [978-1838821098](./Special:BookSources/978-1838821098).
13. [↑](./Single-page_application#cite_ref-13) ["Enhance"](https://github.com/enhance-dev). *[GitHub](./GitHub)*.
14. [↑](./Single-page_application#cite_ref-14) ["Astro framework"](https://github.com/withastro/astro). *[GitHub](./GitHub)*.
15. [↑](./Single-page_application#cite_ref-15) ["Fresh"](https://github.com/denoland/fresh). *[GitHub](./GitHub)*.
16. [↑](./Single-page_application#cite_ref-16) ["Real-Time Monitoring using AJAX and WebSockets"](http://www.computer.org/csdl/proceedings/ecbs/2013/4991/00/4991a110-abs.html). *www.computer.org*. Retrieved June 1, 2016.
17. [↑](./Single-page_application#cite_ref-17) ["Server-Sent Events"](http://www.w3.org/TR/eventsource/). W3C. July 17, 2013.
18. [↑](./Single-page_application#cite_ref-18) ["Unhosted web apps"](https://unhosted.org/).
19. [↑](./Single-page_application#cite_ref-spimanifesto_19-0) ["The Single Page Interface Manifesto"](https://itsnat.sourceforge.net/php/spim/spi_manifesto_en.php). Retrieved April 25, 2014.
20. [↑](./Single-page_application#cite_ref-20) ["Derby"](http://derbyjs.com/). Retrieved December 11, 2011.
21. [↑](./Single-page_application#cite_ref-21) ["Sails.js"](https://github.com/balderdashy/sails). *[GitHub](./GitHub)*. Retrieved February 20, 2013.
22. [↑](./Single-page_application#cite_ref-22) ["Tutorial: Single Page Interface Web Site With ItsNat"](https://itsnat.sourceforge.net/index.php?_page=support.tutorial.spi_site). Retrieved January 13, 2011.
23. [↑](./Single-page_application#cite_ref-23) [HTML5](./HTML5)
24. [↑](./Single-page_application#cite_ref-24) ["What the user sees, what the crawler sees"](https://developers.google.com/webmasters/ajax-crawling/docs/learn-more). Retrieved January 6, 2014. the browser can execute JavaScript and produce content on the fly - the crawler cannot
25. [↑](./Single-page_application#cite_ref-doogledevelopers_25-0) ["Making Ajax Applications Crawlable"](https://developers.google.com/webmasters/ajax-crawling/). Retrieved January 6, 2014. Historically, Ajax applications have been difficult for search engines to process because Ajax content is produced
26. [↑](./Single-page_application#cite_ref-26) ["Proposal for making AJAX crawlable"](http://googlewebmastercentral.blogspot.com/2009/10/proposal-for-making-ajax-crawlable.html). Google. October 7, 2009. Retrieved July 13, 2011.
27. [↑](./Single-page_application#cite_ref-27) ["(Specifications) Making AJAX Applications Crawlable"](https://developers.google.com/webmasters/ajax-crawling/). Google Inc. Retrieved March 4, 2013.
28. [↑](./Single-page_application#cite_ref-Tennison2_28-0) ["Hash URIs"](http://www.w3.org/QA/2011/05/hash_uris.html). *W3C Blog*. May 12, 2011. Retrieved July 13, 2011.
29. [↑](./Single-page_application#cite_ref-29) ["Deprecating our AJAX crawling scheme"](https://webmasters.googleblog.com/2015/10/deprecating-our-ajax-crawling-scheme.html). *Official Google Webmaster Central Blog*. Retrieved February 23, 2017.
30. [↑](./Single-page_application#cite_ref-DynamicRendering_30-0) ["Implement dynamic rendering"](https://developers.google.com/search/docs/guides/dynamic-rendering). *Google Search Central*. October 13, 2018. Retrieved January 7, 2021.
31. [↑](./Single-page_application#cite_ref-DynamicRenderingWorkaround_31-0) ["Dynamic rendering as a workaround"](https://developers.google.com/search/docs/crawling-indexing/javascript/dynamic-rendering). *Google Search Central*. March 18, 2024. Retrieved July 2, 2024.
32. [↑](./Single-page_application#cite_ref-32) ["Fix a single-page app for Google Search"](https://codelabs.developers.google.com/codelabs/making-a-single-page-app-search-friendly). *Google Codelabs*. Retrieved 2021-12-15.
33. [1](./Single-page_application#cite_ref-Holmes2015_33-0) [2](./Single-page_application#cite_ref-Holmes2015_33-1) [3](./Single-page_application#cite_ref-Holmes2015_33-2) Holmes, Simone (2015). *Getting MEAN with Mongo, Express, Angular, and Node*. Manning Publications. [ISBN](./ISBN_(identifier)) [978-1-6172-9203-3](./Special:BookSources/978-1-6172-9203-3)
34. [↑](./Single-page_application#cite_ref-34) ["Single Page Applications (SPA)"](https://appcheck-ng.com/single-page-applications/). *Appcheck Ltd*.

 

## External links

 
- [Migrating Multi-page Web Applications to Single-page Ajax Interfaces (Delft University of Technology)](https://arxiv.org/abs/cs/0610094)
- [Dynamic Rendering](https://developers.google.com/search/docs/guides/dynamic-rendering)

 
| vteWeb interfaces |
| --- |
| Server-sideProtocolsHTTPv2v3EncryptionWebDAVCGISCGIFCGIAJPWSRPWebSocketServer APIsC NSAPIC ASAPIC ISAPICOM ASPJakarta ServletcontainerCLI OWINASP.NET HandlerPython WSGIPython ASGIRuby RackJavaScript JSGIPerl PSGIPortletcontainerApache modulesmod_includemod_jkmod_lispmod_monomod_parrotmod_perlmod_phpmod_proxymod_pythonmod_wsgimod_rubyPhusion PassengerTopicsWeb servicevs.Web resourceWOAvs.ROAOpen APIWebhookApplication servercomparisonScripting | Server-side | Protocols | HTTPv2v3EncryptionWebDAVCGISCGIFCGIAJPWSRPWebSocket | Server APIs | C NSAPIC ASAPIC ISAPICOM ASPJakarta ServletcontainerCLI OWINASP.NET HandlerPython WSGIPython ASGIRuby RackJavaScript JSGIPerl PSGIPortletcontainer | Apache modules | mod_includemod_jkmod_lispmod_monomod_parrotmod_perlmod_phpmod_proxymod_pythonmod_wsgimod_rubyPhusion Passenger | Topics | Web servicevs.Web resourceWOAvs.ROAOpen APIWebhookApplication servercomparisonScripting |
| Server-side |
| Protocols | HTTPv2v3EncryptionWebDAVCGISCGIFCGIAJPWSRPWebSocket |
| Server APIs | C NSAPIC ASAPIC ISAPICOM ASPJakarta ServletcontainerCLI OWINASP.NET HandlerPython WSGIPython ASGIRuby RackJavaScript JSGIPerl PSGIPortletcontainer |
| Apache modules | mod_includemod_jkmod_lispmod_monomod_parrotmod_perlmod_phpmod_proxymod_pythonmod_wsgimod_rubyPhusion Passenger |
| Topics | Web servicevs.Web resourceWOAvs.ROAOpen APIWebhookApplication servercomparisonScripting |
| Client-sideBrowser APIsC NPAPILiveConnectXPConnectC NPRuntimeC PPAPINaClActiveXBHOXBAPWeb APIsWHATWGAudioCanvasDOMSSEVideoWebSocketsWeb messagingWeb storageWeb workerXMLHttpRequestW3CDOM eventsEMEFileGeolocationIndexedDBMSESVGWebAssemblyWebAuthnWebGPUWebRTCWebXRKhronosWebCLWebGLOthersGearsWeb SQL Database(formerly W3C)WebUSBTopicsAjaxandRemote scriptingvs.DHTMLBrowser extensionCross-site scriptingandCORSHydrationMashupPersistent dataWeb IDLScripting | Client-side | Browser APIs | C NPAPILiveConnectXPConnectC NPRuntimeC PPAPINaClActiveXBHOXBAP | Web APIs | WHATWGAudioCanvasDOMSSEVideoWebSocketsWeb messagingWeb storageWeb workerXMLHttpRequestW3CDOM eventsEMEFileGeolocationIndexedDBMSESVGWebAssemblyWebAuthnWebGPUWebRTCWebXRKhronosWebCLWebGLOthersGearsWeb SQL Database(formerly W3C)WebUSB | WHATWG | AudioCanvasDOMSSEVideoWebSocketsWeb messagingWeb storageWeb workerXMLHttpRequest | W3C | DOM eventsEMEFileGeolocationIndexedDBMSESVGWebAssemblyWebAuthnWebGPUWebRTCWebXR | Khronos | WebCLWebGL | Others | GearsWeb SQL Database(formerly W3C)WebUSB | Topics | AjaxandRemote scriptingvs.DHTMLBrowser extensionCross-site scriptingandCORSHydrationMashupPersistent dataWeb IDLScripting |
| Client-side |
| Browser APIs | C NPAPILiveConnectXPConnectC NPRuntimeC PPAPINaClActiveXBHOXBAP |
| Web APIs | WHATWGAudioCanvasDOMSSEVideoWebSocketsWeb messagingWeb storageWeb workerXMLHttpRequestW3CDOM eventsEMEFileGeolocationIndexedDBMSESVGWebAssemblyWebAuthnWebGPUWebRTCWebXRKhronosWebCLWebGLOthersGearsWeb SQL Database(formerly W3C)WebUSB | WHATWG | AudioCanvasDOMSSEVideoWebSocketsWeb messagingWeb storageWeb workerXMLHttpRequest | W3C | DOM eventsEMEFileGeolocationIndexedDBMSESVGWebAssemblyWebAuthnWebGPUWebRTCWebXR | Khronos | WebCLWebGL | Others | GearsWeb SQL Database(formerly W3C)WebUSB |
| WHATWG | AudioCanvasDOMSSEVideoWebSocketsWeb messagingWeb storageWeb workerXMLHttpRequest |
| W3C | DOM eventsEMEFileGeolocationIndexedDBMSESVGWebAssemblyWebAuthnWebGPUWebRTCWebXR |
| Khronos | WebCLWebGL |
| Others | GearsWeb SQL Database(formerly W3C)WebUSB |
| Topics | AjaxandRemote scriptingvs.DHTMLBrowser extensionCross-site scriptingandCORSHydrationMashupPersistent dataWeb IDLScripting |
| Related topicsFrontend and backendMicroservicesRESTGraphQLPush technologySolution stackWeb pageStaticDynamicWeb standardsWeb API securityWeb applicationRichSingle-pageProgressiveWeb framework | Related topics | Frontend and backendMicroservicesRESTGraphQLPush technologySolution stackWeb pageStaticDynamicWeb standardsWeb API securityWeb applicationRichSingle-pageProgressiveWeb framework |
| Related topics |
| Frontend and backendMicroservicesRESTGraphQLPush technologySolution stackWeb pageStaticDynamicWeb standardsWeb API securityWeb applicationRichSingle-pageProgressiveWeb framework |