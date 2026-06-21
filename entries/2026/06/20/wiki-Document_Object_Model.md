---
source: sources/wiki-Document_Object_Model.md
source_url: https://en.wikipedia.org/wiki/Document_Object_Model
---

## Document Object Model (DOM): Architecture, Standards, and API

The Document Object Model (DOM) is a cross-platform, language-independent API that represents HTML or XML documents as a tree structure of node objects. It provides programmatic access to read and modify document structure, style, and content. Standardized initially by the W3C and now maintained as a living standard by WHATWG, the DOM is the foundational interface between scripting languages (primarily JavaScript) and web documents rendered in browsers.

## Key Concepts

- **DOM as a tree**: Documents are represented as a hierarchical tree of nodes, with the Document as the root node. Each branch ends in a node containing objects.
- **Node types**: Document nodes, element nodes, attribute nodes, text nodes, and comment nodes.
- **Text nodes are always leaf nodes** — they cannot have children or attributes.
- **Attributes are properties** of element nodes, not separate child nodes in the tree representation.
- **Language-independent**: The DOM is not tied to JavaScript — it is a platform- and language-neutral interface, though JavaScript is its most common consumer.
- **DOM does not mandate a tree implementation**: The spec defines a logical model; browsers may use any internal representation. Microsoft Edge, for example, modernized away from a traditional tree.
- **Event model**: Nodes can have event handlers (listeners) attached; events trigger their execution.
- **Living standard**: WHATWG maintains the DOM as a living document; W3C publishes periodic stable snapshots of it.
- **DOM exists in memory**: Creating DOM structures programmatically does not display them — they must be appended to the document body to render.

## Commands and Syntax

**Accessing elements:**
```javascript
document.getElementById("id")        // DOM Level 2+
document.myForm.myInput               // Legacy DOM (Level 0)
document.forms[0].elements[0]         // Legacy DOM sequential index
```

**Creating and appending nodes:**
```javascript
var root = document.createElement("root");
var child = document.createElement("child");
root.appendChild(child);
```

**Using innerHTML (string-based DOM construction):**
```javascript
document.getElementById("root").innerHTML = "<child></child>";
```

**Core DOM API methods and properties:**
- `getElementById()` — retrieve element by ID
- `createElement()` — create a new element node
- `appendChild()` — add a child node
- `innerHTML` — get/set HTML content as a string

**DOM tree representation of HTML:**
```
Document (root)
  └─ html
       ├─ head
       │    └─ title
       │         └─ "My Website"
       └─ body
            ├─ h1
            │    └─ "Welcome to DOM"
            └─ p
                 └─ "This is my website."
```

## Relationships

- **JavaScript**: Primary language for DOM manipulation; the browser creates the DOM when a page loads, and JavaScript interacts with it to create dynamic pages.
- **HTML/XML**: The DOM represents parsed HTML or XML documents; HTML5 replaced parts of the DOM Level 2 HTML module.
- **CSS**: DOM Level 2 introduced CSS support; DOM methods can change styles programmatically.
- **Layout engines**: Blink (Chrome, Edge, Opera), WebKit (Safari), Gecko (Firefox), and the discontinued Trident (IE) all parse HTML into DOM structures with varying standards compliance.
- **ECMAScript**: Standardization of ECMAScript prompted the W3C to begin formalizing the DOM specification.
- **DHTML**: Dynamic HTML drove the need for DOM extensions beyond Legacy DOM, though incompatible implementations by Netscape and Microsoft created the "Intermediate DOM."
- **Shadow DOM / Virtual DOM**: Related concepts — Shadow DOM provides encapsulated DOM subtrees; Virtual DOM (used by React, etc.) is an abstraction layer over the real DOM for performance.
- **XPath**: DOM Level 3 added XPath support for navigating XML documents.
- **Frameworks (jQuery, React, Vue, Angular, Svelte)**: Abstract over raw DOM manipulation for efficiency and developer ergonomics.

## Exam-Relevant Points

- **DOM Level 0 (Legacy DOM)**: No formal standard; limited to form, link, and image elements; supported client-side validation and simple interactivity.
- **DOM Level 1** (W3C Recommendation, late 1998): Complete model for entire HTML/XML documents, including modification capability.
- **DOM Level 2** (late 2000): Introduced `getElementById`, the event model, XML namespace support, and CSS support.
- **DOM Level 3** (April 2004): Added XPath, keyboard event handling, and XML serialization.
- **DOM Level 4** (2015, retired November 2020): Last numbered W3C version before transition to WHATWG living standard snapshots.
- **Five node types in HTML DOM**: document, element, attribute, text, comment.
- **W3C vs. WHATWG**: W3C DOM Working Group disbanded in 2004; WHATWG maintains the living standard; W3C now publishes snapshots (e.g., DOM 2020-06 published September 2021).
- **Implementations are typically buffered** because the DOM supports arbitrary navigation (parent, sibling) and modification.
- **Key DOM libraries**: libxml2, MSXML, Xerces (C++/Java/Perl), xml.dom (Python), Domino (Node.js, used by MediaWiki).
- **Browser wars context**: Incompatible Netscape and Microsoft DHTML DOM extensions in 1997 (Intermediate DOM) drove the need for standardization.
- **DOM is not inherently visual**: It is a logical model that can exist entirely in memory without rendering; a DOM can also be created programmatically without originating from a serialized document.
