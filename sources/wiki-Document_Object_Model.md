---
source: https://en.wikipedia.org/wiki/Document_Object_Model
fetched: 2026-06-20
---

Computer document convention 
| Document Object Model (DOM) |
| --- |
| Example of DOM hierarchy in an HTML document |
| Abbreviation | DOM |
| Latest version | DOM4[1]November19, 2015;10 years ago(2015-11-19) |
| Organization | World Wide Web Consortium,WHATWG |
| Base standards | WHATWG DOM Living StandardW3C DOM4 |

 
| HTML |
| --- |
|  |
| HTML and variants |
| Dynamic HTMLHTML5XHTMLBasicMobile Profile |
| HTML elements and attributes |
| HTML elementarticleaudioblinkcanvasdiv and spanmarqueemetavideoHTML attributealt attributeHTML frame |
| Editing |
| HTML editorText editor |
| Character encodings and language |
| Character encodingsCharacter entity references (named characters)UnicodeLanguage code |
| Document and browser models |
| Document Object ModelBrowser Object ModelStyle sheetsCSSFont familyWeb colors |
| Client-side scripting and APIs |
| JavaScriptWebCLHTMX |
| Graphics and Web3D technology |
| Web3DWebGLWebGPUWebXRW3CValidatorWHATWGQuirks modeWeb storageRendering engine |
| Comparisons |
| Document markup languagesComparison of browser engines |
| vte |

 

The **Document Object Model** (**DOM**) is a [cross-platform](./Cross-platform)[[2]](./Document_Object_Model#cite_note-:0-2) and [language-independent](./Language-independent_specification) [API](./API) that treats an [HTML](./HTML) or [XML](./XML) document as a [tree structure](./Tree_structure) wherein each [node](./Node_(computer_science)) is an [object](./Object_(computer_science)) representing a part of the document. The DOM represents a document with a logical tree. Each branch of the tree ends in a node, and each node contains objects. DOM methods allow programmatic access to the tree; with them one can change the structure, style or content of a document.[[2]](./Document_Object_Model#cite_note-:0-2) Nodes can have [event handlers](./Event_handler) (also known as event listeners) attached to them. Once an event is triggered, the event handlers get executed.[[3]](./Document_Object_Model#cite_note-Introduction-3)

 

The principal standardization of the DOM was handled by the [World Wide Web Consortium](./World_Wide_Web_Consortium) (W3C), which last developed a recommendation in 2004. [WHATWG](./WHATWG) took over the development of the standard, publishing it as a [living document](./Living_document). The W3C now publishes stable snapshots of the WHATWG standard.

 

In HTML DOM (Document Object Model), every element is a node[*[clarification needed](./Wikipedia:Please_clarify)*]:[[4]](./Document_Object_Model#cite_note-4)

 
- A document is a document node.
- All HTML elements are element nodes.
- All HTML attributes are attribute nodes.
- Text inserted into HTML elements are text nodes.
- Comments are comment nodes.

 

## History

 

The history of the Document Object Model is intertwined with the history of the "[browser wars](./Browser_wars)" of the late 1990s between [Netscape Navigator](./Netscape_Navigator) and [Microsoft Internet Explorer](./Microsoft_Internet_Explorer), as well as with that of [JavaScript](./JavaScript) and [JScript](./JScript), the first [scripting languages](./Scripting_language) to be widely [implemented](./Implementation) in the [JavaScript engines](./JavaScript_engine) of [web browsers](./Web_browser).[*[citation needed](./Wikipedia:Citation_needed)*]

 

JavaScript was released by [Netscape Communications](./Netscape_Communications) in 1995 within Netscape Navigator 2.0. Netscape's competitor, [Microsoft](./Microsoft), released [Internet Explorer 3.0](./Internet_Explorer_3) the following year with a reimplementation of JavaScript called JScript. JavaScript and JScript let [web developers](./Web_developer) create web pages with [client-side](./Client-side) interactivity. The limited facilities for detecting user-generated [events](./Event_(computing)) and modifying the HTML document in the first generation of these languages eventually became known as "DOM Level 0" or "Legacy DOM." No independent standard was developed for DOM Level 0, but it was partly described in the specifications for [HTML 4](./HTML4).

 

Legacy DOM was limited in the kinds of [elements](./HTML_element) that could be accessed. [Form](./Form_(web)), [link](./Hyperlink) and image elements could be referenced with a hierarchical name that began with the root document object. A hierarchical name could make use of either the names or the [sequential index](./Sequence) of the traversed elements. For example, a [form input element](./Text_box) could be accessed as either `document.myForm.myInput` or `document.forms[0].elements[0]`.

 

The Legacy DOM enabled client-side form validation and simple interface interactivity like creating [tooltips](./Tooltip).

 

In 1997, Netscape and Microsoft released version 4.0 of Netscape Navigator and Internet Explorer respectively, adding support for [Dynamic HTML](./Dynamic_HTML) (DHTML) functionality enabling changes to a loaded HTML document. DHTML required extensions to the rudimentary document object that was available in the Legacy DOM implementations. Although the Legacy DOM implementations were largely compatible since JScript was based on JavaScript, the DHTML DOM extensions were developed in parallel by each browser maker and remained incompatible. These versions of the DOM became known as the "Intermediate DOM".

 

After the standardization of [ECMAScript](./ECMAScript), the [W3C](./World_Wide_Web_Consortium) DOM Working Group began drafting a standard DOM specification. The completed specification, known as "DOM Level 1", became a W3C Recommendation in late 1998. By 2005, large parts of W3C DOM were well-supported by common ECMAScript-enabled browsers, including [Internet Explorer 6](./Internet_Explorer_6) (from 2001), [Opera](./Opera_(web_browser)), [Safari](./Safari_(web_browser)) and [Gecko](./Gecko_(layout_engine))-based browsers (like [Mozilla](./Mozilla_Application_Suite), [Firefox](./Mozilla_Firefox), [SeaMonkey](./SeaMonkey) and [Camino](./Camino_(web_browser))).

 

## Standards

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/0/0d/WHATWG_DOM.png/250px-WHATWG_DOM.png)](./File:WHATWG_DOM.png)WHATWG DOM 

The [W3C](./W3C) DOM Working Group published its final recommendation and subsequently disbanded in 2004. Development efforts migrated to the [WHATWG](./WHATWG), which continues to maintain a living standard.[[5]](./Document_Object_Model#cite_note-5) In 2009, the Web Applications group reorganized DOM activities at the W3C.[[6]](./Document_Object_Model#cite_note-6) In 2013, due to a lack of progress and the impending release of [HTML5](./HTML5), the DOM Level 4 specification was reassigned to the [HTML Working Group](./HTML_Working_Group) to expedite its completion.[[7]](./Document_Object_Model#cite_note-7) Meanwhile, in 2015, the Web Applications group was disbanded and DOM stewardship passed to the Web Platform group.[[8]](./Document_Object_Model#cite_note-8) Beginning with the publication of DOM Level 4 in 2015, the W3C creates new recommendations based on snapshots of the WHATWG standard.

 
- DOM Level 1 provided a complete model for an entire HTML or [XML](./XML) document, including the means to change any portion of the document.
- DOM Level 2 was published in late 2000. It introduced the `getElementById` function as well as an [event model](./DOM_Events) and support for [XML namespaces](./XML_namespace) and CSS.
- DOM Level 3, published in April 2004, added support for [XPath](./XPath) and keyboard [event handling](./Event_handling), as well as an interface for [serializing](./Serialization) documents as XML.
- HTML5 was published in October 2014.  Part of HTML5 had replaced DOM Level 2 HTML module.
- DOM Level 4 was published in 2015 and retired in November 2020.[[9]](./Document_Object_Model#cite_note-9)
- [DOM 2020-06](https://dom.spec.whatwg.org/review-drafts/2020-06/) was published in September 2021 as a W3C Recommendation.[[10]](./Document_Object_Model#cite_note-10) It is a snapshot of the WHATWG living standard.

 

## Applications

 

### Web browsers

 

To [render](./Web_browser_engine) a document such as a HTML page, most web browsers use an internal model similar to the DOM. The nodes of every document are organized in a [tree structure](./Tree_structure), called the *DOM tree*, with the topmost node named as "Document object". When an HTML page is rendered in browsers, the browser downloads the HTML into local memory and automatically parses it to display the page on screen. However, the DOM does not necessarily need to be represented as a tree,[[11]](./Document_Object_Model#cite_note-Level3-Introduction-11) and some browsers have used other internal models.[[12]](./Document_Object_Model#cite_note-Modernizing-Dom-12)

 

### JavaScript

 

When a web page is loaded, the browser creates a Document Object Model of the page, which is an object oriented representation of an HTML document that acts as an interface between JavaScript and the document itself. This allows the creation of [dynamic web pages](./Dynamic_web_page),[[13]](./Document_Object_Model#cite_note-13) because within a page JavaScript can:

 
- add, change, and remove any of the HTML elements and attributes
- change any of the CSS styles
- react to all the existing events
- create new events

 

## DOM tree structure

 

A Document Object Model (DOM) tree is a hierarchical representation of an HTML or [XML](./XML) document. It consists of a root node, which is the document itself, and a series of child nodes that represent the elements, attributes, and text content of the document. Each node in the tree has a parent node, except for the root node, and can have multiple child nodes.

 

### Elements as nodes

Elements in an HTML or XML document are represented as nodes in the DOM tree. Each element node has a tag name and attributes, and can contain other element nodes or text nodes as children. For example, an HTML document with the following structure:

```
<html>
  <head>
    <title>My Website</title>
  </head>
  <body>
    <h1>Welcome to DOM</h1>
    <p>This is my website.</p>
  </body>
</html>

```

will be represented in the DOM tree as:

```
- Document (root)
  - html
    - head
      - title
        - "My Website"
    - body
      - h1
        - "Welcome to DOM"
      - p
        - "This is my website."

```
 

### Text nodes

 

Text content within an element is represented as a text node in the DOM tree. Text nodes do not have attributes or child nodes and are therefore always leaf nodes in the tree. For example, the text content "My Website" in the title element and "Welcome" in the h1 element are both represented as text nodes.

 

### Attributes as properties

Attributes of an element are represented as properties of the element node in the DOM tree. For example, an element with the following HTML:

```
<a href="https://example.com">Link</a>

```

will be represented in the DOM tree as:

```
- a
  - href: "https://example.com"
  - "Link"

```
 

## Manipulating the DOM tree

The DOM tree can be manipulated using JavaScript or other programming languages. Common tasks include navigating the tree, adding, removing, and modifying nodes, and getting and setting the properties of nodes. The DOM API provides a set of methods and properties to perform these operations, such as `getElementById`, `createElement`, `appendChild`, and `innerHTML`.

```
// Create the root element
var root = document.createElement("root");

// Create a child element
var child = document.createElement("child");

// Add the child element to the root element
root.appendChild(child);

```

Another way to create a DOM structure is using the innerHTML property to insert HTML code as a string, creating the elements and children in the process. For example:

```
document.getElementById("root").innerHTML = "<child></child>";

```

Another method is to use a JavaScript library or framework such as [jQuery](./JQuery), [AngularJS](./AngularJS), [React](./React_(JavaScript_library)), [Vue.js](./Vue.js), [Svelte](./Svelte), etc. These libraries provide an efficient way to create, manipulate and interact with the DOM.

 

It is also possible to create a DOM structure from an XML or JSON data, using JavaScript methods to parse the data and create the nodes accordingly.

 

Creating a DOM structure does not necessarily mean that it will be displayed in the web page, it only exists in memory and should be appended to the document body or a specific container to be rendered.

 

In summary, creating a DOM structure involves creating individual nodes and organizing them in a hierarchical structure using JavaScript or other programming languages, and it can be done using several methods depending on the use case and the developer's preference.

 

## Implementations

 

Because the DOM supports navigation in any direction (e.g., parent and previous sibling) and allows for arbitrary modifications, implementations typically buffer the document.[[14]](./Document_Object_Model#cite_note-14) However, a DOM need not originate in a serialized document at all, but can be created in place with the DOM API. And even before the idea of the DOM originated, there were implementations of equivalent structure with persistent disk representation and rapid access, for example [DynaText](./DynaText)'s model disclosed in [[15]](./Document_Object_Model#cite_note-15) and various database approaches.

 

### Layout engines

 

Web browsers rely on [layout engines](./Web_browser_engine) to parse HTML into a DOM. Some layout engines, such as [Trident/MSHTML](./Trident_(layout_engine)), are associated primarily or exclusively with a particular browser, such as Internet Explorer. Others, including [Blink](./Blink_(layout_engine)), [WebKit](./WebKit), and [Gecko](./Gecko_(layout_engine)), are shared by a number of browsers, such as [Google Chrome](./Google_Chrome), [Opera](./Opera_(web_browser)), [Safari](./Safari_(web_browser)), and [Firefox](./Firefox). The different layout engines implement the DOM standards to varying degrees of compliance.

 

### Libraries

 

DOM implementations:

 
- [libxml2](./Libxml2)
- [MSXML](./MSXML)
- [Xerces](./Apache_Xerces) is a collection of DOM implementations written in C++, Java and Perl
- [xml.dom](https://docs.python.org/3/library/xml.dom.html) for [Python](./Python_(programming_language))
- XML for <SCRIPT> is a JavaScript-based DOM implementation[[16]](./Document_Object_Model#cite_note-16)
- [PHP.Gt DOM](https://github.com/PhpGt/Dom) is a server-side DOM implementation based on [libxml2](./Libxml2) and brings DOM level 4 compatibility[[17]](./Document_Object_Model#cite_note-17) to the [PHP](./PHP) programming language
- [Domino](https://github.com/fgnass/domino/) is a Server-side (Node.js) DOM implementation based on Mozilla's dom.js. Domino is used in the [MediaWiki](./MediaWiki) stack with Visual Editor.
- [SimpleHtmlDom](https://github.com/wooly905/SimpleHtmlDom/) is a simple HTML document object model in C#, which can generate HTML string programmatically.

 

APIs that expose DOM implementations:

 
- [JAXP](./Java_API_for_XML_Processing) (Java API for XML Processing, `org.w3c.dom`) is an API for accessing DOM providers
- [Lazarus](./Lazarus_(IDE)) ([Free Pascal](./Free_Pascal) IDE) contains two variants of the DOM - with UTF-8 and ANSI format

 

Inspection tools:

 
- [DOM Inspector](./DOM_Inspector) is a web developer tool

 

## See also

 
- [Shadow DOM](./Shadow_DOM)
- [Virtual DOM](./Virtual_DOM)

 

## References

  
1. [↑](./Document_Object_Model#cite_ref-1) All versioning refers to W3C DOM only.
2. [1](./Document_Object_Model#cite_ref-:0_2-0) [2](./Document_Object_Model#cite_ref-:0_2-1) ["Document Object Model (DOM): definition, structure and example"](https://www.ionos.com/digitalguide/websites/web-development/an-introduction-to-the-document-object-model-dom/). *IONOS Digitalguide*. Retrieved 2022-04-21.
3. [↑](./Document_Object_Model#cite_ref-Introduction_3-0) ["Document Object Model (DOM)"](https://www.w3.org/DOM/#what). W3C. Retrieved 2012-01-12. The Document Object Model is a platform- and language-neutral interface that will allow programs and scripts to dynamically access and update the content, structure and style of documents.
4. [↑](./Document_Object_Model#cite_ref-4) ["JavaScript HTML DOM"](https://www.w3schools.com/js/js_htmldom.asp).
5. [↑](./Document_Object_Model#cite_ref-5) ["DOM Standard"](https://dom.spec.whatwg.org/). Retrieved 23 September 2016.
6. [↑](./Document_Object_Model#cite_ref-6) ["W3C Document Object Model"](https://www.w3.org/DOM/). Retrieved 23 September 2016.
7. [↑](./Document_Object_Model#cite_ref-7) (plh@w3.org), Philippe Le Hegaret. ["New Charter for the HTML Working Group from Philippe Le Hegaret on 2013-09-30 (public-html-admin@w3.org from September 2013)"](https://lists.w3.org/Archives/Public/public-html-admin/2013Sep/0129.html). Retrieved 23 September 2016.`{{cite web}}`:  CS1 maint: numeric names: authors list ([link](./Category:CS1_maint:_numeric_names:_authors_list))
8. [↑](./Document_Object_Model#cite_ref-8) ["PubStatus - WEBAPPS"](https://web.archive.org/web/20170610233948/https://www.w3.org/2008/webapps/wiki/PubStatus). Archived from [the original](https://www.w3.org/2008/webapps/wiki/PubStatus) on 10 June 2017. Retrieved 23 September 2016.
9. [↑](./Document_Object_Model#cite_ref-9) ["W3C DOM4 publication history"](https://www.w3.org/standards/history/dom40/). 3 November 2020. Retrieved 10 August 2024.
10. [↑](./Document_Object_Model#cite_ref-10) ["DOM publication history"](https://www.w3.org/standards/history/dom/). 28 September 2021. Retrieved 10 August 2024.
11. [↑](./Document_Object_Model#cite_ref-Level3-Introduction_11-0) ["What is the Document Object Model?"](https://www.w3.org/TR/2004/REC-DOM-Level-3-Core-20040407/introduction.html). W3C. Retrieved 2021-09-12. However, the DOM does not specify that documents must be implemented as a tree or a grove, nor does it specify how the relationships among objects be implemented. The DOM is a logical model that may be implemented in any convenient manner.
12. [↑](./Document_Object_Model#cite_ref-Modernizing-Dom_12-0) ["Modernizing the DOM tree in Microsoft Edge"](https://blogs.windows.com/msedgedev/2017/04/19/modernizing-dom-tree-microsoft-edge/). Microsoft. 19 April 2017. Retrieved 2021-09-12.
13. [↑](./Document_Object_Model#cite_ref-13) ["JavaScript HTML DOM"](https://www.w3schools.com/js/js_htmldom.asp). Retrieved 23 September 2016.
14. [↑](./Document_Object_Model#cite_ref-14) Kogent Solutions Inc. (2008). [*Ajax Black Book, New Edition (With Cd)*](https://books.google.com/books?id=HuSQGrRY7F4C). Dreamtech Press. p. 40. [ISBN](./ISBN_(identifier)) [978-8177228380](./Special:BookSources/978-8177228380).
15. [↑](./Document_Object_Model#cite_ref-15) [USA Expired 5557722A](https://worldwide.espacenet.com/textdoc?DB=EPODOC&IDX=USA5557722A), Steven DeRose & Jeffrey Vogel, "Data processing system and method for representing, generating a representation of and random access rendering of electronic documents", published 1996-09-17 
16. [↑](./Document_Object_Model#cite_ref-16) ["XML for <script> Cross Platform XML Parser in JavaScript"](https://xmljs.sourceforge.net/). Retrieved 23 September 2016.
17. [↑](./Document_Object_Model#cite_ref-17) ["The modern DOM API for PHP 7 projects"](https://php.gt/dom#features-at-a-glance). 5 December 2021.

 

### General references

 
- Flanagan, David (2006). [*JavaScript: The Definitive Guide*](https://archive.org/details/javascript00libg_297). O'Reilly & Associates. pp. [312](https://archive.org/details/javascript00libg_297/page/n310)–313. [ISBN](./ISBN_(identifier)) [0-596-10199-6](./Special:BookSources/0-596-10199-6).
- Koch, Peter-Paul (May 14, 2001). ["The Document Object Model: an Introduction"](https://web.archive.org/web/20170427220310/http://www.digital-web.com/articles/the_document_object_model/). *Digital Web Magazine*. Archived from [the original](http://www.digital-web.com/articles/the_document_object_model/) on April 27, 2017. Retrieved January 10, 2009.
- Le Hégaret, Philippe (2002). ["The W3C Document Object Model (DOM)"](https://www.w3.org/2002/07/26-dom-article.html). World Wide Web Consortium. Retrieved January 10, 2009.
- Guisset, Fabian. ["What does each DOM Level bring?"](https://web.archive.org/web/20130302191641/https://developer.mozilla.org/en/docs/DOM_Levels). *Mozilla Developer Center*. Mozilla Project. Archived from [the original](https://developer.mozilla.org/en/docs/DOM_Levels) on March 2, 2013. Retrieved January 10, 2009.

 

## External links

   [![Wikimedia Commons logo](//upload.wikimedia.org/wikipedia/en/thumb/4/4a/Commons-logo.svg/40px-Commons-logo.svg.png)](./File:Commons-logo.svg) Wikimedia Commons has media related to [document object models](https://commons.wikimedia.org/wiki/Category:Document%20object%20models).  
- [DOM Living Standard](https://dom.spec.whatwg.org/) by the WHATWG
- [Original W3C DOM hub](https://www.w3.org/DOM/) by the W3C DOM Working Group (outdated)
- [Latest snapshots of the WHATWG living standard](https://www.w3.org/standards/history/dom) published by the W3C HTML Working Group
- [Web Platform Working Group](https://www.w3.org/WebPlatform/WG/) (current steward of W3C DOM)

 
| vteJavaScript |
| --- |
| Code analysis | ESLintJSHintJSLint |
| Subsets,* supersets | JS++Source*TypeScript(ArkTS) |
| Transpilers | AtScriptBabelClojureScriptCoffeeScriptDartElmEmscriptenGoogle Closure CompilerGoogle Web ToolkitHaxeLiveScriptMorfikNimOpaPureScriptReScriptWebSharper |
| Concepts | JavaScript libraryJavaScript syntax |
| Debuggers | Chrome DevToolsFirefoxInspector (formerlyFirebug)Komodo IDESafariWeb Inspector |
| Documentation generators | JSDoc |
| Editors (comparison) | AceCloud9 IDEAtomCodeMirrorBracketsLight TablePhpStormOrionVisual StudioVisual Studio ExpressVisual Studio CodeVisual Studio Team ServicesVim |
| Engines | List of JavaScript engines |
| Frameworks | Comparison of JavaScript frameworksList of JavaScript libraries |
| Relatedtechnologies | AjaxAssemblyScriptasm.jsCSSDOMHTMLHTML5JSONWebAssemblyWebAuthn |
| Package managers | npmpnpmyarnBun |
| Module bundlers | BunesbuildViteWebpack |
| Server-side | Active Server PagesBunCommonJSDenoJSGINode.js |
| Unit testingframeworks (list) | JasmineMochaQUnit |
| People | Douglas CrockfordRyan DahlBrendan EichJohn ResigJesse James Garrett |
| OutlineIndexWikibook |

 
| vteWeb browsers |
| --- |
| Features, standards & protocolsFeaturesBookmarksExtensionsPrivacy modeWeb standardsHTMLv5CSSDOMJavaScriptWebAssemblyWeb storageIndexedDBWebGLWebGPUProtocolsHTTPEncryptionCookiesthird-partyOCSPWebRTCWebSocket | Features, standards & protocols | FeaturesBookmarksExtensionsPrivacy modeWeb standardsHTMLv5CSSDOMJavaScriptWebAssemblyWeb storageIndexedDBWebGLWebGPUProtocolsHTTPEncryptionCookiesthird-partyOCSPWebRTCWebSocket | Features | BookmarksExtensionsPrivacy mode | Web standards | HTMLv5CSSDOMJavaScriptWebAssemblyWeb storageIndexedDBWebGLWebGPU | Protocols | HTTPEncryptionCookiesthird-partyOCSPWebRTCWebSocket |
| Features, standards & protocols |
| FeaturesBookmarksExtensionsPrivacy modeWeb standardsHTMLv5CSSDOMJavaScriptWebAssemblyWeb storageIndexedDBWebGLWebGPUProtocolsHTTPEncryptionCookiesthird-partyOCSPWebRTCWebSocket | Features | BookmarksExtensionsPrivacy mode | Web standards | HTMLv5CSSDOMJavaScriptWebAssemblyWeb storageIndexedDBWebGLWebGPU | Protocols | HTTPEncryptionCookiesthird-partyOCSPWebRTCWebSocket |
| Features | BookmarksExtensionsPrivacy mode |
| Web standards | HTMLv5CSSDOMJavaScriptWebAssemblyWeb storageIndexedDBWebGLWebGPU |
| Protocols | HTTPEncryptionCookiesthird-partyOCSPWebRTCWebSocket |
| ActiveBlink-basedProprietaryGoogle ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandexFOSSChromiumBraveDoobleFalkonOtterSupermiumungoogledGecko-basedFirefoxFloorpGNU IceCatLibreWolfMidoriMullvadSlimBrowserSeaMonkey(uses unnamed Geckofork)TorWaterfoxZenGoanna-basedBasiliskK-MeleonPale MoonWebKit-basedSafariGNOME WebiCabOrionMulti-engine360DuckDuckGoKonquerorLunascapeNetFrontqutebrowserOtherDilloewwFlowLadybirdLinksLynxNetSurfOpera Miniw3m | Active | Blink-basedProprietaryGoogle ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandexFOSSChromiumBraveDoobleFalkonOtterSupermiumungoogledGecko-basedFirefoxFloorpGNU IceCatLibreWolfMidoriMullvadSlimBrowserSeaMonkey(uses unnamed Geckofork)TorWaterfoxZenGoanna-basedBasiliskK-MeleonPale MoonWebKit-basedSafariGNOME WebiCabOrionMulti-engine360DuckDuckGoKonquerorLunascapeNetFrontqutebrowserOtherDilloewwFlowLadybirdLinksLynxNetSurfOpera Miniw3m | Blink-based | ProprietaryGoogle ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandexFOSSChromiumBraveDoobleFalkonOtterSupermiumungoogled | Proprietary | Google ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandex | FOSS | ChromiumBraveDoobleFalkonOtterSupermiumungoogled | Gecko-based | FirefoxFloorpGNU IceCatLibreWolfMidoriMullvadSlimBrowserSeaMonkey(uses unnamed Geckofork)TorWaterfoxZen | Goanna-based | BasiliskK-MeleonPale Moon | WebKit-based | SafariGNOME WebiCabOrion | Multi-engine | 360DuckDuckGoKonquerorLunascapeNetFrontqutebrowser | Other | DilloewwFlowLadybirdLinksLynxNetSurfOpera Miniw3m |
| Active |
| Blink-basedProprietaryGoogle ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandexFOSSChromiumBraveDoobleFalkonOtterSupermiumungoogledGecko-basedFirefoxFloorpGNU IceCatLibreWolfMidoriMullvadSlimBrowserSeaMonkey(uses unnamed Geckofork)TorWaterfoxZenGoanna-basedBasiliskK-MeleonPale MoonWebKit-basedSafariGNOME WebiCabOrionMulti-engine360DuckDuckGoKonquerorLunascapeNetFrontqutebrowserOtherDilloewwFlowLadybirdLinksLynxNetSurfOpera Miniw3m | Blink-based | ProprietaryGoogle ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandexFOSSChromiumBraveDoobleFalkonOtterSupermiumungoogled | Proprietary | Google ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandex | FOSS | ChromiumBraveDoobleFalkonOtterSupermiumungoogled | Gecko-based | FirefoxFloorpGNU IceCatLibreWolfMidoriMullvadSlimBrowserSeaMonkey(uses unnamed Geckofork)TorWaterfoxZen | Goanna-based | BasiliskK-MeleonPale Moon | WebKit-based | SafariGNOME WebiCabOrion | Multi-engine | 360DuckDuckGoKonquerorLunascapeNetFrontqutebrowser | Other | DilloewwFlowLadybirdLinksLynxNetSurfOpera Miniw3m |
| Blink-based | ProprietaryGoogle ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandexFOSSChromiumBraveDoobleFalkonOtterSupermiumungoogled | Proprietary | Google ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandex | FOSS | ChromiumBraveDoobleFalkonOtterSupermiumungoogled |
| Proprietary | Google ChromeArcAtlasAvastCốc CốcCometComodoEcosiaEpicHuaweiMaxthonMicrosoft EdgeOpera(Mobile)PuffinQQSamsungSilkSleipnirSRWareUCVivaldiWhaleYandex |
| FOSS | ChromiumBraveDoobleFalkonOtterSupermiumungoogled |
| Gecko-based | FirefoxFloorpGNU IceCatLibreWolfMidoriMullvadSlimBrowserSeaMonkey(uses unnamed Geckofork)TorWaterfoxZen |
| Goanna-based | BasiliskK-MeleonPale Moon |
| WebKit-based | SafariGNOME WebiCabOrion |
| Multi-engine | 360DuckDuckGoKonquerorLunascapeNetFrontqutebrowser |
| Other | DilloewwFlowLadybirdLinksLynxNetSurfOpera Miniw3m |
| DiscontinuedBlink-basedBeakerCitrioFlockRedcoreRockmeltSalamWebSputnikTorchGecko-basedBeonexCaminoClassillaConkerorFirefox LiteGaleonGhostzillaIceDragonKazehakaseKyloLotusMicroBMinimoMozilla suitePirateBrowserPogoStrataSwiftfoxTenFourFoxTimberwolfWaterfox ClassicxBMSHTML-basedInternet ExplorerAOLDeepnetGreenBrowserMediaBrowserMSN ExplorerMSN Program ViewerNeoPlanetNetCaptorSpaceTimeZACWebKit-basedAroraBOLTDolphinFluidGoogle TVIrisMercuryNokia SymbianOmniWebOpera CoastOrigynQtWebShiiraSteelsurfUzblWebPositivexombreroOtherabacoAmayaArachneArenaBlazerCakeCMDeepfishEdge LegacyELinksGazelleHotJavaIBM Home Page ReaderIBM WebExplorerIBrowseInternet Explorer for MacKidZuiLine ModeMosaicMSN TVNetPositiveNetscapeSkweezerSkyfireThunderHawkVisionWinWAPWorldWideWeb | Discontinued | Blink-basedBeakerCitrioFlockRedcoreRockmeltSalamWebSputnikTorchGecko-basedBeonexCaminoClassillaConkerorFirefox LiteGaleonGhostzillaIceDragonKazehakaseKyloLotusMicroBMinimoMozilla suitePirateBrowserPogoStrataSwiftfoxTenFourFoxTimberwolfWaterfox ClassicxBMSHTML-basedInternet ExplorerAOLDeepnetGreenBrowserMediaBrowserMSN ExplorerMSN Program ViewerNeoPlanetNetCaptorSpaceTimeZACWebKit-basedAroraBOLTDolphinFluidGoogle TVIrisMercuryNokia SymbianOmniWebOpera CoastOrigynQtWebShiiraSteelsurfUzblWebPositivexombreroOtherabacoAmayaArachneArenaBlazerCakeCMDeepfishEdge LegacyELinksGazelleHotJavaIBM Home Page ReaderIBM WebExplorerIBrowseInternet Explorer for MacKidZuiLine ModeMosaicMSN TVNetPositiveNetscapeSkweezerSkyfireThunderHawkVisionWinWAPWorldWideWeb | Blink-based | BeakerCitrioFlockRedcoreRockmeltSalamWebSputnikTorch | Gecko-based | BeonexCaminoClassillaConkerorFirefox LiteGaleonGhostzillaIceDragonKazehakaseKyloLotusMicroBMinimoMozilla suitePirateBrowserPogoStrataSwiftfoxTenFourFoxTimberwolfWaterfox ClassicxB | MSHTML-based | Internet ExplorerAOLDeepnetGreenBrowserMediaBrowserMSN ExplorerMSN Program ViewerNeoPlanetNetCaptorSpaceTimeZAC | WebKit-based | AroraBOLTDolphinFluidGoogle TVIrisMercuryNokia SymbianOmniWebOpera CoastOrigynQtWebShiiraSteelsurfUzblWebPositivexombrero | Other | abacoAmayaArachneArenaBlazerCakeCMDeepfishEdge LegacyELinksGazelleHotJavaIBM Home Page ReaderIBM WebExplorerIBrowseInternet Explorer for MacKidZuiLine ModeMosaicMSN TVNetPositiveNetscapeSkweezerSkyfireThunderHawkVisionWinWAPWorldWideWeb |
| Discontinued |
| Blink-basedBeakerCitrioFlockRedcoreRockmeltSalamWebSputnikTorchGecko-basedBeonexCaminoClassillaConkerorFirefox LiteGaleonGhostzillaIceDragonKazehakaseKyloLotusMicroBMinimoMozilla suitePirateBrowserPogoStrataSwiftfoxTenFourFoxTimberwolfWaterfox ClassicxBMSHTML-basedInternet ExplorerAOLDeepnetGreenBrowserMediaBrowserMSN ExplorerMSN Program ViewerNeoPlanetNetCaptorSpaceTimeZACWebKit-basedAroraBOLTDolphinFluidGoogle TVIrisMercuryNokia SymbianOmniWebOpera CoastOrigynQtWebShiiraSteelsurfUzblWebPositivexombreroOtherabacoAmayaArachneArenaBlazerCakeCMDeepfishEdge LegacyELinksGazelleHotJavaIBM Home Page ReaderIBM WebExplorerIBrowseInternet Explorer for MacKidZuiLine ModeMosaicMSN TVNetPositiveNetscapeSkweezerSkyfireThunderHawkVisionWinWAPWorldWideWeb | Blink-based | BeakerCitrioFlockRedcoreRockmeltSalamWebSputnikTorch | Gecko-based | BeonexCaminoClassillaConkerorFirefox LiteGaleonGhostzillaIceDragonKazehakaseKyloLotusMicroBMinimoMozilla suitePirateBrowserPogoStrataSwiftfoxTenFourFoxTimberwolfWaterfox ClassicxB | MSHTML-based | Internet ExplorerAOLDeepnetGreenBrowserMediaBrowserMSN ExplorerMSN Program ViewerNeoPlanetNetCaptorSpaceTimeZAC | WebKit-based | AroraBOLTDolphinFluidGoogle TVIrisMercuryNokia SymbianOmniWebOpera CoastOrigynQtWebShiiraSteelsurfUzblWebPositivexombrero | Other | abacoAmayaArachneArenaBlazerCakeCMDeepfishEdge LegacyELinksGazelleHotJavaIBM Home Page ReaderIBM WebExplorerIBrowseInternet Explorer for MacKidZuiLine ModeMosaicMSN TVNetPositiveNetscapeSkweezerSkyfireThunderHawkVisionWinWAPWorldWideWeb |
| Blink-based | BeakerCitrioFlockRedcoreRockmeltSalamWebSputnikTorch |
| Gecko-based | BeonexCaminoClassillaConkerorFirefox LiteGaleonGhostzillaIceDragonKazehakaseKyloLotusMicroBMinimoMozilla suitePirateBrowserPogoStrataSwiftfoxTenFourFoxTimberwolfWaterfox ClassicxB |
| MSHTML-based | Internet ExplorerAOLDeepnetGreenBrowserMediaBrowserMSN ExplorerMSN Program ViewerNeoPlanetNetCaptorSpaceTimeZAC |
| WebKit-based | AroraBOLTDolphinFluidGoogle TVIrisMercuryNokia SymbianOmniWebOpera CoastOrigynQtWebShiiraSteelsurfUzblWebPositivexombrero |
| Other | abacoAmayaArachneArenaBlazerCakeCMDeepfishEdge LegacyELinksGazelleHotJavaIBM Home Page ReaderIBM WebExplorerIBrowseInternet Explorer for MacKidZuiLine ModeMosaicMSN TVNetPositiveNetscapeSkweezerSkyfireThunderHawkVisionWinWAPWorldWideWeb |
| ListComparisonCategory |

 
| vteWorld Wide Web Consortium(W3C) |
| --- |
| Products,standards | RecommendationsActivityPubActivity StreamsARIACanonical XMLCDFCSSAnimationsFlexboxGridDOMEXIEmotionMLGeolocation APIGRDDLHTMLHTML5IndexedDBITSJSON-LDLinked Data NotificationsMathMLMicropubMTOMOWLPLSRDFSchemaRDFaRIFSAWSDLSISRSKOSSMILSOAPSRGSSRISSMLSVGAnimationFilter EffectsSCXMLSHACLSPARQLTimed textVoiceXMLWebAssemblyWoTTDWeb storageWSDLWebmentionWebSubWebVTTWOFFWS-AddressingXHTML+RDFaXMLBaseEncryptionEventsInformation SetNamespaceSchemaSignatureXFormsXIncludeXLinkXOPXPath2.03.xXPointerXProcXQueryXSLXSL-FOXSLTelementsNotesIndieAuthXAdESXBLXHTML+SMILXUPWorking draftsCCXMLCURIEEMEInkMLMSESMIL TimesheetssXBLWebGPUWebXRXFDLXFramesXMLHttpRequestGuidelinesWeb Content Accessibility GuidelinesInitiativeMarkup Validation ServiceWeb Accessibility InitiativeWeb ComponentsDeprecatedC-HTMLHDMLJSSSPGMLVMLWebPlatformObsoletedP3PXHTML+MathML+SVG | Recommendations | ActivityPubActivity StreamsARIACanonical XMLCDFCSSAnimationsFlexboxGridDOMEXIEmotionMLGeolocation APIGRDDLHTMLHTML5IndexedDBITSJSON-LDLinked Data NotificationsMathMLMicropubMTOMOWLPLSRDFSchemaRDFaRIFSAWSDLSISRSKOSSMILSOAPSRGSSRISSMLSVGAnimationFilter EffectsSCXMLSHACLSPARQLTimed textVoiceXMLWebAssemblyWoTTDWeb storageWSDLWebmentionWebSubWebVTTWOFFWS-AddressingXHTML+RDFaXMLBaseEncryptionEventsInformation SetNamespaceSchemaSignatureXFormsXIncludeXLinkXOPXPath2.03.xXPointerXProcXQueryXSLXSL-FOXSLTelements | Notes | IndieAuthXAdESXBLXHTML+SMILXUP | Working drafts | CCXMLCURIEEMEInkMLMSESMIL TimesheetssXBLWebGPUWebXRXFDLXFramesXMLHttpRequest | Guidelines | Web Content Accessibility Guidelines | Initiative | Markup Validation ServiceWeb Accessibility InitiativeWeb Components | Deprecated | C-HTMLHDMLJSSSPGMLVMLWebPlatform | Obsoleted | P3PXHTML+MathML+SVG |
| Recommendations | ActivityPubActivity StreamsARIACanonical XMLCDFCSSAnimationsFlexboxGridDOMEXIEmotionMLGeolocation APIGRDDLHTMLHTML5IndexedDBITSJSON-LDLinked Data NotificationsMathMLMicropubMTOMOWLPLSRDFSchemaRDFaRIFSAWSDLSISRSKOSSMILSOAPSRGSSRISSMLSVGAnimationFilter EffectsSCXMLSHACLSPARQLTimed textVoiceXMLWebAssemblyWoTTDWeb storageWSDLWebmentionWebSubWebVTTWOFFWS-AddressingXHTML+RDFaXMLBaseEncryptionEventsInformation SetNamespaceSchemaSignatureXFormsXIncludeXLinkXOPXPath2.03.xXPointerXProcXQueryXSLXSL-FOXSLTelements |
| Notes | IndieAuthXAdESXBLXHTML+SMILXUP |
| Working drafts | CCXMLCURIEEMEInkMLMSESMIL TimesheetssXBLWebGPUWebXRXFDLXFramesXMLHttpRequest |
| Guidelines | Web Content Accessibility Guidelines |
| Initiative | Markup Validation ServiceWeb Accessibility InitiativeWeb Components |
| Deprecated | C-HTMLHDMLJSSSPGMLVMLWebPlatform |
| Obsoleted | P3PXHTML+MathML+SVG |
| Groups,organizations | WHATWGDefunct:World Wide Web FoundationElectedABBoardTAGWorkingCSSSVGWebAssemblyWebAuthnCommunity, businessWeb Advertising BGWebAssemblyCGClosedDevice Description(DDWG)HTMLMultimodal Interaction Activity(MMI) | WHATWGDefunct:World Wide Web Foundation | Elected | ABBoardTAG | Working | CSSSVGWebAssemblyWebAuthn | Community, business | Web Advertising BGWebAssemblyCG | Closed | Device Description(DDWG)HTMLMultimodal Interaction Activity(MMI) |
| WHATWGDefunct:World Wide Web Foundation |
| Elected | ABBoardTAG |
| Working | CSSSVGWebAssemblyWebAuthn |
| Community, business | Web Advertising BGWebAssemblyCG |
| Closed | Device Description(DDWG)HTMLMultimodal Interaction Activity(MMI) |
| Software | CERN httpdLibwwwBrowsersLine Mode(1990–)Arena(1993–98)Agora(1994–97)Argo(1994–97)Amaya(browser/editor, 1996–2012) | CERN httpdLibwww | Browsers | Line Mode(1990–)Arena(1993–98)Agora(1994–97)Argo(1994–97)Amaya(browser/editor, 1996–2012) |
| CERN httpdLibwww |
| Browsers | Line Mode(1990–)Arena(1993–98)Agora(1994–97)Argo(1994–97)Amaya(browser/editor, 1996–2012) |
| Conferences | International World Wide Web Conference(IW3C)Steering Committee(IW3C2)First conference("WWW1", 1994) |

 
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

 
| Authority control databases |
| --- |
| International | GND |
| National | United StatesIsrael |