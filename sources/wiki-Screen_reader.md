---
source: https://en.wikipedia.org/wiki/Screen_reader
fetched: 2026-06-20
---

Assistive technology that converts text or images to speech or Braille 
|  | This articleneeds additional citations forverification.Please helpimprove this articlebyadding citations to reliable sources. Unsourced material may be challenged and removed.Find sources:"Screen reader"–news·newspapers·books·scholar·JSTOR(July 2017)(Learn how and when to remove this message) |
| --- | --- |

 

 An example of someone using a screen reader showing documents that are inaccessible, readable and accessible 

A **screen reader** is a form of [assistive technology](./Assistive_technology) (AT)[[1]](./Screen_reader#cite_note-1) that renders text and image content as speech or braille output. Screen readers are essential to [blind](./Blindness) people,[[2]](./Screen_reader#cite_note-afb-2) and are also useful to people who are [visually impaired](./Visually_impaired),[[2]](./Screen_reader#cite_note-afb-2) [illiterate](./Illiteracy) or [learning-disabled](./Learning_disability).[[3]](./Screen_reader#cite_note-Screen1-3) Screen readers are [software applications](./Application_software) that attempt to convey what people with normal eyesight see on a [display](./Display_device) to their users via non-visual means, like [text-to-speech](./Text-to-speech),[[4]](./Screen_reader#cite_note-4) [earcons](./Earcon),[[5]](./Screen_reader#cite_note-5) or a [braille device](./Refreshable_Braille_display).[[2]](./Screen_reader#cite_note-afb-2) They do this by applying a wide variety of techniques that include, for example, interacting with dedicated [accessibility APIs](./Screen_reader#Accessibility_APIs), using various [operating system](./Operating_system) features (like [inter-process communication](./Inter-process_communication) and querying [user interface](./User_interface) properties), and employing [hooking](./Hooking) techniques.[[6]](./Screen_reader#cite_note-SR_Overview-6)

 

[Microsoft Windows](./Microsoft_Windows) [operating systems](./Operating_systems) have included the [Microsoft Narrator](./Microsoft_Narrator) screen reader since [Windows 2000](./Windows_2000), though separate products such as [Freedom Scientific](./Freedom_Scientific)'s commercially available [JAWS](./JAWS_(screen_reader)) screen reader and [ZoomText](./ZoomText) screen magnifier and the [free and open source](./Free_and_open_source) screen reader [NVDA](./NonVisual_Desktop_Access) by NV Access are more popular for that operating system.[[7]](./Screen_reader#cite_note-7) [Apple Inc.](./Apple_Inc.)'s [macOS](./MacOS), [iOS](./IOS), and [tvOS](./TvOS) include [VoiceOver](./VoiceOver) as a built-in screen reader, while [Google](./Google)'s [Android](./Android_(operating_system)) provides the [Talkback screen reader](./Google_TalkBack) and its [ChromeOS](./ChromeOS) can use ChromeVox.[[8]](./Screen_reader#cite_note-8) Similarly, Android-based devices from Amazon provide the VoiceView screen reader.  There are also free and open source screen readers for [Linux](./Linux) and [Unix-like](./Unix-like) systems, such as Speakup and [Orca](./Orca_(assistive_technology)).

 

## History

 

Around 1978, Al Overby of IBM Raleigh developed a prototype of a talking terminal, known as SAID (for Synthetic Audio Interface Driver), for the [IBM 3270 terminal](./IBM_3270).[[9]](./Screen_reader#cite_note-9) SAID read the ASCII values of the display in a stream and spoke them through a large vocal track synthesizer the size of a suitcase, and it cost around $10,000.[[10]](./Screen_reader#cite_note-:0-10) Dr. Jesse Wright, a blind research mathematician, and [Jim Thatcher](./James_W._Thatcher), formerly his graduate student from the University of Michigan, working as mathematicians for IBM, adapted this as an internal IBM tool for use by blind people. After the early [IBM Personal Computer (PC)](./IBM_Personal_Computer) was released in 1981, Thatcher and Wright developed a software equivalent to SAID, called PC-SAID, or *Personal Computer Synthetic Audio Interface Driver*. This was renamed and released in 1984 as IBM Screen Reader, which became the [proprietary eponym](./Generic_trademark) for that general class of assistive technology.[[10]](./Screen_reader#cite_note-:0-10)

 

## Types

 

### Command-line (text)

 

In early [operating systems](./Operating_system), such as [MS-DOS](./MS-DOS), which employed [command-line interfaces](./Command-line_interface) (CLIs), the screen display consisted of [characters](./Character_(computing)) [mapping](./Memory-mapped_I/O) directly to a [screen buffer](./Screen_buffer) in [memory](./Computer_memory) and a [cursor](./Cursor_(computers)) position. Input was by keyboard. All this information could therefore be obtained from the system either by [hooking](./Hooking) the flow of information around the system and reading the screen buffer or by using a standard hardware output socket[[11]](./Screen_reader#cite_note-11) and communicating the results to the user.

 

In the 1980s, the Research Centre for the Education of the Visually Handicapped (RCEVH) at the [University of Birmingham](./University_of_Birmingham) developed a Screen Reader for the [BBC Micro](./BBC_Micro) and abbr?NEC Portable.[[12]](./Screen_reader#cite_note-12)[[13]](./Screen_reader#cite_note-13)

 

### Graphical

 

#### Off-screen models

 

With the arrival of [graphical user interfaces](./Graphical_user_interface) (GUIs), the situation became more complicated. A GUI has characters and graphics drawn on the screen at particular positions, and therefore there is no purely textual representation of the graphical contents of the display. Screen readers were therefore forced to employ new low-level techniques, gathering messages from the [operating system](./Operating_system) and using these to build up an "off-screen model", a representation of the display in which the required text content is stored.[[14]](./Screen_reader#cite_note-14)

 

For example, the operating system might send messages to draw a command button and its caption. These messages are intercepted and used to construct the off-screen model. The user can switch between controls (such as buttons) available on the screen and the captions and control contents will be read aloud and/or shown on a [refreshable braille display](./Refreshable_braille_display).

 

Screen readers can also communicate information on menus, controls, and other visual constructs to permit blind users to interact with these constructs. However, maintaining an off-screen model is a significant technical challenge; hooking the low-level messages and maintaining an accurate model are both difficult tasks.[*[citation needed](./Wikipedia:Citation_needed)*]

 

#### Accessibility APIs

 

Operating system and application designers have attempted to address these problems by providing ways for screen readers to access the display contents without having to maintain an off-screen model. These involve the provision of alternative and accessible representations of what is being displayed on the screen accessed through an [API](./Application_programming_interface). Existing APIs include:

 
- Android Accessibility Framework[[15]](./Screen_reader#cite_note-15)
- Apple Accessibility API[[16]](./Screen_reader#cite_note-16)
- [AT-SPI](./AT-SPI)
- [IAccessible2](./IAccessible2)
- [Microsoft Active Accessibility](./Microsoft_Active_Accessibility) (MSAA)
- [Microsoft UI Automation](./Microsoft_UI_Automation)
- [Java Access Bridge](./Java_Access_Bridge)[[17]](./Screen_reader#cite_note-17)

 

Screen readers can query the operating system or application for what is currently being displayed and receive updates when the display changes. For example, a screen reader can be told that the current focus is on a button and the button caption is to be communicated to the user. This approach is considerably easier for the developers of screen readers, but fails when applications do not comply with the accessibility API. One approach when the accessibility API is insufficient is to use available operating system messages and application object models to supplement accessibility APIs.

 

Screen readers can be assumed to be able to access all display content that is not intrinsically inaccessible. Web browsers, word processors, icons and windows and email programs are just some of the applications used successfully by screen reader users. However, according to some users,[*[who?](./Wikipedia:Manual_of_Style/Words_to_watch#Unsupported_attributions)*] using a screen reader is considerably more difficult than using a GUI, and many applications have specific problems resulting from the nature of the application (e.g. animations) or failure to comply with accessibility standards for the platform.[*[citation needed](./Wikipedia:Citation_needed)*]

 

## Customization

 

Most screen readers allow the user to select whether most [punctuation](./Punctuation) is announced or silently ignored. Some screen readers can be tailored to a particular application through [**scripting**](./Script_(computing)). One advantage of scripting is that it allows customizations to be shared among users, increasing accessibility for all. [JAWS](./Job_Access_With_Speech) enjoys an active script-sharing community, for example.[[18]](./Screen_reader#cite_note-18)

 

### Verbosity

 

Verbosity is a feature of screen reading software that supports vision-impaired computer users. Speech verbosity controls enable users to choose how much speech feedback they wish to hear. Specifically, verbosity settings allow users to construct a mental model of web pages displayed on their computer screen. Based on verbosity settings, a screen-reading program informs users of certain formatting changes, such as when a frame or table begins and ends, where graphics have been inserted into the text, or when a list appears in the document. The verbosity settings can also control the level of descriptiveness of elements, such as lists, tables, and regions.[[19]](./Screen_reader#cite_note-19) For example, [JAWS](./JAWS_(screen_reader)) provides low, medium, and high web verbosity preset levels. The high web verbosity level provides more detail about the contents of a webpage.[[20]](./Screen_reader#cite_note-20)

 

### Language

 

Some screen readers can read text in more than one [language](./Language), provided that the language of the material is encoded in its [metadata](./Metadata_Encoding_and_Transmission_Standard).[[21]](./Screen_reader#cite_note-21)

 

## See also

 
- [List of screen readers](./List_of_screen_readers)
- [Screen magnifier](./Screen_magnifier)
- [Speech processing](./Speech_processing)
- [Speech recognition](./Speech_recognition)
- [Speech synthesis](./Speech_synthesis)
- [Vinux](./Vinux)
- [VoiceOver](./VoiceOver)

 

## References

   [![Wiktionary logo](//upload.wikimedia.org/wikipedia/commons/thumb/9/99/Wiktionary-logo-en-v2.svg/40px-Wiktionary-logo-en-v2.svg.png)](./File:Wiktionary-logo-en-v2.svg) Look up ***[screen reader](https://en.wiktionary.org/wiki/Special:Search/screen%20reader)*** in Wiktionary, the free dictionary.   
1. [↑](./Screen_reader#cite_ref-1) ["Types of Assistive Technology Products"](https://www.microsoft.com/enable/at/types.aspx). Microsoft Accessibility. Retrieved June 13, 2016.
2. [1](./Screen_reader#cite_ref-afb_2-0) [2](./Screen_reader#cite_ref-afb_2-1) [3](./Screen_reader#cite_ref-afb_2-2) ["Screen reading technology"](https://www.afb.org/blindness-and-low-vision/using-technology/assistive-technology-videos/screen-reading-technology). [AFB](./American_Foundation_for_the_Blind). Retrieved February 23, 2022.
3. [↑](./Screen_reader#cite_ref-Screen1_3-0) ["Screen Readers and how they work with E-Learning"](https://web.archive.org/web/20181113075826/https://www.vadsa.org/ace/reader.htm). Virginia.gov. Archived from [the original](http://www.vadsa.org/ace/reader.htm) on November 13, 2018. Retrieved March 31, 2019.
4. [↑](./Screen_reader#cite_ref-4) ["Hear text read aloud with Narrator"](http://windows.microsoft.com/en-us/windows/hear-text-read-aloud-narrator#1TC=windows-8). [Microsoft](./Microsoft_Office). Retrieved June 13, 2016.
5. [↑](./Screen_reader#cite_ref-5) ["iCons and Earcons: Critical but often overlooked tech skills"](https://www.perkins.org/resource/icons-and-earcons-critical-often-overlooked-tech-skills/). [Perkins School for the Blind](./Perkins_School_for_the_Blind). March 21, 2023. Retrieved January 10, 2026.
6. [↑](./Screen_reader#cite_ref-SR_Overview_6-0) ["What is a Screen Reader"](https://www.nomensa.com/blog/2005/what-screen-reader). [Nomensa](./Nomensa?action=edit&redlink=1). Retrieved July 9, 2017.
7. [↑](./Screen_reader#cite_ref-7) ["Screen Reader User Survey #9"](https://webaim.org/projects/screenreadersurvey9/). [WebAIM](./WebAIM). Retrieved July 1, 2021.
8. [↑](./Screen_reader#cite_ref-8) ["ChromeVox"](http://www.chromevox.com/). Google. Retrieved March 9, 2020.
9. [↑](./Screen_reader#cite_ref-9) Cooke, Annemarie (March 2004). ["A History of Accessibility at IBM"](https://www.afb.org/aw/5/2/14760). *The American Foundation for the Blind (AFB)*.
10. [1](./Screen_reader#cite_ref-:0_10-0) [2](./Screen_reader#cite_ref-:0_10-1) ["Making A Difference Award (2009) — Jim Thatcher (interview)"](https://www.sigcas.org/2018/02/08/making-a-difference-award-2009-jim-thatcher-interview/). *SIGCAS, the Association for Computing Machinery Special Interest Group for Computers and Society*. 2009.
11. [↑](./Screen_reader#cite_ref-11) ["Talking Terminals. BYTE, September 1982"](https://web.archive.org/web/20060625225004/http://www.edstoffel.com/david/talkingterminals.html). Archived from [the original](http://www.edstoffel.com/david/talkingterminals.html) on June 25, 2006. Retrieved September 7, 2006.
12. [↑](./Screen_reader#cite_ref-12) Paul Blenkhorn, "The RCEVH project on micro-computer systems and computer assisted learning", British Journal of Visual Impairment, 4/3, 101-103 (1986). [Free HTML version at Visugate](http://www.visugate.biz/bjvi/1986/autumn1986.html#RCEVH) [Archived](https://web.archive.org/web/20070928210916/http://www.visugate.biz/bjvi/1986/autumn1986.html#RCEVH) September 28, 2007, at the [Wayback Machine](./Wayback_Machine).
13. [↑](./Screen_reader#cite_ref-13) ["Access to personal computers using speech synthesis. RNIB New Beacon No.76, May 1992"](http://www.rnib.org.uk/information-everyday-living-using-technology-beginners-guides/beginners-guide-assistive-technology). March 3, 2014.
14. [↑](./Screen_reader#cite_ref-14) According to "[Making the GUI Talk](ftp://service.boulder.ibm.com/sns/sr-os2/sr2doc/guitalk.txt)[*[dead link](./Wikipedia:Link_rot)*]" (by Richard Schwerdtfeger, *BYTE* December 1991, p. 118-128), the first screen reader to build an off-screen model was outSPOKEN.
15. [↑](./Screen_reader#cite_ref-15) [Implementing Accessibility on Android](https://developer.android.com/training/accessibility/index.html).
16. [↑](./Screen_reader#cite_ref-16) [Apple Accessibility API](https://developer.apple.com/documentation/Accessibility/Reference/AccessibilityLowlevel/index.html).
17. [↑](./Screen_reader#cite_ref-17) ["Oracle Technology Network for Java Developers – Oracle Technology Network – Oracle"](http://java.sun.com/products/accessbridge/).
18. [↑](./Screen_reader#cite_ref-18) ["An Introduction to JAWS Scripting"](https://afb.org/aw/4/6/14806). *AccessWorld (American Foundation for the Blind)*.
19. [↑](./Screen_reader#cite_ref-19) Zong, Jonathan; Lee, Crystal; Lundgard, Alan; Jang, JiWoong; Hajas, Daniel; Satyanarayan, Arvind (2022). "Rich Screen Reader Experiences for Accessible Data Visualization". *Computer Graphics Forum*. **41** (3): 15–27. [arXiv](./ArXiv_(identifier)):[2205.04917](https://arxiv.org/abs/2205.04917). [doi](./Doi_(identifier)):[10.1111/cgf.14519](https://doi.org/10.1111%2Fcgf.14519). [ISSN](./ISSN_(identifier)) [0167-7055](https://search.worldcat.org/issn/0167-7055). [S2CID](./S2CID_(identifier)) [248665696](https://api.semanticscholar.org/CorpusID:248665696).
20. [↑](./Screen_reader#cite_ref-20) ["JAWS Web Verbosity"](https://support.freedomscientific.com/SurfsUp/7-WebVerbosity.htm). *www.freedomscientific.com*. Retrieved February 19, 2026.
21. [↑](./Screen_reader#cite_ref-21) Chris Heilmann (March 13, 2008). ["Yahoo! search results now with natural language support"](https://developer.yahoo.com/blogs/ydn/yahoo-search-results-now-natural-language-support-7318.html). *[Yahoo! Developer Network](./Yahoo!_Developer_Network) Blog*. [Archived](https://web.archive.org/web/20090125024422/http://developer.yahoo.net/blog/archives/2008/03/yahoo_search_re.html) from the original on January 25, 2009. Retrieved February 28, 2015.