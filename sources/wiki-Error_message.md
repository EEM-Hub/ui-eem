---
source: https://en.wikipedia.org/wiki/Error_message
fetched: 2026-06-20
---

Information describing a problematic situation [![](//upload.wikimedia.org/wikipedia/commons/thumb/5/51/System_Message_%22Visualeditor-dialog-error%22_pop-up.png/250px-System_Message_%22Visualeditor-dialog-error%22_pop-up.png)](./File:System_Message_"Visualeditor-dialog-error"_pop-up.png)An error message when attempting to use the Wikipedia Visual editor 

In [computing](./Computing), an **error message** is a relatively short [text](./Plain_text) message that describes a problematic situation. An error message generally indicates that an operation failed and may imply if not direct the [user](./User_(computing)) to a corrective action.

 

An error message is a classification of information reported by [software](./Software). Other information can be classified as a warning to describe a potential problem or as purely informational (not about a problem). Additionally, not all error information is classified as an error message. For example, a [core dump](./Core_dump) or a [stack trace](./Stack_trace) may be reported about an error condition, but although they are a form of error information, they are not considered error messages. A more abstract representation of an error is sometimes used instead of a message such as  an [indicator light](./Light-emitting_diode) or a [numeric display](./Seven-segment_display) which may require the user to consult [documentation](./Documentation) to interpret the error.

 

An error message can be reported in a variety of ways. For example, in a [graphical user interface](./Graphical_user_interface) (GUI), an error message may be displayed in a dialog box. In a [command-line interface](./Command-line_interface) (CLI), an error message may be printed to a [standard stream](./Standard_stream). A [program](./Computer_program) may write an error message to a [log file](./Log_file).[[1]](./Error_message#cite_note-1)

 

The proper design of error messages is an important aspect of [usability](./Usability) and [human–computer interaction](./Human–computer_interaction).[[2]](./Error_message#cite_note-2) When the content of an error message is misleading or wrong, the user struggles to correct the issue and to complete their desired task.

 

## Presentation

 

While graphical user interfaces have different conventions for displaying error messages, several techniques are common.

 Modal dialog box (a.k.a. pop-up message)Appears in a window on the screen, blocking further interaction until it is dismissed. Notification iconAn icon appears to notify the user about a condition without interrupting their work (not modal). On Windows, a notification icon appears in the [System Tray](./System_Tray).  On Mac OS X, a notification icon may appear in the menu bar, or may take the form of an application's icon "bouncing" in the Dock. The [GNOME](./GNOME) user interface for Unix-based systems can display notification icons in a panel. Status barRelatively short error messages may be displayed in a status bar which is generally at the bottom of an application's window. 

## Content

 

The three main factors that influence the design of error messages are technical limitations, the amount of information to be presented, and what kind of user input is required.[[3]](./Error_message#cite_note-3)

 

Some systems have technical limitations that may constrain the amount of information an error message can contain.  For example, a printer with a sixteen-character alphanumeric display can only show a very limited amount of information at once, so it may need to display very terse error messages.  Even with computer monitors, the programmer must consider the smallest monitor that a user might reasonably use, and ensure that any error messages will fit on that screen.

 

The nature of the error determines the amount of information required to effectively convey the error message. A complex issue may require a more detailed error message in order to adequately inform the user of the problem.

 

In general, software designers should take care that the content of a messages does not expose security risk. An error message should not expose information that can be exploited by a [cracker](./Software_cracking) to obtain information that is otherwise difficult to obtain. Examples are [systems](./Software_systems) which may show either "invalid user" or "invalid password" depending on which is incorrect, and the error page in the [web server](./Web_server) [IIS 5.0](./Internet_Information_Services) which provides a complete technical description of the error including a source code fragment.

 

## Examples

 

### Common errors

 

The following error conditions are often reported via an error message. When such a condition occurs, the section header text might be reported as an error message and in fact is in some contexts, but different text is used for the condition in other contexts.

 Access deniedThe user does not have privilege to complete an operation. Device not readyMost often occurs when there is no [floppy disk](./Floppy_disk) (or a bad disk) in the disk drive and the system tries to a access that disk. Disk Boot FailureCommonly occurs when the hard drive of the computer is having problems. If the computer can boot from a network, it may instead display the message "Media test failure, check cable". File not foundA specified file is not found as specified. A similar error occurs on the web as [ HTTP status code 404](./HTTP_404) to indicate that a resource is not found. Low Disk SpaceThis condition occurs when a [storage drive](./Data_storage) is nearly full. To fix this, the user should release storage space (i.e. delete files) or use a different drive. [Out of memory](./Out_of_memory)The system has insufficient [RAM](./Random-access_memory) for an operation. Fixes include closing programs and installing more memory. Resource not found[HTTP status code 404](./HTTP_404) usually results from a link to a page that has been moved or deleted, or a mistyped [URL](./URL). 

### Specific error messages

 

Notable error messages in specific computing contexts include:

 ?the [ed text editor](./Ed_(text_editor)) infamously replies with a single question mark for nearly all error conditions. [Abort, Retry, Fail?](./Abort,_Retry,_Fail%3F)A notoriously confusing error message seen in [MS-DOS](./MS-DOS) [![](//upload.wikimedia.org/wikipedia/commons/4/46/Error_Message_Example_vbs.png)](./File:Error_Message_Example_vbs.png)An example of an Error message .vbs script [Bad command or file name](./Bad_command_or_file_name)A notoriously common and confusing error message seen in [MS-DOS](./MS-DOS_4.0_(multitasking)) [Blue Screen of Death](./Blue_Screen_of_Death) (BSoD)In [Windows](./Windows) and [ReactOS](./ReactOS), this screen appears when the operating system encounters a severe error.[[4]](./Error_message#cite_note-:0-4) It is roughly analogous to a [kernel panic](./Kernel_panic) on [Linux](./Linux), [Unix](./Unix), or [macOS](./MacOS). [Guru Meditation](./Guru_Meditation)In [Amiga](./Amiga), roughly analogous to a kernel panic or BSoD, also adopted by more recent products such as [VirtualBox](./VirtualBox). [lp0 on fire](./Lp0_on_fire)A Unix warning that the printer may be "on fire", literally or not.[*[dubious](./Wikipedia:Accuracy_dispute#Disputed_statement) – [discuss](./Talk:Error_message#doubt_that_it's_literal)*] [Not a typewriter](./Not_a_typewriter)A Unix error message that is confusing due to its now obsolete use of the word "[typewriter](./Typewriter)", and which is sometimes output when the nature of the error is seemingly entirely different. [PC LOAD LETTER](./PC_LOAD_LETTER)An error on several HP laser printers that simply asked the user to add "Letter" size paper in a confusing way.[[5]](./Error_message#cite_note-5) [SYNTAX ERROR](./Syntax_error)Seen in many older computing contexts when the received instruction is not understood. Error 1603A problem during installation of a [computer program](./Computer_program). This error particularly occurs on [Windows](./Windows) computer systems. *application* has stoppedAn error message commonly found on [Android](./Android_(operating_system)) devices, that indicates that an application unexpectedly stopped working or crashed. SuccessIn [POSIX](./POSIX) and other contexts, success is sometimes and confusingly reported as an error. This is a form of sloppy error handling resulting from reporting a success status code as an error. 

### Fail pets

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/8/8c/Tumbeasts_servers.png/250px-Tumbeasts_servers.png)](./File:Tumbeasts_servers.png)Tumbeasts gnawing on servers, used by Tumblr in 2011 

With the rise of Web 2.0 services such as [Twitter](./Twitter), end-user facing error messages such as [HTTP 404](./HTTP_404) and [HTTP 500](./HTTP_500) started to be displayed with whimsical characters, termed Fail Pets or Error Mascots. The term "Fail Pet" was coined, or at least first used in print, by Mozilla Engineer Fred Wenzel in a post on his blog entitled "Why [Wikipedia](./Wikipedia) might need a fail-pet — and why Mozilla does not."[[6]](./Error_message#cite_note-6) Dr. Sean Rintel argues that error messages are a critical strategic moment in [brand awareness](./Brand_awareness) and loyalty. Fail pets are of interest to marketers because they can result in brand recognition (especially through [earned media](./Earned_media)). "However, that same recognition carries the danger of highlighting service failure."[[7]](./Error_message#cite_note-7) The most famous fail pet is Twitter's [Fail Whale](./Fail_Whale) (see [Twitter](./Twitter) service outages). Other fail pets include:

 
- [Ars Technica](./Ars_Technica): Moon Shark (March 3, 2013)
- [Chuck E. Cheese](./Chuck_E._Cheese): Chuck E. jumping
- [Facebook](./Facebook): Thumbs up with bandage
- [FarmVille](./FarmVille) on Facebook: Sad cow.
- [GitHub](./GitHub): Octocat
- [Google](./Google): Broken robot (March 2, 2011)
- [iCloud](./ICloud): Cloud with [Apple System 7](./System_7) emoticon-style face and a magnifying glass
- [Macintosh](./Macintosh): [Sad Mac](./Macintosh_startup#Sad_Mac)
- [Palliser Furniture](./Palliser_Furniture): Between the cushions (January 31, 2018)
- [Tumblr](./Tumblr): Tumbeasts (January 25, 2011)
- [Twitter](./Twitter): Fail Whale / Twitter Robot (July 30, 2008)
- [YouTube](./YouTube): Televisions (on main site), light static inside video window (embedded video), Monkey
- [Cartoon Network](./Cartoon_Network): [BMO](./BMO_(Adventure_Time)) from *[Adventure Time](./Adventure_Time)*, Domo in Asian regions
- [Google Chrome](./Google_Chrome): T-Rex
- [Patreon](./Patreon): [Red fox](./Red_fox) with a helmet floating in [space](./Outer_space)
- [VK](./VK_(service)): Sad VK dog
- [Scratch](./Scratch_(programming_language)): Giga scratching their head

 

## See also

 
- [Alert dialog box](./Alert_dialog_box) – Computer interface element
- [Definitive diagnostic data](./Definitive_diagnostic_data)
- [Does not compute](./Does_not_compute) – Phrase often uttered by computers and robots in popular culture
- [Exception handling](./Exception_handling) – Programming language construct for special conditions
- [Interaction design](./Interaction_design) – Specialization of design focused on the experience users have of a product or service
- [Medium error](./Medium_error)
- [User error](./User_error) – Error made by the human user of a complex system
- [User interface design](./User_interface_design) – Planned operator–machine interaction

 

## References

  
1. [↑](./Error_message#cite_ref-1) Raskin, Jef (2000). ["6-4-2: Messages to the User"](https://books.google.com/books?id=D39vjmLfO3kC&pg=PA178). *The Humane Interface: New Directions for Designing Interactive Systems*. ACM Press Series. Addison-Wesley. p. 178. [ISBN](./ISBN_(identifier)) [978-0-201-37937-2](./Special:BookSources/978-0-201-37937-2).
2. [↑](./Error_message#cite_ref-2) Minhas, Saadis (May 30, 2018). ["How to Write Good Error Messages"](https://web.archive.org/web/20220914063305/https://uxplanet.org/how-to-write-good-error-messages-858e4551cd4). *UX*. Archived from [the original](https://uxplanet.org/how-to-write-good-error-messages-858e4551cd4) on September 14, 2022. Retrieved Jan 30, 2019.
3. [↑](./Error_message#cite_ref-3) ["Non-Fatal Errors: Creating usable, effective error messages"](https://web.archive.org/web/20090508152354/http://winwriters.com/articles/message/index.html). Archived from [the original](http://www.winwriters.com/articles/message/index.html) on 2009-05-08. Retrieved 2007-02-16.
4. [↑](./Error_message#cite_ref-:0_4-0) Fisher, Tim (2019-01-16). ["Blue Screens of Death (BSOD): Everything You Need to Know"](https://www.lifewire.com/blue-screen-of-death-bsod-2625816). *Lifewire*. Retrieved 2019-01-30.
5. [↑](./Error_message#cite_ref-5) McNamara, Paul (2009-04-29). ["LaserJet turns 25 ... 'PC LOAD LETTER' still unfathomable"](https://www.networkworld.com/article/764169/data-center-laserjet-turns-25-pc-load-letter-still-unfathomable.html). *Network World*. Retrieved 2019-01-30.
6. [↑](./Error_message#cite_ref-6) Wenzel, Fred (August 2009). ["why wikipedia might need a fail-pet — and why mozilla does not"](http://fredericiana.com/2009/08/01/why-wikipedia-might-need-a-fail-pet-and-why-mozilla-does-not/). Retrieved 8 February 2012.
7. [↑](./Error_message#cite_ref-7) Rintel, Sean (2 November 2011). ["The Evolution of Fail Pets : Strategic Whimsy and Brand Awareness in Error Messages"](http://uxmag.com/articles/the-evolution-of-fail-pets). UX Magazine. Retrieved 8 February 2012.

 

## External links

   [![Wikimedia Commons logo](//upload.wikimedia.org/wikipedia/en/thumb/4/4a/Commons-logo.svg/40px-Commons-logo.svg.png)](./File:Commons-logo.svg) Wikimedia Commons has media related to [Error messages](https://commons.wikimedia.org/wiki/Category:Error%20messages).  
- [A more useful 404 (A List Apart)](http://www.alistapart.com/articles/amoreuseful404/)
- [Avoid being embarrassed by your error messages (UX Matters)](http://www.uxmatters.com/mt/archives/2010/08/avoid-being-embarrassed-by-your-error-messages.php)
- [Oops! I ruined your life. :) (Cooper Journal)](http://www.cooper.com/journal/2012/01/oops_i_ruined_your_life.html) [Archived](https://web.archive.org/web/20140825150411/http://www.cooper.com/journal/2012/01/oops_i_ruined_your_life.html) 2014-08-25 at the [Wayback Machine](./Wayback_Machine)

 
| vteError messages |
| --- |
| System failure | Bomb iconFatal system errorGuru MeditationKernel panicLinux kernel oopsRed Ring of DeathSad MacScreen of deathBlueBlack |
| Application failure | ABENDFatal exception errorSegmentation fault |
| Device and data errors | HTTP 402HTTP 403HTTP 404HTTP 500lp0 on fireNot a typewriterPC LOAD LETTER |
| Other | Abort, Retry, Fail?Bad command or file nameHalt and Catch FireHTTP 418Out of memoryDoes not compute |
| Lists | List of HTTP status codesList of FTP server return codesList of SMTP server return codeserrno.h |
| Related | Spinning pinwheelWindows wait cursor |