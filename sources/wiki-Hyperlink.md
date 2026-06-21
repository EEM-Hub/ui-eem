---
source: https://en.wikipedia.org/wiki/Hyperlink
fetched: 2026-06-20
---

Method of referencing visual computer data For help creating links on Wikipedia, see [Help:Links](./Help:Links). For the song by Eiffel 65, see [Europop (album)](./Europop_(album)). 

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/8/8e/Hyperlink_example.svg/250px-Hyperlink_example.svg.png)](./File:Hyperlink_example.svg)An example of a hyperlink as commonly seen in a [web browser](./Web_browser), with a [computer mouse](./Computer_mouse) pointer hovering above it [![](//upload.wikimedia.org/wikipedia/commons/thumb/1/19/Hyperlinks_scheme.svg/250px-Hyperlinks_scheme.svg.png)](./File:Hyperlinks_scheme.svg)Visual abstraction of several documents being connected by hyperlinks 

In [computing](./Computing), a **hyperlink**, or simply a **link**, is a digital reference providing direct access to [data](./Data_(computing)) by a [user's](./User_(computing)) [clicking](./Point_and_click) or [tapping](./Touchscreen).[[1]](./Hyperlink#cite_note-1) A hyperlink points to a whole document or to a specific element within a document. [Hypertext](./Hypertext) is text with hyperlinks. The text that is linked from is known as [anchor text](./Anchor_text). A software system that is used for viewing and creating hypertext is a *hypertext system*, and to create a hyperlink is *to hyperlink* (or simply *to link*). A user following hyperlinks is said to *navigate* or *browse* the hypertext.

 

The document containing a hyperlink is known as its source document. For example, in content from [Wikipedia](./Wikipedia) or [Google Search](./Google_Search), many words and terms in the text are hyperlinked to definitions of those terms. Hyperlinks are often used to implement reference [mechanisms](./Mechanism_(engineering)) such as tables of contents, [footnotes](./Footnotes), [bibliographies](./Bibliographies), [indexes](./Index_(publishing)), and [glossaries](./Glossaries).

 

In some hypertext, hyperlinks can be bidirectional: they can be followed in two directions, so both ends act as [anchors](./HTML_element#Anchor) and as targets. More complex arrangements exist, such as many-to-many links.

 

The effect of following a hyperlink may vary with the hypertext system and may sometimes depend on the link itself; for instance, on the [World Wide Web](./World_Wide_Web) most hyperlinks cause the target document to replace the document being displayed, but some are marked to cause the target document to open in a new window (or, perhaps, in a new [tab](./Tab_(interface))).[[2]](./Hyperlink#cite_note-2) Another possibility is [transclusion](./Transclusion), for which the link target is a [document fragment](./URI_fragment) that replaces the link anchor within the source document. Not only persons browsing the document may follow hyperlinks. These hyperlinks may also be followed automatically by programs. A program that traverses the hypertext, following each hyperlink and gathering all the retrieved documents is known as a Web *spider* or [crawler](./Web_crawler).

 

## Links

 

### Inline links

 

An [inline link](./Inline_linking) displays remote content without the need for embedding the content. The remote content may be accessed with or without the user following the link.

 

An inline link may display a modified version of the content; for instance, instead of an image, a [thumbnail](./Thumbnail), [low resolution](./Image_resolution) [preview](./Preview_(computing)), [cropped](./Cropping_(image)) section, or [magnified](./Magnification) section may be shown. The full content is then usually available on demand, as is the case with [print publishing](./Desktop_publishing) software –  e.g., with an [external link](./External_link). This allows for smaller file sizes and quicker response to changes when the full linked content is not needed, as is the case when rearranging a [page layout](./Page_layout).

 

### Anchor links

Retain the anchor in this heading; anchor links to this section exist elsewhere. 

An anchor hyperlink (anchor link) is a link bound to a portion of a document,[[3]](./Hyperlink#cite_note-3) which is often called a [fragment](https://en.wiktionary.org/wiki/fragment#English:_internet). The fragment is generally a portion of text or a heading, though not necessarily. For instance, it may also be a [*hot area*](./Screen_hotspot) in an image ([image map](./Image_map) in [HTML](./HTML)), a designated, often irregular part of an image.

 

Fragments are marked with *anchors* (in any of various ways), which is why a link to a fragment is called an anchor link (that is, a link to an anchor). For example, in [XML](./XML), the element `<anchor id="name" />"` provides anchoring capability (as long as the [DTD](./Document_type_definition) or schema defines it), and in [wiki markup](./Wiki_markup), `{{anchor|name}}` is a typical example of implementing itwhich is how en.Wikipedia's implementation of MediaWiki provides it. In [word processor](./Word_processor) apps, anchors can be inserted where desired and may be called *bookmarks*which is what Microsoft Word calls them. In [URLs](./URLs), the hash character (#) precedes the name of the anchor for the fragment.

 

One way to define a hot area in an image is by a list of coordinates that indicate its boundaries. For example, a political map of Africa may have each country hyperlinked to further information about that country. A separate invisible hot area interface allows for swapping [skins](./Skin_(computing)) or labels within the linked hot areas without repetitive embedding of links in the various skin elements.

 

**Text hyperlink.** Hyperlink is embedded into a word or a phrase and makes this text clickable.

 

**Image hyperlink.** Hyperlink is embedded into an image and makes this image clickable.

 

**Bookmark hyperlink.** Hyperlink is embedded into a text or an image and takes visitors to another part of a web page.

 

**E-mail hyperlink.** Hyperlink is embedded into e-mail address and allows visitors to send an e-mail message to this e-mail address.[[4]](./Hyperlink#cite_note-4)

 

### Fat links

 

A **fat link** (also known as a "one-to-many" link, an "extended link"[[5]](./Hyperlink#cite_note-5) or a "multi-tailed link")[[6]](./Hyperlink#cite_note-6) is a hyperlink which leads to multiple endpoints; the link is a [set-valued function](./Set-valued_function).

 

## Uses in various technologies

 

### HTML

 Main article: [HTML element § Anchor](./HTML_element#Anchor) 

[Tim Berners-Lee](./Tim_Berners-Lee) saw the possibility of using hyperlinks to link any information to any other information over the [Internet](./Internet). Hyperlinks were therefore integral to the creation of the [World Wide Web](./World_Wide_Web). Web pages are written in the hypertext mark-up language [HTML](./HTML).

 

This is what a hyperlink to the home page of the [W3C organization](./W3C_organization) could look like in HTML code:

 
```
<a href="https://www.w3.org/">W3C organization website</a>

```
 

This HTML code consists of several [tags](./HTML_element):

 
- The hyperlink starts with an anchor opening tag `<a`, and includes a hyperlink reference `href="https://www.w3.org/"` to the [URL](./URL) for the page. (The URL is enclosed in quotes.)
- The [URL](./URL) is followed by `>`, marking the end of the anchor opening tag.
- The words that follow identify what is being linked; this is the only part of the code that is ordinarily visible on the screen when the page is rendered, but when the cursor hovers over the link, many browsers display the target URL somewhere on the screen, such as in the lower left-hand corner.
- Typically these words are underlined and colored (for example, blue for a link that has not yet been visited and purple for a link already visited).
- The anchor closing tag (`</a>`) terminates the hyperlink code.
- The `<a>` tag can also consist of various [attributes](./HTML_attribute) such as the `"rel"` attribute which specifies the relationship between the current document and linked document.

 

[Webgraph](./Webgraph) is a [graph](./Graph_(discrete_mathematics)), formed from [web pages](./Web_page) as vertices and hyperlinks, as directed edges.

 

### XLink

 

The [W3C](./W3C) recommendation called [XLink](./XLink) describes hyperlinks that offer a far greater degree of functionality than those offered in HTML. These **extended links** can be *multidirectional*, remove linking from, within, and between XML documents. It can also describe *simple links*, which are unidirectional and therefore offer no more functionality than hyperlinks in HTML.[*[citation needed](./Wikipedia:Citation_needed)*]

 

### Permalinks

 Main article: [Digital preservation](./Digital_preservation) 

[Permalinks](./Permalink) are URLs that are intended to remain unchanged for many years into the future, yielding hyperlinks that are less susceptible to [link rot](./Link_rot). Permalinks are often rendered simply, that is, as friendly URLs, so as to be easy for people to type and remember. Permalinks are used in order to [point](./Pointer_(computer_programming)#Typed_pointers_and_casting) and [redirect](./URL_redirection#Meaningful,_persistent_aliases_for_long_or_changing_URLs) readers to the same [Web page](./Web_page), blog post or any online digital media.[[7]](./Hyperlink#cite_note-techopedia.com-7)

 

The scientific literature is a place where link persistence is crucial to the public knowledge. A 2013 study in [BMC Bioinformatics](./BMC_Bioinformatics) analyzed 15,000 links in abstracts from Thomson Reuters' [Web of Science](./Web_of_Science) citation index, founding that the median lifespan of Web pages was 9.3 years, and just 62% were archived.[[8]](./Hyperlink#cite_note-8) The median lifespan of a Web page constitutes high-degree variable, but its [order of magnitude](./Order_of_magnitude) usually is of some months.[[9]](./Hyperlink#cite_note-9)

 

### File based hyperlinks

 

#### Internet shortcut (.url) file

 

An *Internet shortcut* file, also known as the URL file format, has the [file extension](./File_extension) .url (possibly hidden by default in the [graphical user interface](./Graphical_user_interface)), and is the [file format](./File_format) in [Windows](./Microsoft_Windows) systems used for hyperlinks to the Internet.

 

Internet shortcuts are [text files](./Text_files), but their internal structure is similar to that of an [INI file](./INI_file). Opening them in the graphical file browser of Windows or [macOS](./MacOS) (but not [Linux](./Linux))[[10]](./Hyperlink#cite_note-q859-10) will open the link in the default web browser. Internet shortcut files can be easily made by hand, as the minimum features needed to operate as a hyperlink are simply the `[InternetShortcut]` header and the `URL=` key-value pair. Other key-value pairs are irregularly supported across operating systems.[[11]](./Hyperlink#cite_note-l824-11) An example of a valid Windows Internet Shortcut with some specialized key-value pairs is shown below:

 
```
[InternetShortcut]
URL=https://www.wikipedia.org/
WorkingDirectory=C:\WINDOWS
ShowCommand=7
IconIndex=1
IconFile=C:\WINDOWS\SYSTEM\url.dll
Modified=20F06BA06D07BD014D
HotKey=1601

```
 

#### macOS .webloc file

 

On [macOS](./MacOS) systems, the specialized file format for file based hyperlinks is the .webloc file. It uses [XML](./XML) [Property list](./Property_list) syntax:

 
```
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>URL</key>
	<string>https://www.wikipedia.org/</string>
</dict>
</plist>

```
 

#### Linux Freedesktop.org .desktop file

 

A file based hyperlink under Unix/Linux with a desktop environment is stored in a .desktop file.[[12]](./Hyperlink#cite_note-12) It is only supported under Linux.[[10]](./Hyperlink#cite_note-q859-10) It is a text file with a syntax highly similar to the Windows `URL` file described above.  An example of a valid Freedesktop.org .desktop file is shown below:

 
```
[Desktop Entry]
Encoding=UTF-8
Type=Link
Name=Wikipedia
URL=https://www.wikipedia.org/

```
 

#### link.html file 

 

A Windows, macOS, and Linux cross-platform file based hyperlink can be implemented with an unofficial link.html style file:[[10]](./Hyperlink#cite_note-q859-10)

 
```
<!DOCTYPE html><html lang="en">
<!--
Example of a link.html file: i.e. a file based hyperlink that works cross-platform on Windows, macOS, and Linux. 
-->
<head>
  <meta http-equiv="refresh" content="0; url=https://www.wikipedia.org" />
  <title>Redirecting to https://www.wikipedia.org ...</title>
</head>
<body>
  Loading <a href="https://www.wikipedia.org">https://www.wikipedia.org</a> ...
</body>
</html>

```
 

## How hyperlinks work in HTML

 

A link from one domain to another is said to be *outbound* from its source anchor and [*inbound*](./Inbound_link) to its target.

 

The most common destination anchor is a [URL](./Uniform_Resource_Locator) used in the [World Wide Web](./World_Wide_Web). This can refer to a document, e.g. a [webpage](./Webpage), or other resource, or to a position in a webpage. The latter is achieved by means of an [HTML element](./HTML_element) with a "name" or "id" attribute at that position of the HTML document. The URL of the position is the URL of the webpage with a [fragment identifier](./Fragment_identifier) –  "#*id attribute*" –  appended.

 

When linking to PDF documents from an HTML page the "*id attribute*" can be replaced with syntax that references a page number or another element of the PDF, for example, "#*page=386*".

 

### Link behavior in web browsers

 

A [web browser](./Web_browser) usually displays a hyperlink in some distinguishing way, e.g. in a different [color](./Color), [font](./Font) or [style](./Typeface), or with certain symbols following to visualize link target or document types. This is also called *link decoration*. The behavior and style of links can be specified using the [Cascading Style Sheets](./Cascading_Style_Sheets) (CSS) language.

 

In a graphical user interface, the appearance of a mouse [cursor](./Cursor_(user_interface)) may change into a hand motif to indicate a link. In most graphical web browsers, links are displayed in underlined blue text when they have not been visited, but underlined purple text when they have. When the [user](./User_(computing)) activates the link (e.g., by clicking on it with the [mouse](./Computer_mouse)) the browser displays the link's target. If the target is not an HTML file, depending on the [file type](./File_type) and on the browser and its [plugins](./Plug-in_(computing)), another program may be activated to open the file.

 

The HTML code contains some or all of the five main characteristics of a link:

 
- **link destination** ("href" pointing to a URL)
- **[link label](./Anchor_text)**
- **link title**
- **link target**
- **link class** or **link id**

 

It uses the [HTML element "a"](./HTML_anchor) with the attribute "href" (HREF is an abbreviation for "Hypertext REFerence"[[13]](./Hyperlink#cite_note-13)) and optionally also the attributes "title", "target", and "[class](./Cascading_Style_Sheets)" or "id":

 `<a href="URL" title="link title" target="link target" class="link class">link label</a>` 

To embed a link into a web page, blogpost, or comment, it may take this form:

 `<a href="https://example.com/">Example</a>` 

In a typical web browser, this would display as the underlined word "Example" in blue, which when clicked would take the user to the example.com website. This contributes to a clean, easy to read text or document.

 

By default, browsers will usually display hyperlinks as such:

 
- An unvisited link is usually blue and underlined
- A visited link is usually purple and underlined
- An active link is usually red and underlined

 

When the cursor hovers over a link, depending on the browser and graphical user interface, some informative text about the link can be shown, popping up, not in a regular [window](./Window_(computing)), but in a special [hover box](./Mouse_hover), which disappears when the cursor is moved away (sometimes it disappears anyway after a few seconds, and reappears when the cursor is moved away and back). [Mozilla Firefox](./Mozilla_Firefox), [IE](./Internet_Explorer), [Opera](./Opera_(web_browser)), and many other web browsers all show the URL. In addition, the URL is commonly shown in the [status bar](./Status_bar).

 

Normally, a link opens in the current [frame](./Framing_(World_Wide_Web)) or window, but sites that use frames and multiple windows for navigation can add a special "target" attribute to specify where the link loads. If no window exists with that name, a new window is created with the ID, which can be used to refer to the window later in the browsing session.

 

Creation of new windows is probably the most common use of the "target" attribute. To prevent accidental reuse of a window, the special window names "_blank" and "_new" are usually available, and always cause a new window to be created. It is especially common to see this type of link when one large website links to an external page. The intention in that case is to ensure that the person browsing is aware that there is no endorsement of the site being linked to by the site that was linked from. However, the attribute is sometimes overused and can sometimes cause many windows to be created even while browsing a single site.

 

Another special page name is "_top", which causes any frames in the current window to be cleared away so that browsing can continue in the full window.

 

## History

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/0/0e/SRI_ARC_Engelbart_Nov_1969.jpg/250px-SRI_ARC_Engelbart_Nov_1969.jpg)](./File:SRI_ARC_Engelbart_Nov_1969.jpg)Douglas Engelbart and his team at [SRI](./SRI_International), 1969 

The term "link" was coined in 1965 (or possibly 1964) by [Ted Nelson](./Ted_Nelson) at the start of [Project Xanadu](./Project_Xanadu). Nelson had been inspired by "[As We May Think](./As_We_May_Think)", a popular 1945 essay by [Vannevar Bush](./Vannevar_Bush). In the essay, Bush described a microfilm-based machine (the [Memex](./Memex)) in which one could link any two pages of information into a "trail" of related information, and then scroll back and forth among pages in a trail as if they were on a single microfilm reel.

 

In a series of books and articles published from 1964 through 1980, Nelson transposed Bush's concept of automated cross-referencing into the computer context, made it applicable to specific text strings rather than whole pages, generalized it from a local desk-sized machine to a theoretical proprietary worldwide computer network, and advocated the creation of such a network. Though Nelson's Xanadu Corporation was eventually funded by [Autodesk](./Autodesk) in the 1980s, it never created this proprietary public-access network. Meanwhile, working independently, a team led by [Douglas Engelbart](./Douglas_Engelbart) (with [Jeff Rulifson](./Jeff_Rulifson) as chief [programmer](./Programmer)) was the first to implement the hyperlink concept for scrolling within a single document (1966), and soon after for connecting between paragraphs within separate documents (1968), with [NLS](./NLS_(computer_system)). [Ben Shneiderman](./Ben_Shneiderman) working with graduate student Dan Ostroff designed and implemented the highlighted link in the HyperTIES system in 1983.  HyperTIES was used to produce the world's first electronic journal, the July 1988 [Communications of the ACM](./Communications_of_the_ACM), which was cited as the source for the link concept in [Tim Berners-Lee](./Tim_Berners-Lee)'s Spring 1989 manifesto for the Web.  In 1988, [Ben Shneiderman](./Ben_Shneiderman) and Greg Kearsley used HyperTIES to publish "Hypertext Hands-On!", the world's first electronic book.[*[citation needed](./Wikipedia:Citation_needed)*]

 

Released in 1987 for the [Apple Macintosh](./Mac_(computer)), the database program [HyperCard](./HyperCard) allowed for hyperlinking between various pages within a document, as well as to other documents and separate applications on the same computer.[[14]](./Hyperlink#cite_note-"Search_paths"-14) In 1990, [Windows Help](./Windows_Help), which was introduced with [Microsoft Windows 3.0](./Microsoft_Windows_3.0), had widespread use of hyperlinks to link different pages in a single [help file](./Online_help) together; in addition, it had a visually different kind of hyperlink that caused a popup help message to appear when clicked, usually to give definitions of terms introduced on the help page. The first widely used open protocol that included hyperlinks from any Internet site to any other Internet site was the [Gopher protocol](./Gopher_(protocol)) from 1991. It was soon eclipsed by HTML after the 1993 release of the [Mosaic browser](./Mosaic_(web_browser)) (which could handle Gopher links as well as HTML links). HTML's advantage was the ability to mix graphics, text, and hyperlinks, unlike Gopher, which just had menu-structured text and hyperlinks.

 

## Legal issues

 Main article: [Copyright aspects of hyperlinking and framing](./Copyright_aspects_of_hyperlinking_and_framing) 

While hyperlinking among webpages is an intrinsic feature of the [web](./World_Wide_Web), some websites object to being linked by other websites; some have claimed that linking to them is not allowed without permission.

 

Contentious in particular are [deep links](./Deep_linking), which do not point to a site's [home page](./Home_page) or other entry point designated by the site owner, but to content elsewhere, allowing the user to bypass the site's own designated flow, and *inline links*, which incorporate the content in question into the pages of the linking site, making it seem part of the linking site's own content unless an explicit attribution is added.[[15]](./Hyperlink#cite_note-15)

 

In certain jurisdictions, it is or has been held that hyperlinks are not merely [references](./Reference) or [citations](./Citations), but are devices for copying web pages. In the Netherlands, [Karin Spaink](./Karin_Spaink) was initially convicted in this way of copyright infringement by linking, although this ruling was overturned in 2003. The courts that advocate this view see the mere [publication](./Publication) of a hyperlink that connects to illegal material to be an illegal act in itself, regardless of whether referencing illegal material is illegal. In 2004, [Josephine Ho](./Josephine_Ho) was acquitted of 'hyperlinks that corrupt traditional values' in Taiwan[[16]](./Hyperlink#cite_note-16)

 

In 2000, [British Telecom](./British_Telecom) sued [Prodigy](./Prodigy_(ISP)), claiming that Prodigy infringed its patent ([U.S. patent 4,873,662](https://patents.google.com/patent/US4873662)) on web hyperlinks. After litigation, a court found for Prodigy, ruling that [British Telecom](./British_Telecom)'s patent did not cover web hyperlinks.[[17]](./Hyperlink#cite_note-17)

 

In United States *[jurisprudence](./Jurisprudence)*, there is a distinction between the mere act of linking to someone else's website, and linking to content that is illegal (e.g., gambling illegal in the US) or [infringing](./Copyright_infringement) (e.g., illegal MP3 copies).[[18]](./Hyperlink#cite_note-18) Several courts have found that merely linking to someone else's website, even if by bypassing commercial advertising, is not copyright or trademark infringement, regardless of how much someone else might object.[[19]](./Hyperlink#cite_note-19)[[20]](./Hyperlink#cite_note-20)[[21]](./Hyperlink#cite_note-21) Linking to illegal or infringing content can be sufficiently problematic to give rise to legal liability.[[22]](./Hyperlink#cite_note-22)[[23]](./Hyperlink#cite_note-23)[[24]](./Hyperlink#cite_note-24) Compare[[25]](./Hyperlink#cite_note-25) for a summary of the current status of US copyright law as to hyperlinking, see the discussion regarding [the *Arriba Soft* and *Perfect 10* cases](./Copyright_aspects_of_hyperlinking_and_framing#State_of_US_law_after_Arriba_Soft_and_Perfect_10).

 

Somewhat controversially, [Vuestar Technologies](./Vuestar_Technologies) has tried to enforce [patents](./Patent) applied for by its owner, Ronald Neville Langford,[[26]](./Hyperlink#cite_note-26) around the world relating to search techniques using hyperlinked images to other [websites](./Websites) or web pages.[[27]](./Hyperlink#cite_note-inquirer-27)

 

## See also

 
- [Backlink](./Backlink)
- [Dereference](./Dereference_operator) (operator)
- [Internal link](./Internal_link)
- [Link building](./Link_building)
- [Link rot](./Link_rot)
- [Object hyperlinking](./Object_hyperlinking)
- [Overlinking](./Overlinking)
- [PageRank](./PageRank)
- [URI fragment](./URI_fragment)
- [Xenu's Link Sleuth](./Xenu's_Link_Sleuth)
- [Nofollow](./Nofollow)

 

## References

  
1. [↑](./Hyperlink#cite_ref-1) ["hyperlink"](https://www.merriam-webster.com/dictionary/hyperlink). *Merriam-Webster*. 2025-03-13.
2. [↑](./Hyperlink#cite_ref-2) ["Tabbed browsing"](https://www.computerhope.com/jargon/t/tabbrows.htm). *Computer Hope*. Dec 31, 2020. [Archived](https://web.archive.org/web/20210526055511/https://www.computerhope.com/jargon/t/tabbrows.htm) from the original on May 26, 2021. Retrieved July 26, 2021.
3. [↑](./Hyperlink#cite_ref-3) Brusilovski, Peter; Kommers, Piet; Streitz, Norbert (1996-05-15). [*Multimedia, Hypermedia, and Virtual Reality: Models, Systems, and Application: First International Conference, MHVR'94, Moscow, Russia September (14–16), 1996. Selected Papers*](https://books.google.com/books?id=BoiMpnq5bmUC&q=%C2%A0An+anchor+hyperlink+is+a+link+bound+to+a+portion+of+a+document&pg=PA28). Springer Science & Business Media. [ISBN](./ISBN_(identifier)) [9783540612827](./Special:BookSources/9783540612827). [Archived](https://web.archive.org/web/20180207163213/https://books.google.com/books?id=BoiMpnq5bmUC&pg=PA28&dq=%C2%A0An+anchor+hyperlink+is+a+link+bound+to+a+portion+of+a+document&hl=en&sa=X&ved=0ahUKEwiRm8id6u3UAhVLslQKHRj1BCMQ6AEIJDAA#v=onepage&q=%C2%A0An%20anchor%20hyperlink%20is%20a%20link%20bound%20to%20a%20portion%20of%20a%20document&f=false) from the original on 2018-02-07.
4. [↑](./Hyperlink#cite_ref-4) ["The Anchor element – HTML: HyperText Markup Language"](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a). *Mozilla Developer Network*. [Archived](https://web.archive.org/web/20220830154353/https://developer.mozilla.org/en-US/docs/Web/HTML/Element/A) from the original on 2022-08-30. Retrieved 2021-10-13.
5. [↑](./Hyperlink#cite_ref-5) ["XML Linking Language (XLink) Version 1.0"](https://www.w3.org/TR/xlink/#extended-link). *W3C*. [Archived](https://web.archive.org/web/20210717122126/http://www.w3.org/TR/xlink/#extended-link) from the original on July 17, 2021. Retrieved July 26, 2021.
6. [↑](./Hyperlink#cite_ref-6) ["HTML, Web Browsers, and Other Paraphernalia"](https://web.archive.org/web/20130704143743/http://people.duke.edu/~mshumate/fiction/htt/tools.html#fatlink). Archived from [the original](http://people.duke.edu/~mshumate/fiction/htt/tools.html) on July 4, 2013.
7. [↑](./Hyperlink#cite_ref-techopedia.com_7-0) ["Definition of Permanent Link (Permalink)"](https://www.techopedia.com/definition/4900/permanent-link-permalink). *techopedia.com*. [Archived](https://web.archive.org/web/20181101015428/https://www.techopedia.com/definition/4900/permanent-link-permalink) from the original on November 1, 2018. Retrieved Oct 31, 2018.
8. [↑](./Hyperlink#cite_ref-8) W. Kille, Leighton (2015-10-09). ["The growing problem of Internet 'link rot' and best practices for media and online publishers"](https://journalistsresource.org/studies/society/internet/website-linking-best-practices-media-online-publishers). *journalistsresource.org*. [Archived](https://web.archive.org/web/20140919162322/https://journalistsresource.org/studies/society/internet/website-linking-best-practices-media-online-publishers) from the original on September 19, 2014. Retrieved Oct 30, 2018.
9. [↑](./Hyperlink#cite_ref-9) ["The Average Lifespan of a Webpage"](https://blogs.loc.gov/thesignal/2011/11/the-average-lifespan-of-a-webpage/). November 8, 2011. [Archived](https://web.archive.org/web/20160908223104/https://blogs.loc.gov/thesignal/2011/11/the-average-lifespan-of-a-webpage/) from the original on September 8, 2016. Retrieved Oct 31, 2018.
10. [1](./Hyperlink#cite_ref-q859_10-0) [2](./Hyperlink#cite_ref-q859_10-1) [3](./Hyperlink#cite_ref-q859_10-2) Craig-Wood, Nick (2014-03-16). ["Google drive"](https://rclone.org/drive/#:~:text=url-,INI%20style%20link%20file,-macOS%2C%20Windows). *Rclone*. Retrieved 2025-07-15.
11. [↑](./Hyperlink#cite_ref-l824_11-0) Edward L. Blake. ["An Unofficial Guide to the URL File Format"](https://www.cyanwerks.com/formats/file-format-url.html). *CyanWerks*. Retrieved 2025-07-15.
12. [↑](./Hyperlink#cite_ref-12) Preston Brown; et al. (2020-04-27). ["Desktop Entry Specification"](https://specifications.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html). *specifications.freedesktop.org*. Retrieved 2024-07-01.
13. [↑](./Hyperlink#cite_ref-13) [Tim Berners-Lee](./Tim_Berners-Lee). ["Making a Server ("HREF" is for "hypertext reference")"](https://www.w3.org/Provider/ServerWriter.html). W3C. [Archived](https://web.archive.org/web/20121025220948/http://www.w3.org/Provider/ServerWriter.html) from the original on 2012-10-25. Retrieved 2012-10-25.
14. [↑](./Hyperlink#cite_ref-"Search_paths"_14-0) (Atkinson, Bill?) (1987). "3". [*Hypercard User's Guide*](https://vintageapple.org/macprogramming/pdf/HyperCard_Users_Guide_1987.pdf#page=73) (PDF) (1 ed.). Apple Computer Inc. p. 49. [Archived](https://web.archive.org/web/20180123113437/http://vintageapple.org/macprogramming/pdf/HyperCard_Users_Guide_1987.pdf) (PDF) from the original on 2018-01-23.
15. [↑](./Hyperlink#cite_ref-15) See [*Arriba Soft* case](./Copyright_aspects_of_hyperlinking_and_framing#Kelly_v._Arriba_Soft). The Ninth Circuit decision in this case is the first important decision of a US court on linking. In it, the Ninth Circuit held the deep linking by Arriba Soft to images on Kelly's website to be legal under the fair use doctrine.
16. [↑](./Hyperlink#cite_ref-16) ["The prosecution of Taiwan sexuality researcher and activist Josephine Ho"](https://web.archive.org/web/20120208052339/http://sex.ncu.edu.tw/animal-love/news/2004Jan-Jun/Wang.pdf) (PDF). Sex.ncu.edu.tw. Archived from [the original](http://sex.ncu.edu.tw/animal-love/news/2004Jan-Jun/Wang.pdf) (PDF) on February 8, 2012. Retrieved 2012-10-25.
17. [↑](./Hyperlink#cite_ref-17) [CNET](./CNET) News.com, [Hyperlink patent case fails to click](https://web.archive.org/web/20030207070416/http://news.com.com/2100-1033-955001.html). August 23, 2002.
18. [↑](./Hyperlink#cite_ref-18) [Cybertelecom:: Legal to Link?](https://web.archive.org/web/20110629041507/http://www.cybertelecom.org/ip/link.htm)  The *Internet Archive*. Retrieved June 11, 2012.
19. [↑](./Hyperlink#cite_ref-19) Ford Motor Company v. 2600 Enterprises, 177 F.Supp.2d 661 (EDMi December 20, 2001)
20. [↑](./Hyperlink#cite_ref-20) American Civil Liberties Union v. Miller, 977 F.Supp. 1228 (ND Ga. 1997)
21. [↑](./Hyperlink#cite_ref-21) Ticketmaster Corp. v. Tickets.Com, Inc., No. 99-07654 (CD Calif. March 27, 2000)
22. [↑](./Hyperlink#cite_ref-22) [Intellectual Reserve v. Utah Lighthouse Ministry, Inc.](http://www.law.uh.edu/faculty/cjoyce/copyright/release10/IntRes.html) [Archived](https://web.archive.org/web/20081220211433/http://www.law.uh.edu/faculty/cjoyce/copyright/release10/IntRes.html) 2008-12-20 at the [Wayback Machine](./Wayback_Machine), 75 FSupp2d 1290 (D Utah 1999)
23. [↑](./Hyperlink#cite_ref-23) Universal City Studios Inc v Reimerdes, 111 FSupp2d 294 (DCNY 2000)
24. [↑](./Hyperlink#cite_ref-24) [Comcast of Illinois X LLC v. Hightech Elec. Inc.](http://www.linksandlaw.com/decision-161-comcast-illinoi-hightech-elec.pdf) [Archived](https://web.archive.org/web/20081217124715/http://www.linksandlaw.com/decision-161-comcast-illinoi-hightech-elec.pdf) 2008-12-17 at the [Wayback Machine](./Wayback_Machine), District Court for the Northern District of Illinois, Decision of July 28, 2004, 03 C 3231
25. [↑](./Hyperlink#cite_ref-25) [Perfect 10 v. Google](http://www.linksandlaw.com/decision-163-perfect-10-pictures-google.pdf) [Archived](https://web.archive.org/web/20081217124705/http://www.linksandlaw.com/decision-163-perfect-10-pictures-google.pdf) 2008-12-17 at the [Wayback Machine](./Wayback_Machine), Decision of February 21, 2006, Case No. CV 04-9484 AHM (CD Cal. 2/21/06), CRI 2006, 76–88 No liability for thumbnail links to infringing content
26. [↑](./Hyperlink#cite_ref-26) [TelecomTV – TelecomTV One – News Bot generated title ](http://web20.telecomtv.com/pages/?newsid=43241&id=e9381817-0593-417a-8639-c4c53e2a2a10&view=news) [Archived](https://web.archive.org/web/20081223012806/http://web20.telecomtv.com/pages/?newsid=43241&id=e9381817-0593-417a-8639-c4c53e2a2a10&view=news) 2008-12-23 at the [Wayback Machine](./Wayback_Machine)
27. [↑](./Hyperlink#cite_ref-inquirer_27-0) [All your Interwibble is belong to us](https://web.archive.org/web/20090221083137/http://www.theinquirer.net/inquirer/news/093/1029093/singapore-firm-owns-pictures), Silvie Barak, [The Inquirer](./The_Inquirer), 21 February 2009

 

## Further reading

 
- Weinreich, Harald; Hartmut Obendorf; Winfried Lamersdorf (2001). "The look of the link – concepts for the user interface of extended hyperlinks". *Proceedings of the 12th ACM conference on Hypertext and Hypermedia*. p. 19. [CiteSeerX](./CiteSeerX_(identifier)) [10.1.1.17.4220](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.17.4220). [doi](./Doi_(identifier)):[10.1145/504216.504225](https://doi.org/10.1145%2F504216.504225). [ISBN](./ISBN_(identifier)) [9781581134209](./Special:BookSources/9781581134209). [S2CID](./S2CID_(identifier)) [14289046](https://api.semanticscholar.org/CorpusID:14289046).

 
| vteGraphical control elements |
| --- |
| Commandinput | Adjustment handleButtonContext menuDrop-down listHamburger buttonMenuPie menu |
| Datainput-output | CheckboxColor pickerCombo boxCycle buttonDate pickerGrid viewToggle switchList boxList builderRadio buttonScrollbarSearch boxSliderSpinnerText box |
| Informational | Balloon helpHead-up display in computingHUD in video gamesIconInfobarLabelLoading screenProgress indicatorProgress barSplash screenThrobberSidebarStatus barToastTooltip |
| Containers | AccordionTree viewClient-side decorationDisclosure widgetFrame / FieldsetMenu barPanelPopoverRibbonTabToolbarWindowWindow decorationWorkspace |
| Navigational | Address barBookmarks barBreadcrumb navigationHyperlinkNavigation barVirtual desktop |
| Specialwindows | Alert dialog boxDialog boxFile dialogInspector windowModal windowPalette window |
| Relatedconcepts | File viewerList of graphical user interface elementsLayout managerLook and feelMouseoverScrollingWidget toolkitWIMPZoomable user interface |

 
| Authority control databases | GND |
| --- | --- |