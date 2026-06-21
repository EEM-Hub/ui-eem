---
source: https://en.wikipedia.org/wiki/Perceived_performance
fetched: 2026-06-20
---

|  | This articleneeds additional citations forverification.Please helpimprove this articlebyadding citations to reliable sources. Unsourced material may be challenged and removed.Find sources:"Perceived performance"–news·newspapers·books·scholar·JSTOR(December 2009)(Learn how and when to remove this message) |
| --- | --- |

 

**Perceived performance**, in [computer engineering](./Computer_engineering), refers to how quickly a [software feature](./Software_feature) appears to perform its task. The concept applies mainly to [user acceptance](./User_acceptance?action=edit&redlink=1) aspects.

 

The amount of time an application takes to start up, or a file to download, is not made faster by showing a startup screen (see [Splash screen](./Splash_screen)) or a file progress [dialog box](./Dialog_box). However, it satisfies some human needs: it *appears* faster to the user as well as providing a visual cue to let them know the system is handling their request.

 

In most cases, increasing real performance increases perceived performance, but when real performance cannot be increased due to physical limitations, techniques can be used to increase perceived performance at the cost of marginally decreasing real performance. For example, drawing and refreshing a [progress bar](./Progress_bar) while loading a file satisfies the user who is watching, but steals time from the process that is actually loading the file, but usually this is only a very small amount of time. All such techniques must exploit the inability of the user to accurately judge real performance, or they would be considered detrimental to performance.

 

Techniques for improving perceived performance may include more than just decreasing the delay between the user's request and visual feedback. Sometimes an increase in delay can be perceived as a performance improvement, such as when a variable controlled by the user is set to a running average of the users input. This can give the impression of smoother motion, but the controlled variable always reaches the desired value a bit late. Since it smooths out hi-frequency jitter, when the user is attempting to hold the value constant, they may feel like they are succeeding more readily. This kind of compromise would be appropriate for control of a sniper rifle in a video game. Another example may be doing trivial computation ahead of time rather than after a user triggers an action, such as pre-sorting a large list of data before a user wants to see it.

 

A technique to measure and interpret perceived performance remote systems is shown in a 2003[[1]](./Perceived_performance#cite_note-one-1) and updated in 2005 for virtual machines.[[2]](./Perceived_performance#cite_note-two-2)

 

## Web Performance

 

For [Web Performance](./Web_performance) optimization, perceived performance plays an important role. It tricks the user into thinking a site loads faster than it actually is. To achieve that, render-blocking resources will be loaded last in order to let the browser render the other elements first: like text content, images. In this way, even though the browser loads the same elements, by loading the non-blocking resources first, the user starts to see some content immediately. This trick improves the perceived performance, improving the overall [user experience](./User_experience).

 

Here are the main [perceived performance](https://developer.mozilla.org/en-US/docs/Learn/Performance/perceived_performance) steps for better user experiences:

 

**Minimize initial page load**

 

Load only the resources you need in order to display the first content seen by the user. After these resources are loaded, the rest of the resources can be loaded. 

 

**Interactive elements should be available**

 

Elements that are interactive, that the user can click on or interact with, should be able to perform those actions as soon as possible. Even with the rest of the page being still loaded, if the user can interact faster with the page, the user will perceive the site as being fast.

 

**Avoid rendering elements that can cause flicker on screen**

 

Elements like fonts or content that takes longer to load should be avoided as much as possible. When loading fonts, try to adjust their size and appearance closer to the default browser styles. In this way, when the font will be loaded, the switch won't look weird and be obvious. For images, charts, or embedded content, make sure you have a placeholder that has the same with and height. In this way when the content comes, the screen won't flicker and the height of the page won't change.

 

### Tools

 

In order to improve the perceived performance of a web page, there are numerous tools that can be helpful:

 

[Google Chrome](./Google_Chrome): DevTools provides ways to measure the performance of a site giving you insights on how to improve.

 

[Webpagetest](https://www.webpagetest.org/) - SpeedIndex represents the average time it takes for the visible part of a site to be displayed. 

 

## References

  
1. [↑](./Perceived_performance#cite_ref-one_1-0) [Perceived Performance](http://www.tmurgent.com/WhitePapers/PerceivedPerformance.pdf)
2. [↑](./Perceived_performance#cite_ref-two_2-0) [Perceived Performance and Virtual Operating Systems](http://www.tmurgent.com/WhitePapers/PerceivedPerformance_VirtualOS.pdf)