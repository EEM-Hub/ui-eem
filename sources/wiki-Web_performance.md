---
source: https://en.wikipedia.org/wiki/Web_performance
fetched: 2026-06-20
---

Speed web pages are downloaded and displayed 

**Web performance** refers to the speed in which [web pages](./Web_page) are downloaded and displayed on the user's [web browser](./Web_browser). **Web performance optimization (WPO)**, or **website optimization** is the field of knowledge about increasing web performance.

 

Faster website download speeds have been shown to increase visitor retention and loyalty[[1]](./Web_performance#cite_note-Google_Adds_Site_Speed_To_Search_Ranking-1)[[2]](./Web_performance#cite_note-WPO_|_Preparing_for_Cyber_Monday_Traffic-2) and user satisfaction, especially for users with slow internet connections and those on [mobile devices](./Mobile_device).[[3]](./Web_performance#cite_note-Web_First_for_Mobile-3) Web performance also leads to less data travelling across the web, which in turn lowers a website's power consumption and environmental impact.[[4]](./Web_performance#cite_note-Web_performance_optimization_for_everyone-4) Some aspects which can affect the speed of page load include browser/server cache, image optimization, and encryption (for example [SSL](./Transport_Layer_Security)), which can affect the time it takes for pages to render. The performance of the web page can be improved through techniques such as multi-layered cache, light weight design of [presentation layer](./Presentation_layer) components and [asynchronous communication](./Asynchronous_communication) with server side components.

 

## History

 

In the first decade or so of the web's existence, web performance improvement was focused mainly on optimizing website code and pushing hardware limitations. According to the 2002 book *Web Performance Tuning* by Patrick Killelea, some of the early techniques used were to use simple servlets or CGI, increase server memory, and look for [packet loss](./Packet_loss) and retransmission.[[5]](./Web_performance#cite_note-5) Although these principles now comprise much of the optimized foundation of internet applications, they differ from current optimization theory in that there was much less of an attempt to improve the browser display speed.

 

Steve Souders coined the term "web performance optimization" in 2004.[[6]](./Web_performance#cite_note-6) At that time Souders made several predictions regarding the impact that WPO as an "emerging industry" would bring to the web, such as websites being fast by default, consolidation, [web standards](./Web_standards) for performance, environmental impacts of optimization, and speed as a differentiator.[[7]](./Web_performance#cite_note-7)

 

One major point that Souders made in 2007 is that at least 80% of the time that it takes to download and view a website is controlled by the front-end structure. This lag time can be decreased through awareness of typical browser behavior, as well as of how [HTTP](./HTTP) works.[[8]](./Web_performance#cite_note-8)

 

## Optimization techniques

 

Web performance optimization improves [user experience](./User_experience) (UX) when visiting a website and therefore is highly desired by [web designers](./Web_designers) and [web developers](./Web_developers). They employ several techniques that streamline web optimization tasks to decrease web page load times. This process is known as front end optimization (FEO) or content optimization. FEO concentrates on reducing file sizes and "minimizing the number of requests needed for a given page to load."

 

In addition to the techniques listed below, the use of a [content delivery network](./Content_delivery_network)—a group of proxy servers spread across various locations around the globe—is an efficient delivery system that chooses a server for a specific user based on network proximity.[[9]](./Web_performance#cite_note-9) Typically the server with the quickest response time is selected.

 

The following techniques are commonly used web optimization tasks and are widely used by web developers:

 

Web browsers open separate [Transmission Control Protocol](./Transmission_Control_Protocol) (TCP) connections for each [Hypertext Transfer Protocol](./Hypertext_Transfer_Protocol) (HTTP) request submitted when downloading a web page. These requests total the number of page elements required for download. However, a browser is limited to opening only a certain number of simultaneous connections to a single host. To prevent bottlenecks, the number of individual page elements are reduced using resource consolidation whereby smaller files (such as images) are bundled together into one file. This reduces HTTP requests and the number of "round trips" required to load a web page.

 

Web pages are constructed from code files such [JavaScript](./JavaScript) and [Hypertext Markup Language](./Hypertext_Markup_Language) (HTML). As web pages grow in complexity, so do their code files and subsequently their load times. File compression can reduce code files by about 40 percent,[[10]](./Web_performance#cite_note-10) thereby improving site responsiveness.

 

[Web Caching Optimization](./Web_cache) reduces server load, bandwidth usage and [latency](./Latency_(engineering)). CDNs use dedicated web caching [software](./Software) to store copies of documents passing through their system. Many website platforms, such as [SiteGround](./SiteGround), [IONOS](./IONOS?action=edit&redlink=1), [Wix](./Wix.com), and [Hostinger](./Hostinger), rely on global CDNs and caching technologies to deliver faster page loads across different geographical regions.[[11]](./Web_performance#cite_note-11)[[12]](./Web_performance#cite_note-12)[[13]](./Web_performance#cite_note-13)

 

Subsequent requests from the cache may be fulfilled should certain conditions apply. Web caches are located on either the client side (forward position) or web-server side (reverse position) of a [CDN](./Content_delivery_network). Web browsers are also able to store content for re-use through the HTTP cache or [web cache](./Web_cache). Requests web browsers make are typically routed to the HTTP cache to validate if a cached response may be used to fulfill a request. If such a match is made, the response is fulfilled from the cache. This can be helpful for reducing network latency and costs associated with data-transfer. The HTTP cache is configured using request and response headers.

 

[Code minification](./Minification_(programming)) distinguishes discrepancies between codes written by web developers and how network elements interpret code. Minification removes comments and extra spaces as well as crunch variable names in order to minimize code, decreasing files sizes by as much as 60%. In addition to caching and compression, lossy [compression](./Image_compression) techniques (similar to those used with audio files) remove non-essential header information and lower original image quality on many high resolution images. These changes, such as [pixel](./Pixel) complexity or color gradations, are transparent to the end-user and do not noticeably affect perception of the image. Another technique is the replacement of [raster graphics](./Raster_graphics) with resolution-independent [vector graphics](./Vector_graphics). Vector substitution is best suited for simple geometric images.[*[citation needed](./Wikipedia:Citation_needed)*]

 

[Lazy loading](./Lazy_loading) of images and video reduces initial page load time, initial page weight, and [system resource](./System_resource) usage, all of which have positive impacts on website performance.[[14]](./Web_performance#cite_note-14) It is used to defer initialization of an object right until the point at which it is needed. The browser loads the images in a page or post when they are needed such as when the user scrolls down the page and not all images at once, which is the default behavior, and naturally, takes more time.

 

## HTTP/1.x and HTTP/2

 

Since web browsers use multiple TCP connections for parallel user requests, congestion and browser monopolization of network resources may occur. Because HTTP/1 requests come with associated [overhead](./Overhead_(computing)), web performance is impacted by limited bandwidth and increased usage.

 

Compared to HTTP/1, HTTP/2

 
- is [binary](./Binary_file) instead of textual
- is fully [multiplexed](./Multiplexing) instead of ordered and blocked
- can therefore use one connection for [parallelism](./Parallel_computing)
- uses [header](./Header_(computing)) compression to reduce overhead
- allows servers to "push" responses proactively into client caches[[15]](./Web_performance#cite_note-15)

 

Instead of a website's hosting server, CDNs are used in tandem with [HTTP/2](./HTTP/2) in order to better serve the end-user with web resources such as images, JavaScript files and [Cascading Style Sheet](./Cascading_Style_Sheet) (CSS) files since a CDN's location is usually in closer proximity to the end-user.[[16]](./Web_performance#cite_note-16)

 

## Metrics

 

In recent years, several metrics have been introduced that help developers measure various aspects of the performance of their websites. In 2019, [Google](./Google) introduced metrics such as Time to First Byte (TTFB), First Contentful Paint (FCP), First Paint (FP), First Input Delay (FID), Cumulative Layout Shift (CLS) and Largest Contentful Paint (LCP) allow for website owner to gain insights into issues that might hurt the performance of their websites making it seem sluggish or slow to the user. Other metrics including Request Count (number of requests required to load a page),[[17]](./Web_performance#cite_note-17) DOMContentLoaded (time when HTML document is completely loaded and parsed excluding CSS style sheets, images, etc.),[[18]](./Web_performance#cite_note-18) Above The Fold Time (content that is visible without scrolling),[[19]](./Web_performance#cite_note-:1-19) Round Trip Time,[[19]](./Web_performance#cite_note-:1-19) number of Render Blocking Resources (such as scripts, stylesheets),[[20]](./Web_performance#cite_note-20) Onload Time, Connection Time, Total Page Size help provide an accurate picture of latencies and slowdowns occurring at the networking level which might slow down a site.[[21]](./Web_performance#cite_note-:0-21)[[22]](./Web_performance#cite_note-22)[[23]](./Web_performance#cite_note-23)

 

Modules to measure metrics such as TTFB, FCP, LCP, FP etc are provided with major frontend JavaScript libraries such as [React](./React_(JavaScript_library)),[[24]](./Web_performance#cite_note-24) [NuxtJS](./Nuxt.js)[[25]](./Web_performance#cite_note-25) and [Vue](./Vue.js).[[26]](./Web_performance#cite_note-26) Google publishes a library, the core-web-vitals library that allows for easy measurement of these metrics in frontend applications. In addition to this, Google also provides the Lighthouse, a Chrome dev-tools component and PageSpeed Insight a site that allows developers to measure and compare the performance of their website with Google's recommended minimums and maximums.[[27]](./Web_performance#cite_note-27)

 

In addition to this, tools such as the Network Monitor by [Mozilla Firefox](./Mozilla_Firefox) help provide insight into network-level slowdowns that might occur during transmission of data.[[21]](./Web_performance#cite_note-:0-21)

 

## References

  
1. [↑](./Web_performance#cite_ref-Google_Adds_Site_Speed_To_Search_Ranking_1-0) ["Google Adds Site Speed To Search Ranking"](http://www.stevesouders.com/blog/2010/04/09/google-adds-site-speed-to-search-ranking/). Retrieved 4 December 2012.
2. [↑](./Web_performance#cite_ref-WPO_|_Preparing_for_Cyber_Monday_Traffic_2-0) Sharon, Bell. ["WPO | Preparing for Cyber Monday Traffic"](http://www.cdnetworks.com/blog/cyber-monday-web-performance-optimization/). *CDNetworks*. Retrieved 4 December 2012.
3. [↑](./Web_performance#cite_ref-Web_First_for_Mobile_3-0) Souders, Steve. ["Web First for Mobile"](http://www.stevesouders.com/blog/2012/05/16/web-first-for-mobile/). Retrieved 4 December 2012.
4. [↑](./Web_performance#cite_ref-Web_performance_optimization_for_everyone_4-0) Bellonch, Albert (10 October 2012). ["Web performance optimization for everyone"](https://www.slideshare.net/itnig/web-performance-optimization-for-everyone). Retrieved 4 December 2012.
5. [↑](./Web_performance#cite_ref-5) Killelea, Patrick (2002). [*Web Performance Tuning*](http://www.oreillynet.com/pub/a/javascript/2002/06/27/web_tuning.html). Sebastopol: O'Reilly Media. p. 480. [ISBN](./ISBN_(identifier)) [059600172X](./Special:BookSources/059600172X).
6. [↑](./Web_performance#cite_ref-6) Frick, Tim (2016). *Designing for Sustainability: A Guide to Building Greener Digital Products and Services*. Boston: O'Reilly Media. p. 195. [ISBN](./ISBN_(identifier)) [978-1491935774](./Special:BookSources/978-1491935774).
7. [↑](./Web_performance#cite_ref-7) Frick, Tim (2016). *Designing for Sustainability: A Guide to Building Greener Digital Products and Services*. Boston: O'Reilly Media. p. 56. [ISBN](./ISBN_(identifier)) [978-1491935774](./Special:BookSources/978-1491935774).
8. [↑](./Web_performance#cite_ref-8) Souders, Steve (2007). [*High Performance Websites*](https://web.archive.org/web/20190308213900/http://stevesouders.com/hpws/). Farnham: O'Reilly Media. p. 170. [ISBN](./ISBN_(identifier)) [978-0596529307](./Special:BookSources/978-0596529307). Archived from [the original](http://stevesouders.com/hpws/) on 8 March 2019.
9. [↑](./Web_performance#cite_ref-9) Saverimoutou, Antoine; Mathieu, Bertrand; Vaton, Sandrine (2019). ["Influence of Internet Protocols and CDN on Web Browsing"](https://imt-atlantique.hal.science/hal-02136202/file/ASaverimoutou-NTMS2019.pdf) (PDF). [*2019 10th IFIP International Conference on New Technologies, Mobility and Security (NTMS)*](https://hal-imt-atlantique.archives-ouvertes.fr/hal-02136202/file/ASaverimoutou-NTMS2019.pdf) (PDF). p. 6. [doi](./Doi_(identifier)):[10.1109/NTMS.2019.8763827](https://doi.org/10.1109%2FNTMS.2019.8763827). [ISBN](./ISBN_(identifier)) [978-1-7281-1542-9](./Special:BookSources/978-1-7281-1542-9).
10. [↑](./Web_performance#cite_ref-10) Sakamoto, Yasutaka; Matsumoto, Shinsuke; Tokunaga, Seiki; Saiki, Sachio; Nakamura, Masahide (February 2015). "Empirical study on effects of script minification and HTTP compression for traffic reduction". *2015 Third International Conference on Digital Information, Networking, and Wireless Communications (DINWC)*. IEEE. pp. 127–132. [doi](./Doi_(identifier)):[10.1109/DINWC.2015.7054230](https://doi.org/10.1109%2FDINWC.2015.7054230). [ISBN](./ISBN_(identifier)) [978-1-4799-6376-8](./Special:BookSources/978-1-4799-6376-8).
11. [↑](./Web_performance#cite_ref-11) Masoner, Liz (2024-12-19). ["10 Best Web Hosting Services Of 2025"](https://www.forbes.com/advisor/business/software/best-web-hosting-services/). *Forbes Advisor*. Retrieved 2026-01-28.
12. [↑](./Web_performance#cite_ref-12) ["Wix vs Squarespace 2026: I Tried Both Builders – My Verdict"](https://cybernews.com/best-website-builders/wix-vs-squarespace/). *Cybernews*. 2022-05-06. Retrieved 2026-01-28.
13. [↑](./Web_performance#cite_ref-13) ["Web Hosting Australia 2026: 9 Best Hosts Tested for Speed & Price"](https://cybernews.com/au/best-web-hosting/web-hosting-australia/). *Cybernews*. 2024-07-08. Retrieved 2026-01-28.
14. [↑](./Web_performance#cite_ref-14) ["Lazy loading - Web Performance | MDN"](https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading). *developer.mozilla.org*. Retrieved 2022-03-15.
15. [↑](./Web_performance#cite_ref-15) ["HTTP/2 Frequently Asked Questions"](https://http2.github.io/faq/). *HTTP Working Group*. Retrieved 14 April 2017.
16. [↑](./Web_performance#cite_ref-16) ["HTTP/2 – A Real-World Performance Test and Analysis"](https://css-tricks.com/http2-real-world-performance-test-analysis//). *CSS Tricks*. Retrieved 14 April 2017.
17. [↑](./Web_performance#cite_ref-17) *Mobile Web Performance Optimization*. 2015. [ISBN](./ISBN_(identifier)) [9781785284625](./Special:BookSources/9781785284625).
18. [↑](./Web_performance#cite_ref-18) Skvorc, Bruno; Perna, Maria Antonietta; Buckler, Craig; Curic, Ivan; Pitt, Christopher; Jankov, Tonino; Lavaryan, Reza; Berman, Daniel; Bouchefra, Ahmed; James, Hayden; Antolovic, Zoran; Ribeiro, Claudio (2018). *The Web Performance Collection*. SitePoint Pty. [ISBN](./ISBN_(identifier)) [9781492069805](./Special:BookSources/9781492069805).
19. [1](./Web_performance#cite_ref-:1_19-0) [2](./Web_performance#cite_ref-:1_19-1) Magazine, Smashing (24 September 2014). *Performance Optimization: Techniques And Strategies*. Smashing Magazine GmbH. [ISBN](./ISBN_(identifier)) [9783944540948](./Special:BookSources/9783944540948).
20. [↑](./Web_performance#cite_ref-20) Frain, Ben (2022). *Responsive Web Design with HTML5 and CSS*. Packt Publishing. [ISBN](./ISBN_(identifier)) [9781803231723](./Special:BookSources/9781803231723).
21. [1](./Web_performance#cite_ref-:0_21-0) [2](./Web_performance#cite_ref-:0_21-1) ["Measuring performance - Learn web development | MDN"](https://developer.mozilla.org/en-US/docs/Learn/Performance/Measuring_performance). *developer.mozilla.org*. Retrieved 2023-01-09.
22. [↑](./Web_performance#cite_ref-22) ["Measuring Web Performance in 2023: The Definitive Guide"](https://requestmetrics.com/web-performance/measure-web-performance). *Request Metrics*. Retrieved 2023-01-09.
23. [↑](./Web_performance#cite_ref-23) ["Front-End Performance Checklist 2021 (PDF, Apple Pages, MS Word)"](https://www.smashingmagazine.com/2021/01/front-end-performance-2021-free-pdf-checklist/). *Smashing Magazine*. 2021-01-12. Retrieved 2023-01-09.
24. [↑](./Web_performance#cite_ref-24) ["Measuring Performance | Create React App"](https://create-react-app.dev/docs/measuring-performance). *create-react-app.dev*. 20 June 2020. Retrieved 2023-01-09.
25. [↑](./Web_performance#cite_ref-25) ["@nuxtjs/web-vitals"](https://www.npmjs.com/package/@nuxtjs/web-vitals). *npm*. Retrieved 2023-01-09.
26. [↑](./Web_performance#cite_ref-26) ["vue-web-vitals"](https://www.npmjs.com/package/vue-web-vitals). *npm*. 22 May 2021. Retrieved 2023-01-09.
27. [↑](./Web_performance#cite_ref-27) ["User-centric performance metrics"](https://web.dev/user-centric-performance-metrics/). *web.dev*. Retrieved 2023-01-09.