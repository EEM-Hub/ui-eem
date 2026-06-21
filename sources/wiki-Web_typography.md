---
source: https://en.wikipedia.org/wiki/Web_typography
fetched: 2026-06-20
---

Publishing considerations for the Web [![](//upload.wikimedia.org/wikipedia/commons/thumb/1/14/Web_fonts.svg/250px-Web_fonts.svg.png)](./File:Web_fonts.svg)Web fonts allow Web designers to use fonts that are not installed on the viewer's computer. 

**Web typography**, like [typography](./Typography) generally, is the design of pages –  their layout and [typeface](./Typeface) choices. Unlike traditional print-based typography (where the page is fixed once [typeset](./Typeset)), pages intended for display on the [World Wide Web](./World_Wide_Web) have additional technical challenges and – given its ability to change the presentation dynamically – additional opportunities. Early web page designs were very simple due to technology limitations; modern designs use [Cascading Style Sheets](./Cascading_Style_Sheets) (CSS), [JavaScript](./JavaScript) and other techniques to deliver the typographer's and the client's vision.

 

When [HTML](./HTML) was first created, typefaces and styles were controlled exclusively by the settings of each [web browser](./Web_browser). There was no mechanism for individual Web pages to control font display until [Netscape](./Netscape) introduced the `font` element in 1995, which was then standardized in the HTML 3.2 specification. However, the [computer font](./Computer_font) specified by the `font` element had to be installed on the user's computer or a fallback font, such as a browser's default [sans-serif](./Sans-serif) or [monospace](./Monospaced_font) font, would be used. The first CSS specification was published in 1996 and provided the same capabilities.

 

The [CSS2](./CSS2) specification was released in 1998 and attempted to improve the font selection process by adding font matching, synthesis and download. These techniques did not gain much use, and were removed in the CSS2.1 specification. However, [Internet Explorer](./Internet_Explorer) added support for the font downloading feature in [version 4.0](./Internet_Explorer_4), released in 1997.[[1]](./Web_typography#cite_note-1) Font downloading was later included in the CSS3 fonts module, and has since been implemented in [Safari 3.1](./Safari_(web_browser)), [Opera 10](./Opera_10) and [Mozilla Firefox 3.5](./Mozilla_Firefox_3.5). This has subsequently increased interest in Web typography, as well as the use of font downloading.

 

## CSS1

 In traditional typography nomenclature, a [font](./Font) is a specific instance of a [typeface](./Typeface). In this article, word "font" is to be read as "[computer font](./Computer_font)" and "[font family](./Font_family)" is the web equivalent of a print-industry typeface. 

In the first CSS specification,[[2]](./Web_typography#cite_note-2) authors specified font characteristics via a series of properties:

 
- `font-family`
- `font-style`
- `font-variant`
- `font-weight`
- `font-size`

 

All fonts were identified solely by name. Beyond the properties mentioned above, designers had no way to style fonts, and no mechanism existed to select fonts not present on the client system.

 

### Web-safe fonts

 "System font" redirects here. For the fonts named 'System', see [System (typeface)](./System_(typeface)) and [Fixedsys](./Fixedsys). 

**Web-safe fonts** are [computer fonts](./Computer_font) that may reasonably be expected to be present on a wide range of [computer](./Computer) systems, and used by [Web](./Website) content authors to increase the likelihood that content displays in their chosen font. If a visitor to a Web site does not have the specified font, their browser tries to select a similar alternative, based on the author-specified [fallback fonts](./Web_typography#Fallback_fonts) and [generic families](./Web_typography#Generic_font_families) or it uses [font substitution](./Font_substitution) defined in the visitor's operating system.

 

### Microsoft's Core fonts for the Web

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/7/7e/3_Core_Fonts_for_the_web.png/250px-3_Core_Fonts_for_the_web.png)](./File:3_Core_Fonts_for_the_web.png)Since being released under Microsoft's [Core fonts for the Web](./Core_fonts_for_the_Web) program, Arial, Georgia, and Verdana have become three de facto fonts of the Web. Main article: [Core fonts for the Web](./Core_fonts_for_the_Web) 

To ensure that all Web users had a basic set of fonts, [Microsoft](./Microsoft) started the [Core fonts for the Web](./Core_fonts_for_the_Web) initiative in 1996 (terminated in 2002). Released fonts include [Arial](./Arial), [Courier New](./Courier_New), [Times New Roman](./Times_New_Roman), [Comic Sans](./Comic_Sans), [Impact](./Impact_(typeface)), [Georgia](./Georgia_(typeface)), [Trebuchet](./Trebuchet_MS), [Webdings](./Webdings) and [Verdana](./Verdana)—under an [EULA](./EULA) that made them freely distributable but also limited some rights to their use. Their high penetration rate has made them a staple for Web designers. However, most [Linux distributions](./Linux_distributions) don't include these fonts by default.

 

[CSS2](./CSS2) attempted to increase the tools available to Web developers by adding font synthesis, improved font matching and the ability to download remote fonts.[[3]](./Web_typography#cite_note-3)

 

Some CSS2 font properties were removed from CSS2.1 and later included in CSS3.[[4]](./Web_typography#cite_note-4)[[5]](./Web_typography#cite_note-5)

 

### Fallback fonts

 Main article: [Fallback font](./Fallback_font) 

The CSS specification allows for multiple fonts to be listed as fallback fonts.[[6]](./Web_typography#cite_note-CSS2fontspec-6) In CSS, the `font-family` property accepts a list of comma-separated font faces to use, like so:

 
```
font-family: "Nimbus Sans L", Helvetica, Arial, sans-serif;

```
 

The first font specified is the preferred font. If this font is not available, the Web browser attempts to use the next font in the list. If none of the fonts specified are found, the browser displays its default font. This same process also happens on a per-character basis if the browser tries to display a character not present in the specified font.

 

### Generic font families

 

To give Web designers some control over the appearance of fonts on their Web pages, even when the specified fonts are not available, the CSS specification allows the use of several generic [font families.](./Font_family_(HTML)) These families are designed to split fonts into several categories based on their general appearance. They are commonly specified as the last in a series of fallback fonts, as a last resort in the event that none of the fonts specified by the author are available. For several years, there were five generic families:[[6]](./Web_typography#cite_note-CSS2fontspec-6)

 

[Sans-serif](./Sans-serif)

 Fonts that do not have decorative markings, or serifs, on their letters. These fonts are often considered easier to read on screens.[[7]](./Web_typography#cite_note-7) 

[Serif](./Serif)

 Fonts that have decorative markings, or serifs, present on their characters. These fonts are traditionally used in printed books. 

[Monospace](./Monospaced_font)

 Fonts in which all characters are equally wide. 

[Cursive](./Cursive)

 Fonts that resemble cursive writing. These fonts may have a decorative appearance, but they can be difficult to read at small sizes, so they are generally used sparingly. 

[Fantasy](./Fantasy_fonts?action=edit&redlink=1)

 Fonts that may contain symbols or other decorative properties, but still represent the specified character. 

### CSS fonts working draft 4 with lesser browser support

 

As of February 2024[[update]](https://en.wikipedia.org/w/index.php?title=Web_typography&action=edit), the [CSS Working Group](./CSS_Working_Group) of [W3C](./W3C) proposes that systems specify a default font using `ui` tags;[[8]](./Web_typography#cite_note-8) as of the same date, these are not widely supported yet.[[9]](./Web_typography#cite_note-cssf4-9)

 
- System-ui Default fonts on a given system: the purpose of this option is to allow web content to integrate with the look and feel of the native OS.
- ui-serif Default fonts on a given system in a serif style
- ui-sans-serif Default fonts on a given system in a sans-serif style
- ui-monospace Default fonts on a given system in a monospace style
- ui-rounded Default fonts on a given system in a rounded style
- [Emoji](./Emoji) Fonts using [emoji](./Emoji)
- [Math](./Typographical_conventions_in_mathematical_formulae) Fonts for complex mathematical formula and expressions.
- [Fangsong](./Fang_Song) ([Chinese](./Chinese_language): 仿宋体) 
- Chinese typefaces that are between serif Song and cursive Kai forms. This style is often used for government documents.

 

## Web fonts

 

### History

 

A technique to refer to and automatically download remote fonts was first specified in the CSS2 specification, which introduced the `@font-face` construct. At the time, fetching font files from the web was controversial because fonts meant to be used only for certain web pages could also be downloaded and installed in breach of the font license.[[10]](./Web_typography#cite_note-10)

 

Microsoft first added support for downloadable [EOT](./Embedded_OpenType) fonts in [Internet Explorer 4](./Internet_Explorer_4) in 1997. Authors had to use the proprietary [WEFT](./Web_Embedding_Fonts_Tool) tool to create a subsetted font file for each page. EOT showed that webfonts could work and the format saw some use in [writing systems](./Writing_system) not supported by common operating systems. However, the format never gained widespread acceptance and was ultimately rejected by W3C.[[11]](./Web_typography#cite_note-11)

 

In 2006, [Håkon Wium Lie](./Håkon_Wium_Lie) started a campaign against using EOT and rather have web browsers support commonly used font formats.[[12]](./Web_typography#cite_note-12)[[13]](./Web_typography#cite_note-13)[[14]](./Web_typography#cite_note-14) Support for the commonly used TrueType and OpenType font formats has since been implemented in [Safari 3.1](./Safari_(web_browser)), [Opera 10](./Opera_10), [Mozilla Firefox 3.5](./Mozilla_Firefox_3.5) and [Internet Explorer 9](./Internet_Explorer_9).

 

In 2010, the [WOFF](./Web_Open_Font_Format) compression method for TrueType and OpenType fonts was submitted to W3C by the [Mozilla Foundation](./Mozilla_Foundation), [Opera Software](./Opera_Software) and [Microsoft](./Microsoft), and browsers have since added support.[[15]](./Web_typography#cite_note-15)[[16]](./Web_typography#cite_note-16)[[17]](./Web_typography#cite_note-17)

 

[Google Fonts](./Google_Fonts) was launched in 2010 to serve webfonts under [open-source](./Open-source_software#Free_software) licenses. By 2016, more than 800 webfont families are available.[[18]](./Web_typography#cite_note-18)

 

Webfonts have become an important tool for web designers and as of 2016 a majority of sites use webfonts.[[19]](./Web_typography#cite_note-19)

 

### File formats

 

By using a specific CSS `@font-face` embedding technique[[20]](./Web_typography#cite_note-20) it is possible to embed fonts such that they work with IE4+, Firefox 3.5+, Safari 3.1+, Opera 10+ and Chrome 4.0+. This allows the vast majority of Web users to access this functionality.  Some commercial foundries object to the redistribution of their fonts. For example, [Hoefler & Frere-Jones](./Hoefler_&_Frere-Jones) says that, while they "...enthusiastically [support] the emergence of a more expressive Web in which designers can safely and reliably use high-quality fonts online," the current delivery of fonts using `@font-face` is considered "illegal distribution" by the foundry and is not permitted.<ref&#x3E;{{citation|url=http://typography.com/ask/faq.php#Ft_10 |title=What's involved in using fonts on websites? |publisher=[[Hoefler &#x26; Frere&#x2D;Jones]] |access&#x2D;date=2010&#x2D;03&#x2D;17 |url&#x2D;status=dead |archive&#x2D;url=https://web.archive.org/web/20100322235842/http://www.typography.com/ask/faq.php#Ft_9 |archive&#x2D;date=March 22, 2010 }}</ref&#x3E;[[21]](./Web_typography#cite_note-21) Instead, Hoefler & Co. offer a proprietary font delivery system rooted in the cloud. Many other commercial type foundries address the redistribution of their fonts by offering a specific license, known as a web font license, which permits the use of the font software to display content on the web, a use normally prohibited by basic desktop licenses. Naturally this does not interfere with fonts and foundries under free licences.[[m 1]](./Web_typography#cite_note-22)

 

#### TrueDoc

 

[TrueDoc](./TrueDoc), while not specifically a webfont specification, was the first standard for embedding fonts. It was developed by the type foundry [Bitstream](./Bitstream_Inc.) in 1994, and became natively supported in [Netscape Navigator](./Netscape_Navigator) 4, in 1996. Due to open source license restrictions, with Netscape unable to release Bitstream's source code, native support for the technology ended when Netscape Navigator 6 was released. An [ActiveX](./ActiveX) plugin was available to add support for TrueDoc to [Internet Explorer](./Internet_Explorer), but the technology had to compete against [Microsoft](./Microsoft)'s [Embedded OpenType](./Embedded_OpenType) fonts, which had natively supported in their Internet Explorer browser since version 4.0.[[22]](./Web_typography#cite_note-23) Another impediment was the lack of open-source or free tool to create webfonts in TrueDoc format, whereas Microsoft made available a free [Web Embedding Fonts Tool](./Web_Embedding_Fonts_Tool) to create webfonts in their format.

 

#### Embedded OpenType

 

Internet Explorer has supported font embedding through the proprietary [Embedded OpenType](./Embedded_OpenType) standard since version 4.0. It uses [digital rights management](./Digital_rights_management) techniques to help prevent fonts from being copied and used without a license. A simplified subset of EOT has been formalized under the name of CWT (*Compatibility Web Type*, formerly *EOT-Lite*)[[23]](./Web_typography#cite_note-24)

 

#### Scalable Vector Graphics

 

Web typography applies to [SVG](./Scalable_Vector_Graphics) in two ways:

 
1. All versions of the SVG 1.1 specification, including the [SVGT](./Scalable_Vector_Graphics#Mobile_profiles) subset, define a font module allowing the creation of fonts within an SVG document. [Safari](./Safari_(web_browser)) introduced support for many of these properties in version 3. [Opera](./Opera_(web_browser)) added preliminary support in version 8.0, with support for more properties in 9.0.
2. The SVG specification lets CSS apply to SVG documents in a similar manner to HTML documents, and the `@font-face` rule can be applied to text in SVG documents. Opera added support for this in version 10,[[24]](./Web_typography#cite_note-25) and [WebKit](./WebKit) since version 325 also supports this method using [SVG fonts](./SVG_fonts?action=edit&redlink=1) only.

 

#### Scalable Vector Graphics Fonts

 

[SVG fonts](./SVG_fonts?action=edit&redlink=1) was a W3C standard of fonts using SVG graphic that became a subset of OpenType fonts.[[25]](./Web_typography#cite_note-26) It allowed multicolor[[26]](./Web_typography#cite_note-27) or animated fonts.[[27]](./Web_typography#cite_note-28) It was first a subset of SVG 1.1 specifications[[28]](./Web_typography#cite_note-29) but it has been deprecated[[29]](./Web_typography#cite_note-30) in the SVG 2.0 specification. The SVG fonts as independent format is supported by most browsers apart from IE and Firefox, and is deprecated in Chrome (and Chromium).[[30]](./Web_typography#cite_note-31) That's now generally deprecated; the standard that most browser vendor agreed with is SVG font subset included in OpenType (and then WOFF superset, see below), called [SVGOpenTypeFonts](./SVGOpenTypeFonts?action=edit&redlink=1).[[31]](./Web_typography#cite_note-32) Firefox has supported SVG OpenType since Firefox 26.

 

#### TrueType/OpenType

 Main articles: [TrueType](./TrueType) and [OpenType](./OpenType) 

Linking to industry-standard *TrueType* (TTF) and *OpenType* (TTF/OTF) fonts is supported by
Mozilla Firefox 3.5+, Opera 10+,[[32]](./Web_typography#cite_note-33) Safari 3.1+,[[33]](./Web_typography#cite_note-34) and Google Chrome 4.0+.[[34]](./Web_typography#cite_note-35) Internet Explorer 9+ supports only those fonts with embedding permissions set to installable.[[35]](./Web_typography#cite_note-36)

 

#### Web Open Font Format

 Main article: [Web Open Font Format](./Web_Open_Font_Format) 

The [Web Open Font Format](./Web_Open_Font_Format) (WOFF) is essentially [OpenType](./OpenType) or [TrueType](./TrueType) with compression and additional metadata. WOFF is supported by Mozilla Firefox 3.6+,[[36]](./Web_typography#cite_note-37) [Google Chrome](./Google_Chrome) 5+,[[37]](./Web_typography#cite_note-38)[[38]](./Web_typography#cite_note-39) [Opera](./Opera_(web_browser)) [Presto](./Presto_(layout_engine)),[[39]](./Web_typography#cite_note-40)
and is supported by [Internet Explorer 9](./Internet_Explorer_9) (since March 14, 2011).[[40]](./Web_typography#cite_note-41) Support is available on Mac OS X Lion's [Safari](./Safari_(web_browser)) from release 5.1.

 

## Unicode fonts

 

The term *Unicode font* is a [computer font](./Computer_font) that maps [glyphs](./Glyph) to [code points](./Code_point) defined in the [Unicode Standard](./Unicode_Standard).[[41]](./Web_typography#cite_note-42) The term has become redundant since the vast majority of modern computer fonts use Unicode mappings, even those fonts which only include glyphs for a single [writing system](./Writing_system), or even only support the [basic Latin alphabet](./Basic_Latin_(Unicode_block)). Fonts which support a wide range of [Unicode scripts](./Unicode_scripts) and [Unicode symbols](./Unicode_symbols) are sometimes referred to as "pan-Unicode fonts", although as the maximum number of glyphs that can be defined in a [TrueType](./TrueType) font is restricted to 65,535, it is not possible for a single font to provide individual glyphs for all defined Unicode characters (159,801 characters, with Unicode 17.0). 

 

Only two fonts available by default on the [Windows](./Microsoft_Windows) platform, [Microsoft Sans Serif](./Microsoft_Sans_Serif) and [Lucida Sans Unicode](./Lucida_Sans_Unicode), provide a wide [Unicode](./Unicode) character repertoire.[*[needs update](./Wikipedia:Manual_of_Style/Dates_and_numbers#Chronological_items)*]

 

On [free and open-source software](./Free_and_open-source_software) platforms such as [Linux](./Linux), [GNU Unifont](./GNU_Unifont) and [GNU FreeFont](./GNU_FreeFont) provide a wide range of characters. On [ChromeOS](./ChromeOS), Google's [Noto fonts](./Noto_fonts) support (or are planned to support) all the [scripts](./Script_(Unicode)) encoded in the Unicode standard

 

## Alternatives

 

A common hurdle in Web design is the design of mockups that include fonts that are not Web-safe. There are a number of solutions for situations like this. One common solution is to replace the text with a similar Web-safe font or use a series of similar-looking fallback fonts.

 

Another technique is *image replacement*. This practice involves overlaying text with an image containing the same text written in the desired font. This is good for aesthetic purposes, but prevents text selection, increases bandwidth use, is bad for [search engine optimization](./Search_engine_optimization), and makes the text [inaccessible](./Web_accessibility) for users with disabilities.[*[citation needed](./Wikipedia:Citation_needed)*]

 

In the past, [Flash](./Adobe_Flash)-based solutions such as [sIFR](./SIFR) were used. This is similar to image replacement techniques, though the text is selectable and rendered as a vector. However, this method requires the presence of a proprietary plugin on a client's system.

 

Another solution is using JavaScript to replace the text with [VML](./Vector_Markup_Language) (for Internet Explorer) or [SVG](./Scalable_Vector_Graphics) (for all other browsers).[[42]](./Web_typography#cite_note-43)

 

## See also

 
- [Scalable Inman Flash Replacement](./Scalable_Inman_Flash_Replacement)

 

## Notes

 
1. [↑](./Web_typography#cite_ref-22) See [Open-source typefaces](./Category:Open-source_typefaces) and [Free software Unicode typefaces](./Category:Free_software_Unicode_typefaces) listings for such fonts.

 

## References

 
1. [↑](./Web_typography#cite_ref-1) Garaffa, Dave (2 September 1997). ["Embedded Fonts In Microsoft IE4pr2"](https://web.archive.org/web/19980708194539/http://browserwatch.internet.com/news/story/microsoft265.html). [Internet.com](./Internet.com). Archived from [the original](http://browserwatch.internet.com/news/story/microsoft265.html) on 8 July 1998.
2. [↑](./Web_typography#cite_ref-2) [*Cascading Style Sheets, level 1*](http://www.w3.org/TR/CSS1/), W3C, 1996-12-17
3. [↑](./Web_typography#cite_ref-3) ["Fonts"](http://www.w3.org/TR/2008/REC-CSS2-20080411/fonts.html), *Cascading Style Sheets, level 2:CSS2 Specification*, [World Wide Web Consortium](./World_Wide_Web_Consortium), 1998-05-12, retrieved 2009-07-28
4. [↑](./Web_typography#cite_ref-4) [*CSS2.1 Changes —C.2.97 Chapter 15 Fonts*](http://www.w3.org/TR/CSS21/changes.html#q104), [World Wide Web Consortium](./World_Wide_Web_Consortium), retrieved 2010-01-30
5. [↑](./Web_typography#cite_ref-5) [*CSS3 module: Web Fonts*](http://www.w3.org/TR/css3-webfonts), [World Wide Web Consortium](./World_Wide_Web_Consortium), retrieved 2010-01-30
6. [1](./Web_typography#cite_ref-CSS2fontspec_6-0) [2](./Web_typography#cite_ref-CSS2fontspec_6-1) ["CSS2 specification"](http://www.w3.org/TR/CSS2/fonts.html), *Fonts*, [World Wide Web Consortium](./World_Wide_Web_Consortium)
7. [↑](./Web_typography#cite_ref-7) Poole, Alex (2005-04-07). ["Which Are More Legible: Serif or Sans Serif Typefaces?"](http://alexpoole.info/blog/which-are-more-legible-serif-or-sans-serif-typefaces/). [Archived](https://web.archive.org/web/20170722154726/http://alexpoole.info/blog/which-are-more-legible-serif-or-sans-serif-typefaces/) from the original on 2017-07-22. Retrieved 2017-09-27.
8. [↑](./Web_typography#cite_ref-8) CSS Working Group (1 February 2024). ["CSS Fonts Module Level 4"](https://www.w3.org/TR/css-fonts-4/).
9. [↑](./Web_typography#cite_ref-cssf4_9-0)  ["Ui-serif, ui-sans-serif, ui-monospace and ui-rounded values for font-family | Can I use... Support tables for HTML5, CSS3, etc"](https://caniuse.com/extended-system-fonts).
10. [↑](./Web_typography#cite_ref-10) Hill, Bill (2008-07-21), [*Font Embedding on the Web*](https://web.archive.org/web/20150906112130/http://blogs.msdn.com/b/ie/archive/2008/07/21/font-embedding-on-the-web.aspx), Microsoft, archived from [the original](http://blogs.msdn.com/b/ie/archive/2008/07/21/font-embedding-on-the-web.aspx) on 2015-09-06
11. [↑](./Web_typography#cite_ref-11) [W3C team comment](http://www.w3.org/Submission/2008/01/Comment)
12. [↑](./Web_typography#cite_ref-12) [Microsoft's forgotten monopoly](https://www.cnet.com/news/microsofts-forgotten-monopoly/)
13. [↑](./Web_typography#cite_ref-13) [Web fonts: the view from the free world](http://people.opera.com/howcome/2008/atypi/)
14. [↑](./Web_typography#cite_ref-14) [CSS @ Ten: The Next Big Thing](http://www.alistapart.com/articles/cssatten)
15. [↑](./Web_typography#cite_ref-15) [WOFF File Format 1.0 Submission Request to W3C](http://www.w3.org/Submission/2010/03/)
16. [↑](./Web_typography#cite_ref-16) Galineau, Sylvain (2010-04-23), [*Meet WOFF, The Standard Web Font Format*](http://blogs.msdn.com/b/ie/archive/2010/04/23/meet-woff-the-standard-web-font-format.aspx), Microsoft
17. [↑](./Web_typography#cite_ref-17) [*WOFF conversion reference code*](https://web.archive.org/web/20161007142454/https://people.mozilla.org/~jkew/woff/), archived from [the original](https://people.mozilla.org/~jkew/woff/) on October 7, 2016, retrieved May 8, 2016
18. [↑](./Web_typography#cite_ref-18) ["The new Google Fonts database is a design geek's paradise"](https://www.theverge.com/2016/6/15/11950320/google-fonts-website-redesign-2016). *Theverge.com*. Retrieved 24 August 2016.
19. [↑](./Web_typography#cite_ref-19) Richard Fink (2016-09-06)[Webfonts on the Prairie](https://alistapart.com/article/webfonts-on-the-prairie), Alist Apart
20. [↑](./Web_typography#cite_ref-20) Kimler, Scott Thomas (2009-07-04), [*xBrowser Fonts — Expand Your Font Palette Using CSS3*](https://web.archive.org/web/20120315104135/http://randsco.com/index.php/2009/07/04/cross_browser_font_embedding), archived from [the original](http://randsco.com/index.php/2009/07/04/cross_browser_font_embedding) on 2012-03-15, retrieved 2010-02-05
21. [↑](./Web_typography#cite_ref-21) Wubben, Mark (February 27, 2009). ["Geek Meet: Web Typography and sIFR 3 - Slide 15 and 16"](https://www.slideshare.net/novemberborn/geek-meet-web-typography-and-sifr-3#15). [SlideShare](./SlideShare). Retrieved 17 March 2010.
22. [↑](./Web_typography#cite_ref-23) Niederst, Jennifer (2001). [*Web design in a nutshell: a desktop quick reference*](https://archive.org/details/webdesigninnutsh00nied_0) (2nd ed.). O'Reilly. p. [36](https://archive.org/details/webdesigninnutsh00nied_0/page/36). [ISBN](./ISBN_(identifier)) [0-596-00196-7](./Special:BookSources/0-596-00196-7). Retrieved 20 March 2016. what year was truedoc developed.
23. [↑](./Web_typography#cite_ref-24) Daggett, John (2009-07-31), [*EOT-Lite File Format v.1.1*](http://lists.w3.org/Archives/Public/www-font/2009JulSep/0969.html), [World Wide Web Consortium](./World_Wide_Web_Consortium), retrieved 2010-01-30
24. [↑](./Web_typography#cite_ref-25) Mills, Chris (2008-12-04), [*Opera Presto 2.2 and Opera 10 — a first look*](http://dev.opera.com/articles/view/presto-2-2-and-opera-10-a-first-look/#webfontssvg), [Opera Software](./Opera_Software), retrieved 2010-01-30
25. [↑](./Web_typography#cite_ref-26) [*SVG in OpenType*](http://www.w3.org/2013/10/SVG_in_OpenType/), W3C, retrieved 2014-09-20
26. [↑](./Web_typography#cite_ref-27) [*Colorful typography on the web: get ready for multicolor fonts*](http://pixelambacht.nl/2014/multicolor-fonts/), Pixel Ambacht, retrieved 2014-09-20
27. [↑](./Web_typography#cite_ref-28) [*Anymated Glyph Example*](https://web.archive.org/web/20141009122339/http://people.mozilla.org/~jkew/opentype-svg/soccer.html), people.Mozilla, archived from [the original](https://people.mozilla.org/~jkew/opentype-svg/soccer.html) on 2014-10-09, retrieved 2014-09-20
28. [↑](./Web_typography#cite_ref-29) [*Fonts*](http://www.w3.org/TR/SVG/fonts.html), W3C, retrieved 2014-09-20
29. [↑](./Web_typography#cite_ref-30) [*Fonts chapter*](https://www.w3.org/TR/SVG2/changes.html#fonts), W3C, retrieved 2018-03-08
30. [↑](./Web_typography#cite_ref-31) [*Can I Use SVG fonts*](http://caniuse.com/svg-fonts), CanIuse, retrieved 2014-09-20
31. [↑](./Web_typography#cite_ref-32) [*SVGOpenTypeFonts*](https://wiki.mozilla.org/SVGOpenTypeFonts), Mozilla, retrieved 2014-09-20
32. [↑](./Web_typography#cite_ref-33) Mills, Chris (2008-12-04), [*Opera Presto 2.2 and Opera 10 — a first look*](http://www.opera.com/docs/specs/presto22/#css), Opera Developer Community, retrieved 2010-01-29
33. [↑](./Web_typography#cite_ref-34) Marsal, Katie (2008-02-07), [*Apple's Safari 3.1 to support downloadable web fonts, more*](http://www.appleinsider.com/articles/08/02/07/apples_safari_3_1_to_support_downloadable_web_fonts_more.html), [AppleInsider](./AppleInsider), retrieved 2010-02-05
34. [↑](./Web_typography#cite_ref-35) Irish, Paul (2010-01-25), [*Chrome and @font-face: It's here!*](http://paulirish.com/2009/chrome-and-font-face-a-summary/)
35. [↑](./Web_typography#cite_ref-36) Galineau, Sylvain (2010-07-15), [*The CSS Corner: Better Web Typography For Better Design*](http://blogs.msdn.com/b/ie/archive/2010/07/15/the-css-corner-better-web-typography-for-better-design.aspx), Microsoft
36. [↑](./Web_typography#cite_ref-37) Shapiro, Melissa (2009-10-20), [*Mozilla Supports Web Open Font Format*](http://blog.mozilla.com/blog/2009/10/20/mozilla-supports-web-open-font-format/), Mozilla, retrieved 2010-02-05
37. [↑](./Web_typography#cite_ref-38) Gilbertson, Scott (2010-04-26), [*Google Chrome to Support the Web Open Font Format*](http://www.webmonkey.com/2010/04/google-chrome-to-support-the-web-open-font-format), webmonkey
38. [↑](./Web_typography#cite_ref-39) [*Bug 38217 - [chromium] Add WOFF support*](https://bugs.webkit.org/show_bug.cgi?id=38217), WebKit
39. [↑](./Web_typography#cite_ref-40) [*Web specifications support in Opera Presto 2.7*](http://www.opera.com/docs/specs/presto27/), Opera
40. [↑](./Web_typography#cite_ref-41) Galineau, Sylvain (2010-04-23), [*Meet WOFF, The Standard Web Font Format*](http://blogs.msdn.com/ie/archive/2010/04/23/meet-woff-the-standard-web-font-format.aspx), Microsoft
41. [↑](./Web_typography#cite_ref-42) ["Fonts and keyboards"](https://www.unicode.org/faq/font_keyboard.html). Unicode Consortium. 28 June 2017. [Archived](https://web.archive.org/web/20191018224143/http://unicode.org/faq/font_keyboard.html) from the original on 18 October 2019. Retrieved 13 October 2019.
42. [↑](./Web_typography#cite_ref-43) [About Cufon](https://github.com/sorccu/cufon/wiki/About)

 

## External links

   **Web typography**  at Wikipedia's [sister projects](./Wikipedia:Wikimedia_sister_projects)  
- [![Wikimedia Commons logo](//upload.wikimedia.org/wikipedia/en/thumb/4/4a/Commons-logo.svg/20px-Commons-logo.svg.png)](./File:Commons-logo.svg)[Media](https://commons.wikimedia.org/wiki/Category:Web%20design) from Commons
- [![Wikiversity logo](//upload.wikimedia.org/wikipedia/commons/thumb/0/0b/Wikiversity_logo_2017.svg/40px-Wikiversity_logo_2017.svg.png)](./File:Wikiversity_logo_2017.svg)[Resources](https://en.wikiversity.org/wiki/Web%20Design) from Wikiversity
- ![](//upload.wikimedia.org/wikipedia/commons/thumb/f/ff/Wikidata-logo.svg/40px-Wikidata-logo.svg.png)[Data](https://www.wikidata.org/wiki/Q1899429) from Wikidata
- [![MediaWiki logo](//upload.wikimedia.org/wikipedia/commons/thumb/a/a6/MediaWiki-2020-icon.svg/40px-MediaWiki-2020-icon.svg.png)](./File:MediaWiki-2020-icon.svg)[Documentation](https://www.mediawiki.org/wiki/Design/Typography) from MediaWiki

  
- [W3C CSS Fonts Specification](https://www.w3.org/TR/css-fonts-3/)
- List of RFC as mentioned in WOFF (draft of 2009-10-23):

- RFC [1950](https://www.rfc-editor.org/rfc/rfc1950) ZLIB Compressed Data Format Specification
- RFC [2119](https://www.rfc-editor.org/rfc/rfc2119) Key words for use in RFCs to Indicate Requirement Levels
- RFC [4647](https://www.rfc-editor.org/rfc/rfc4647) Matching of Language Tags

 
| vteTypography |
| --- |
| Page | Canons of page constructionColumnEven workingMarginPage numberingPaper sizePaginationPull quoteRecto and versoIntentionally blank page |
| Paragraph | AlignmentLeadingLine lengthRiverRunaroundWidows and orphansrunt |
| Character | Typeface anatomyCounterDiacriticsDingbatGlyphInk trapLigatureRotationSubscript and superscriptSwashText figuresTittleCapitalizationAll capsCamel caseInitialLetter caseSmall capsSnake caseTitle caseVisual distinctionBlackboard boldBoldColor printingItalicsObliqueUnderlineWhitespaceHorizontal aspectsFigure spaceKerningLetter spacingPitchSentence spacingThin spaceWord spacingVertical aspectsAscenderBaselineBody heightCap heightDescenderMean lineOvershootx-height | Typeface anatomy | CounterDiacriticsDingbatGlyphInk trapLigatureRotationSubscript and superscriptSwashText figuresTittle | Capitalization | All capsCamel caseInitialLetter caseSmall capsSnake caseTitle case | Visual distinction | Blackboard boldBoldColor printingItalicsObliqueUnderlineWhitespace | Horizontal aspects | Figure spaceKerningLetter spacingPitchSentence spacingThin spaceWord spacing | Vertical aspects | AscenderBaselineBody heightCap heightDescenderMean lineOvershootx-height |
| Typeface anatomy | CounterDiacriticsDingbatGlyphInk trapLigatureRotationSubscript and superscriptSwashText figuresTittle |
| Capitalization | All capsCamel caseInitialLetter caseSmall capsSnake caseTitle case |
| Visual distinction | Blackboard boldBoldColor printingItalicsObliqueUnderlineWhitespace |
| Horizontal aspects | Figure spaceKerningLetter spacingPitchSentence spacingThin spaceWord spacing |
| Vertical aspects | AscenderBaselineBody heightCap heightDescenderMean lineOvershootx-height |
| Typefaceclassifications | Roman typeSerifAntiquaDidoneslab serifSans-serifBlackletter typeBastardaFrakturRotundaSchwabacherGaelic typeInsularUncialSpecialistRecord typeDisplay typefacescriptfat facereverse-contrast | Roman type | SerifAntiquaDidoneslab serifSans-serif | Blackletter type | BastardaFrakturRotundaSchwabacher | Gaelic type | InsularUncial | Specialist | Record typeDisplay typefacescriptfat facereverse-contrast |
| Roman type | SerifAntiquaDidoneslab serifSans-serif |
| Blackletter type | BastardaFrakturRotundaSchwabacher |
| Gaelic type | InsularUncial |
| Specialist | Record typeDisplay typefacescriptfat facereverse-contrast |
| Punctuation(List) | BulletDashHanging punctuationHyphenminus signInterpunctSpaceVertical bar |
| Typesetting | Etaoin shrdluFontcomputermonospacedFont catalogFor position onlyLetterpressLorem ipsumMicroprintingMicrotypographyMovable typePangramPhototypesettingPunchcuttingReversing typeSortType colorType designTypefacelist |
| Typographic units | AgateCiceroEmEnMetric unitsPicaPointtraditional point-size namesTwip |
| Digital typography | Character encodingHintingText shapingRasterizationTypographic featuresWeb typographyBézier curvesDesktop publishing |
| Typography in otherwriting systems | ArabicCyrillicPT FontsEast AsianThaiNational Fonts |
| Related articles | PenmanshipHandwritingHandwriting scriptCalligraphyLetteringStyle guideType designType foundryHistory of Western typographyIntellectual property protection of typefacesTechnical letteringVox-ATypI classification |
| Related template | Punctuation and other typographic symbols |
| Category |