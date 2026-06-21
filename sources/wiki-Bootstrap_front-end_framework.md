---
source: https://en.wikipedia.org/wiki/Bootstrap_(front-end_framework)
fetched: 2026-06-20
---

Web design front-end  This article is about the CSS framework. For other uses, see [Bootstrapping (disambiguation)](./Bootstrap_(disambiguation)). 
| Bootstrap |
| --- |
|  |
| Original authors | Mark Otto, Jacob Thornton |
| Developer | Bootstrap Core Team |
| Release | August19, 2011;14 years ago(2011-08-19) |
|  |
| Stable release | 5.3.8[1]/ 25 August 2025;9 months ago(25 August 2025) |
|  |
| Written in | HTML,CSS,Less(v3),Sass(v4) andJavaScript |
| Platform | Web platform |
| License | MIT License[2](Apache License 2.0prior to 3.1.0)[3] |
| Website | getbootstrap.com |
| Repository | github.com/twbs/bootstrap |

  

**Bootstrap** (formerly **Twitter Bootstrap**) is a [free and open-source](./Free_and_open-source) [CSS framework](./CSS_framework) directed at responsive, [mobile-first](./Responsive_web_design#Related_concepts) [front-end web development](./Front-end_web_development). It contains [HTML](./HTML), [CSS](./CSS) and (optionally) [JavaScript](./JavaScript)-based design templates for [typography](./Web_design#Typography), [forms](./Form_(HTML)), [buttons](./Button_(computing)#HTML), [navigation](./Web_navigation#Local_website_navigation), and other interface components.

 

As of May 2023[[update]](https://en.wikipedia.org/w/index.php?title=Bootstrap_(front-end_framework)&action=edit), Bootstrap is the 17th most starred project (4th most starred library) on [GitHub](./GitHub), with over 164,000 stars.[[4]](./Bootstrap_(front-end_framework)#cite_note-most-starred-4) According to W3Techs, Bootstrap is used by 19.2% of all websites.[[5]](./Bootstrap_(front-end_framework)#cite_note-5)

 

## Features

 

Bootstrap is an HTML, CSS and JS library that focuses on simplifying the development of informative web pages (as opposed to [web applications](./Web_application)). The primary purpose of adding it to a web project is to apply Bootstrap's choices of color, size, font and layout to that project. As such, the primary factor is whether the developers in charge find those choices to their liking. Once added to a project, Bootstrap provides basic style definitions for all [HTML elements](./HTML_element). The result is a uniform appearance for prose, tables and form elements across [web browsers](./Web_browser). In addition, developers can take advantage of CSS classes defined in Bootstrap to further customize the appearance of their contents. For example, Bootstrap has provisioned for light- and dark-colored tables, page headings, more prominent [pull quotes](./Pull_quote), and text with a highlight.

 

Bootstrap also comes with several JavaScript components which do not require other libraries like [jQuery](./JQuery). They provide additional user interface elements such as [dialog boxes](./Dialog_box), [tooltips](./Tooltip), progress bars, navigation drop-downs, and carousels. Each Bootstrap component consists of an HTML structure, CSS declarations, and in some cases accompanying JavaScript code. They also extend the functionality of some existing interface elements, including for example an auto-complete function for input fields.

 [![Example of a webpage using Bootstrap framework](//upload.wikimedia.org/wikipedia/commons/thumb/d/da/Bootstrap_5_Example.png/250px-Bootstrap_5_Example.png)](./File:Bootstrap_5_Example.png)Example of a webpage using Bootstrap framework rendered in [Firefox](./Firefox) 

The most prominent components of Bootstrap are its layout components, as they affect an entire web page. The basic layout component is called "Container", as every other element in the page is placed in it. Developers can choose between a fixed-width container and a fluid-width container. While the latter always fills the width with the web page, the former uses one of the five predefined fixed widths, depending on the size of the screen showing the page:[[6]](./Bootstrap_(front-end_framework)#cite_note-6)

 
- Smaller than 576 pixels
- 576–768 pixels
- 768–992 pixels
- 992–1200 pixels
- 1200–1400 pixels
- Larger than 1400 pixels

 

Once a container is in place, other Bootstrap layout components implement a CSS Flexbox layout through defining rows and columns.

 

A precompiled version of Bootstrap is available in the form of one CSS file and three JavaScript files that can be readily added to any project. The raw form of Bootstrap, however, enables developers to implement further customization and size optimizations. This raw form is modular, meaning that the developer can remove unneeded components, apply a theme and modify the uncompiled [Sass](./Sass_(stylesheet_language)) files.

 

## History

 

### Early beginnings

 

Bootstrap, originally named Twitter Blueprint, was developed by Mark Otto and Jacob Thornton at [Twitter](./Twitter) in 2010 as a framework to encourage consistency across internal tools. Before Bootstrap, various libraries were used for interface development, which led to inconsistencies and a high maintenance burden. According to Otto:

 

A super small group of developers and I got together to design and build a new internal tool and saw an opportunity to do something more. Through that process, we saw ourselves build something much more substantial than another internal tool. Months later, we ended up with an early version of Bootstrap as a way to document and share common design patterns and assets within the company.[[7]](./Bootstrap_(front-end_framework)#cite_note-bootstrap_a_list_apart-7)

 

After a few months of development by a small group, many developers at Twitter began to contribute to the project as a part of Hack Week, a [hackathon](./Hackathon)-style week for the Twitter development team. It was renamed from Twitter Blueprint to Twitter Bootstrap and released as an open-source project on August 19, 2011.[[8]](./Bootstrap_(front-end_framework)#cite_note-v1-release-8) It has continued to be maintained by Otto, Thornton, a small group of core developers, and a large community of contributors.[[9]](./Bootstrap_(front-end_framework)#cite_note-about-9)

 

### Bootstrap 2

 

On January 31, 2012, Bootstrap 2 was released, which added built-in support for Glyphicons, several new components, as well as changes to many of the existing components. This version supports [responsive web design](./Responsive_web_design), meaning the layout of web pages adjusts dynamically, taking into account the characteristics of the device used (whether desktop, tablet, mobile phone).[[10]](./Bootstrap_(front-end_framework)#cite_note-v2-release-10) Shortly before the release of Bootstrap 2.1.2, Otto and Thornton left Twitter, but committed to continue to work on Bootstrap as an independent project.[[11]](./Bootstrap_(front-end_framework)#cite_note-11)

 

### Bootstrap 3

 

On August 19, 2013, Bootstrap 3 was released. It redesigned components to use [flat design](./Flat_design) and a [mobile first](./Responsive_web_design#Mobile_first,_unobtrusive_JavaScript,_and_progressive_enhancement) approach.[[12]](./Bootstrap_(front-end_framework)#cite_note-12) Bootstrap 3 features new plugin system with [namespaced](./Namespace) events. Bootstrap 3 dropped Internet Explorer 7 and Firefox 3.6 support, but there is an optional [polyfill](./Polyfill_(programming)) for these browsers.[[13]](./Bootstrap_(front-end_framework)#cite_note-v3-release-13) Bootstrap 3 was also the first version released under the twbs organization on GitHub instead of the Twitter one.[[14]](./Bootstrap_(front-end_framework)#cite_note-14)

 

### Bootstrap 4

 

Otto announced Bootstrap 4 on October 29, 2014.[[15]](./Bootstrap_(front-end_framework)#cite_note-v3.3.0-release-15) The first alpha version of Bootstrap 4 was released on August 19, 2015.[[16]](./Bootstrap_(front-end_framework)#cite_note-v4.0.0-alpha-release-16) The first beta version was released on August 10, 2017.[[17]](./Bootstrap_(front-end_framework)#cite_note-v4.0.0-beta-release-17) Otto suspended work on Bootstrap 3 on September 6, 2016, to free up time to work on Bootstrap 4. Bootstrap 4 was finalized on January 18, 2018.[[18]](./Bootstrap_(front-end_framework)#cite_note-18)

 

Significant changes include:

 
- Major rewrite of the code
- Replacing [Less](./Less_(stylesheet_language)) with [Sass](./Sass_(stylesheet_language))
- Addition of `Reboot`, a collection of element-specific CSS changes in a single file, based on `Normalize`
- Dropping support for [IE8](./Internet_Explorer_8), [IE9](./Internet_Explorer_9), and [iOS 6](./IOS_6)
- [CSS Flexible Box](./CSS_Flexible_Box_Layout) support
- Adding navigation customization options
- Adding responsive spacing and sizing utilities
- Switching from the [pixels](./Pixel) unit in CSS to [root ems](./Root_em)
- Increasing global font size from 14px to 16px for enhanced readability
- Dropping the `panel`, `thumbnail`, `pager`, and `well` components
- Dropping the `Glyphicons` icon font
- Huge number[*[quantify](./Wikipedia:Manual_of_Style/Dates_and_numbers)*] of utility classes
- Improved form styling, buttons, drop-down menus, media objects and image classes

 

Bootstrap 4 supports the latest versions of [Google Chrome](./Google_Chrome), [Firefox](./Firefox), [Internet Explorer](./Internet_Explorer), [Opera](./Opera_(web_browser)), and [Safari](./Safari_(web_browser)) (except on Windows). It additionally supports back to [IE10](./Internet_Explorer_10) and the latest [Firefox](./Firefox) Extended Support Release (ESR).[[19]](./Bootstrap_(front-end_framework)#cite_note-supported-browsers-19)

 

### Bootstrap 5

 

Bootstrap 5 was officially released on May 5, 2021.[[20]](./Bootstrap_(front-end_framework)#cite_note-20)[[21]](./Bootstrap_(front-end_framework)#cite_note-21)

 

**Major changes include:**[[22]](./Bootstrap_(front-end_framework)#cite_note-22)

 
- New offcanvas menu component
- Removing dependence on [jQuery](./JQuery) in favor of vanilla JavaScript
- Rewriting the grid to support responsive gutters and columns placed outside of rows
- Migrating the documentation from [Jekyll](./Jekyll_(software)) to [Hugo](./Hugo_(software))
- Dropping support for [Internet Explorer](./Internet_Explorer)[[23]](./Bootstrap_(front-end_framework)#cite_note-23)
- Moving testing infrastructure from [QUnit](./QUnit) to [Jasmine](./Jasmine_(JavaScript_testing_framework))
- Adding custom set of SVG icons[[24]](./Bootstrap_(front-end_framework)#cite_note-24)
- Adding CSS custom properties
- Improved API
- Enhanced grid system
- Improved customizing docs
- Updated forms
- RTL support
- Built in darkmode support

 

## See also

 
- ![](//upload.wikimedia.org/wikipedia/commons/thumb/3/31/Free_and_open-source_software_logo_%282009%29.svg/40px-Free_and_open-source_software_logo_%282009%29.svg.png)[Free and open-source software portal](./Portal:Free_and_open-source_software)

 
- [CSS framework](./CSS_framework)
- [jQuery Mobile](./JQuery_Mobile)
- [JavaScript framework](./JavaScript_framework)
- [JavaScript library](./JavaScript_library)
- [Tailwind CSS](./Tailwind_CSS)
- [Web framework](./Web_framework) — some support rendering in Bootstrap.[[25]](./Bootstrap_(front-end_framework)#cite_note-25)[[26]](./Bootstrap_(front-end_framework)#cite_note-26)

 

## References

  
1. [↑](./Bootstrap_(front-end_framework)#cite_ref-wikidata-da004572943d69132f6a36b52c6c747919706ae1-v20_1-0) ["Release v5.3.8"](https://github.com/twbs/bootstrap/releases/tag/v5.3.8). August 25, 2025. Retrieved August 25, 2025.
2. [↑](./Bootstrap_(front-end_framework)#cite_ref-2) ["bootstrap/LICENSE"](https://github.com/twbs/bootstrap/blob/main/LICENSE). *Github*.
3. [↑](./Bootstrap_(front-end_framework)#cite_ref-3) ["bootstrap/LICENSE (v3.0.3)"](https://github.com/twbs/bootstrap/blob/v3.0.3/LICENSE). *Github*.
4. [↑](./Bootstrap_(front-end_framework)#cite_ref-most-starred_4-0) ["Search · stars:>100000"](https://github.com/search?q=stars:%3E100000&type=repositories). *GitHub*. Retrieved December 4, 2022.
5. [↑](./Bootstrap_(front-end_framework)#cite_ref-5) ["Usage statistics and market share of Bootstrap for websites"](https://w3techs.com/technologies/details/cs-bootstrap). *w3techs.com*. Retrieved January 24, 2023.
6. [↑](./Bootstrap_(front-end_framework)#cite_ref-6) ["Bootstrap Containers · Bootstrap v5.0"](https://getbootstrap.com/docs/5.0/layout/containers/).
7. [↑](./Bootstrap_(front-end_framework)#cite_ref-bootstrap_a_list_apart_7-0) Otto, Mark (January 17, 2012). ["Bootstrap in A List Apart No. 342"](http://markdotto.com/2012/01/17/bootstrap-in-a-list-apart-342/). *Mark Otto's blog*. [Archived](https://web.archive.org/web/20161028153404/http://markdotto.com/2012/01/17/bootstrap-in-a-list-apart-342/) from the original on October 28, 2016. Retrieved February 23, 2017.
8. [↑](./Bootstrap_(front-end_framework)#cite_ref-v1-release_8-0) Otto, Mark (August 19, 2011). ["Bootstrap from Twitter"](https://blog.twitter.com/2011/bootstrap-twitter). *Developer Blog*. Twitter. [Archived](https://web.archive.org/web/20170223125113/https://blog.twitter.com/2011/bootstrap-twitter) from the original on February 23, 2017. Retrieved February 23, 2017.
9. [↑](./Bootstrap_(front-end_framework)#cite_ref-about_9-0) ["About"](https://getbootstrap.com/about/). *Bootstrap*. August 19, 2011. Retrieved February 23, 2017.
10. [↑](./Bootstrap_(front-end_framework)#cite_ref-v2-release_10-0) Otto, Mark (January 31, 2012). ["Say hello to Bootstrap 2.0"](https://blog.twitter.com/2012/say-hello-to-bootstrap-2). *Developer Blog*. Twitter. [Archived](https://web.archive.org/web/20170223125701/https://blog.twitter.com/2012/say-hello-to-bootstrap-2) from the original on February 23, 2017. Retrieved February 23, 2017.
11. [↑](./Bootstrap_(front-end_framework)#cite_ref-11) Otto, Mark (September 29, 2012). ["Onward"](https://blog.getbootstrap.com/2012/09/29/onward/). *blog.getbootstrap.com*.
12. [↑](./Bootstrap_(front-end_framework)#cite_ref-12) ["Bootstrap Blog - Bootstrap 3 released"](https://blog.getbootstrap.com/2013/08/19/bootstrap-3-released/). August 19, 2013.
13. [↑](./Bootstrap_(front-end_framework)#cite_ref-v3-release_13-0) Otto, Mark (August 19, 2013). ["Bootstrap 3 released"](https://blog.getbootstrap.com/2013/08/19/bootstrap-3-released/). [Archived](https://web.archive.org/web/20161021202024/http://blog.getbootstrap.com/2013/08/19/bootstrap-3-released/) from the original on October 21, 2016. Retrieved February 23, 2017.
14. [↑](./Bootstrap_(front-end_framework)#cite_ref-14) ["Bootstrap 3 plans"](https://blog.getbootstrap.com/2012/12/10/bootstrap-3-plans/). December 10, 2012.
15. [↑](./Bootstrap_(front-end_framework)#cite_ref-v3.3.0-release_15-0) Otto, Mark (October 29, 2014). ["Bootstrap 3.3.0 released"](https://blog.getbootstrap.com/2014/10/29/bootstrap-3-3-0-released/). [Archived](https://web.archive.org/web/20160724153923/http://blog.getbootstrap.com/2014/10/29/bootstrap-3-3-0-released/) from the original on July 24, 2016. Retrieved February 23, 2017.
16. [↑](./Bootstrap_(front-end_framework)#cite_ref-v4.0.0-alpha-release_16-0) Otto, Mark (August 19, 2015). ["Bootstrap 4 alpha"](https://blog.getbootstrap.com/2015/08/19/bootstrap-4-alpha/). [Archived](https://web.archive.org/web/20170123145832/http://blog.getbootstrap.com/2015/08/19/bootstrap-4-alpha/) from the original on January 23, 2017. Retrieved February 23, 2017.
17. [↑](./Bootstrap_(front-end_framework)#cite_ref-v4.0.0-beta-release_17-0) Otto, Mark; Thornton, Jacob (August 10, 2017). ["Bootstrap 4 Beta"](https://blog.getbootstrap.com/2017/08/10/bootstrap-4-beta/). Retrieved August 16, 2017.
18. [↑](./Bootstrap_(front-end_framework)#cite_ref-18) ["Bootstrap 4"](https://blog.getbootstrap.com/2018/01/18/bootstrap-4/). *blog.getbootstrap.com*. January 18, 2018. Retrieved February 5, 2021.
19. [↑](./Bootstrap_(front-end_framework)#cite_ref-supported-browsers_19-0) ["Supported browsers"](https://getbootstrap.com/getting-started/#support-browsers). *Bootstrap*. Retrieved February 23, 2017.
20. [↑](./Bootstrap_(front-end_framework)#cite_ref-20) ["Release Release v5.0.0 (#33647) · twbs/bootstrap"](https://github.com/twbs/bootstrap/releases/tag/v5.0.0). *GitHub*. Retrieved May 5, 2021.
21. [↑](./Bootstrap_(front-end_framework)#cite_ref-21) ["Bootstrap 5"](https://blog.getbootstrap.com/2021/05/05/bootstrap-5/). *blog.getbootstrap.com*. May 5, 2021.
22. [↑](./Bootstrap_(front-end_framework)#cite_ref-22) ["Bootstrap 5 grid by MartijnCuppens · Pull Request #28517 · twbs/bootstrap"](https://github.com/twbs/bootstrap/pull/28517). *GitHub*. Retrieved September 29, 2019.
23. [↑](./Bootstrap_(front-end_framework)#cite_ref-23) ["v5: drop Internet Explorer support by XhmikosR · Pull Request #30377 · twbs/bootstrap"](https://github.com/twbs/bootstrap/pull/30377). *GitHub*. Retrieved April 7, 2020.
24. [↑](./Bootstrap_(front-end_framework)#cite_ref-24) ["Bootstrap Icons"](https://icons.getbootstrap.com/). Retrieved November 7, 2022.
25. [↑](./Bootstrap_(front-end_framework)#cite_ref-25) ["Bootstrap-Flask"](https://github.com/helloflask/bootstrap-flask). HelloFlask. Retrieved November 7, 2022.
26. [↑](./Bootstrap_(front-end_framework)#cite_ref-26) ["Bootstrap-Django"](https://github.com/zelenij/django-bootstrap-v5). zelenij. Retrieved November 7, 2022.

 

## External links

   [![Wikimedia Commons logo](//upload.wikimedia.org/wikipedia/en/thumb/4/4a/Commons-logo.svg/40px-Commons-logo.svg.png)](./File:Commons-logo.svg) Wikimedia Commons has media related to [Bootstrap (framework)](https://commons.wikimedia.org/wiki/Category:Bootstrap%20(framework)).  
- [Official website](https://getbootstrap.com) [![Edit this at Wikidata](//upload.wikimedia.org/wikipedia/en/thumb/8/8a/OOjs_UI_icon_edit-ltr-progressive.svg/20px-OOjs_UI_icon_edit-ltr-progressive.svg.png)](https://www.wikidata.org/wiki/Q893195#P856)
- [Twbs](https://github.com/twbs) on [GitHub](./GitHub)

 
| Authority control databases | GND |
| --- | --- |