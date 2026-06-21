---
source: https://en.wikipedia.org/wiki/Modal_window
fetched: 2026-06-20
---

Subordinate user interface element Not to be confused with [dialog box](./Dialog_box). 

In [user interface](./User_interface) design, a **modal window**, or **modal** for short,[[1]](./Modal_window#cite_note-1)[[2]](./Modal_window#cite_note-2) is a [graphical control element](./Graphical_control_element_(software)) subordinate to an application's [main window](./Main_window).

 

A modal window creates a [mode](./Mode_(user_interface)) that disables user interaction with the main window but keeps it visible, with the modal window as a [child window](./Window_(computing)#Properties) in front of it. Users *must* interact with the modal window before they can return to the [parent](./Tree_(data_structure)#Terminology) window. This avoids interrupting the [workflow](./Workflow) on the main window. Modal windows are sometimes called **heavy windows** or **modal dialogs** because they often display a [dialog box](./Dialog_box).

 

User interfaces typically use modal windows to command user awareness and to display emergency states, though [interaction designers](./Interaction_designer) argue they are ineffective for that use.[[3]](./Modal_window#cite_note-undo-3) Modal windows are prone to [mode errors](./Mode_error).[[3]](./Modal_window#cite_note-undo-3)[[4]](./Modal_window#cite_note-4)[[5]](./Modal_window#cite_note-5)

 

On the [Web](./World_Wide_Web), they often show images in detail, such as those implemented by the [Lightbox](./Lightbox_(JavaScript)) library, or are used for [hover ads](./Hover_ad).[[6]](./Modal_window#cite_note-6)[[7]](./Modal_window#cite_note-useit-7)

 

The opposite of modal is **[modeless](./Modeless)**. Modeless windows don't block the main window, so the user can switch their [focus](./User_focus) between them, treating them as [palette windows](./Palette_window).

 

## Relevance and use

 

### Use cases

 

Frequent uses of modal windows include:

 
- Drawing attention to vital pieces of information. This use has been criticized as ineffective because users are bombarded with too many dialog boxes, and habituate to simply clicking "Close", "Cancel", or "OK" without reading or understanding the message.[[8]](./Modal_window#cite_note-8)[[9]](./Modal_window#cite_note-9)[[10]](./Modal_window#cite_note-10)
- Blocking the application flow until information required to continue is entered, as for example a [password](./Password) in a [login](./Logging_(computer_security)) process. Another example are [file dialogs](./File_dialog) to open and save files in an application.
- Collecting application configuration options in a centralized dialog. In such cases, typically the changes are applied upon closing the dialog, and access to the application is disabled while the edits are being made.
- Warning that the effects of the current action are not reversible. This is a frequent [interaction pattern](./Interaction_design_pattern) for modal dialogs, but some usability experts criticize it as ineffective for its intended use (protection against errors in destructive actions) due to [habituation](./Habituation). They recommend making the action reversible (providing an "undo" option) instead.[[3]](./Modal_window#cite_note-undo-3)

 

### Modal sheets in Mac OS X

 "Sheet (computing)" redirects here; not to be confused with [spreadsheet](./Spreadsheet). 

Many features that would typically be represented by modal windows are implemented as modal [transient](./Transient_screen) panels called "Sheets"[[11]](./Modal_window#cite_note-11) on Mac OS X. Transient windows behave similarly to modal windows – they are always on top of the parent window and are not shown in the window list, but they do not disable the use of other windows in the application. Sheets slide out of the window's title bar, and usually must be dismissed before the user can continue to work in the window, but the rest of the application stays usable. Thus they create a mode inside the window that contains them, but are modeless with respect to the rest of the application.

 

## Control of interaction flow

 

Modal windows are common in GUI toolkits for guiding user workflow. [Alan Cooper](./Alan_Cooper_(software_designer)) contends that the importance of requiring the user to attend to important issues justifies restricting the user's freedom and that the alternative would increase user frustration.[[12]](./Modal_window#cite_note-12)

 

### Unexpected interruptions

 

Unexpected [alert dialogs](./Alert_dialog_box) are particular culprits of [mode errors](./Mode_error)[[3]](./Modal_window#cite_note-undo-3) with potentially severe consequences. Usability practitioners prescribe that dangerous actions should be undoable wherever possible; an alert box that appears unexpectedly or is dismissed by [habituation](./Habituation) doesn't protect from the dangerous action.[[13]](./Modal_window#cite_note-13) A modeless [infobar](./Infobar) is increasingly seen as preferable to a dialog box because it does not interrupt the user's activities, but rather allows the user to read extra information in their own time.

 

One proposed approach is to design every input element as a self-contained, [task-oriented](./Task_analysis) interaction, guided by its own specific requirements rather than by the global state of the entire application. For example, required elements might be preceded with an [asterisk](./Asterisk), elements with invalid data might acquire a red border, and so on. With this approach, users actually benefit from seeing many input elements at once — they can enter data in a way that makes sense to them, instead of having all the other unrelated elements blocked until a predefined data-entry sequence is completed.

 

### Problems

 See also: [Assessment of modes in computer interfaces](./Mode_(computer_interface)#Assessment) 

A modal window blocks all other [workflows](./Workflows) in the top-level program until the modal window is closed, as opposed to [modeless](./Modeless) dialogs that allow users to operate with other windows.[[14]](./Modal_window#cite_note-java-14) Modal windows are intended to grab the user's full attention.[[15]](./Modal_window#cite_note-15) Users may not recognize that a modal window requires their attention, leading to confusion about the main window being non-responsive, or causing loss of the user's data input intended for the main window (see [mode error](./Mode_error)). In severe cases, the modal window appears behind another window controlled by the same program, potentially rendering the entire program unresponsive until the modal window can be located manually.

 

However, many interface designers have recently taken steps to make modal windows more obvious by darkening the background behind the window or allowing any mouse click outside of the modal window to force the modal window to close – a design called a [lightbox](./Lightbox_(JavaScript))[[7]](./Modal_window#cite_note-useit-7) – thus alleviating those problems. Jakob Nielsen states as an advantage of modal dialogs that it improves user awareness: "When something does need fixing, it's better to make sure that the user knows about it." For this goal, the lightbox design provides strong visual contrast of the dialog over the rest of the visuals. The lightbox technique is now a common tool in website design.

 

Modal windows are commonly implemented in ways that block the possibility to move, minimize, iconify, or push that window back, and they grab input focus, which often prevents use of a system's [cut, copy, and paste](./Cut,_copy,_and_paste) facilities. This can interfere with the use of their parent applications by blocking access to other windows and data within the same application, particularly in cases where the modal window is requiring the user to input information only available in one of the windows it's covering.

 

For users using virtual work areas larger than their actual screens, modal windows can cause further undesirable behavior, including creating the modal on a portion of the virtual screen not currently on the display, or abruptly switching the display from what the user was working on to an entirely different section.

 

Modal windows tend to create an abrupt diversion of text input, especially typed input intended for other programs, into themselves. Further, modals usually interpret actuation of the [enter key](./Enter_key) (or in rare cases the presence of a [newline](./Newline) in pasted input) as a cue to accept the input and process it—or, in rare cases, may intercept a mouse click intended for a different application that has suddenly been covered. Such interception, called [focus stealing](./Focus_stealing) (or stealing focus) can compromise privacy and security practices, as well as capture inappropriate, out-of-context input that can cause undefined, arbitrary results in the program that generated the modal window.

 

Depending on the specifics of implementation, modal windows can violate the [principle of least surprise](./Principle_of_least_surprise).

 

### Recommendations

 See also: [Mode (user interface) § Design recommendations](./Mode_(user_interface)#Design_recommendations) 

Modal dialogs are part of a task flow, and recommendations are given to place them where the focus is in that flow. For example, the window could be placed near the [graphical control element](./Graphical_control_element_(software)) that triggers its activation.[[16]](./Modal_window#cite_note-Implementation-16)

 

Using a semi-transparent dark background can obscure information in the main window, so it is best used only when that information would be distracting. A semi-transparent background can be made less intrusive by having the whole background area function as a close button: this is standard on most mobile operating systems, avoids making the user feel trapped, and makes modal windows feel less like malicious pop-ups.

 

Design should follow common practices in the platform the program is running on. [Microsoft Windows](./Microsoft_Windows) uses standard controls for modal [window dialogs](./Window_dialog), with affirmative action buttons at the lower right of the panel. [Mac OS X](./Mac_OS_X) uses [modal sheets](./Modal_sheet) with affirmative action buttons being the right-most command.[[17]](./Modal_window#cite_note-17)

 

## See also

 
- [Application posture](./Application_posture)
- [Popover (GUI)](./Popover_(GUI))

 

## References

 
1. [↑](./Modal_window#cite_ref-1) Segun, Daniel (2022-09-07). ["Are Modals In Web Design A UX Disaster?"](https://webdesignerdepot.com/are-modals-in-web-design-a-ux-disaster/). Retrieved 2025-09-26.
2. [↑](./Modal_window#cite_ref-2) Coyier, Chris (2016-07-18). ["Considerations for Styling a Modal"](https://css-tricks.com/considerations-styling-modal/). *CSS-Tricks*. Retrieved 2025-09-26.
3. [1](./Modal_window#cite_ref-undo_3-0) [2](./Modal_window#cite_ref-undo_3-1) [3](./Modal_window#cite_ref-undo_3-2) [4](./Modal_window#cite_ref-undo_3-3) ["Never Use a Warning When you Mean Undo"](https://alistapart.com/article/neveruseawarning). *alistapart.com*. Retrieved 2015-10-09.
4. [↑](./Modal_window#cite_ref-4) Raskin, Jef (2000). [*The Humane Interface*](https://archive.org/details/humaneinterfacen00rask). United States: Addison Wesley. [ISBN](./ISBN_(identifier)) [0-201-37937-6](./Special:BookSources/0-201-37937-6).
5. [↑](./Modal_window#cite_ref-5) ["Nitpicker / The Humane Interface"](http://nitpicker.pbworks.com/w/page/12451253/The%2520Humane%2520Interface). *nitpicker.pbworks.com*. Rule 1a. Retrieved 2015-10-09.
6. [↑](./Modal_window#cite_ref-6) Quince UX patterns explorer. ["Modal Panel"](https://web.archive.org/web/20100227095647/http://quince.infragistics.com/Patterns/Modal%20Panel.html). Archived from [the original](http://quince.infragistics.com/Patterns/Modal%20Panel.html) on 2010-02-27. The popular Lightbox JavaScript library uses a modal panel approach for showing the images
7. [1](./Modal_window#cite_ref-useit_7-0) [2](./Modal_window#cite_ref-useit_7-1) Jakob Nielsen, Alertbox. ["10 Best Application UIs"](https://www.useit.com/alertbox/application-design.html).
8. [↑](./Modal_window#cite_ref-8) [Joel Spolsky](./Joel_Spolsky), User Interface Design for Programmers: [Designing for People Who Have Better Things To Do With Their Lives](https://www.joelonsoftware.com/uibook/chapters/fog0000000062.html)
9. [↑](./Modal_window#cite_ref-9) [Raymond Chen](./Raymond_Chen), The Old New Thing: [The default answer to every dialog box is "Cancel"](https://devblogs.microsoft.com/oldnewthing/20030901-00/?p=42723)
10. [↑](./Modal_window#cite_ref-10) Jeff Atwood, Coding Horror: [Teaching Users to Read](http://www.codinghorror.com/blog/archives/000114.html)
11. [↑](./Modal_window#cite_ref-11) ["Sheets - Presentation - Components - Human Interface Guidelines - Design - Apple Developer"](https://developer.apple.com/design/human-interface-guidelines/components/presentation/sheets/). *Apple Developer*. Retrieved 7 September 2022.
12. [↑](./Modal_window#cite_ref-12) Cooper, Alan (March 17, 2003). [*About Face 2.0: The Essentials of Interaction Design*](https://archive.org/details/aboutface20essen0000coop). Wiley. [ISBN](./ISBN_(identifier)) [0-7645-2641-3](./Special:BookSources/0-7645-2641-3).
13. [↑](./Modal_window#cite_ref-13) Raskin, Jef (2000). [*The Humane Interface*](https://archive.org/details/humaneinterfacen00rask). Addison Wesley. [ISBN](./ISBN_(identifier)) [0-201-37937-6](./Special:BookSources/0-201-37937-6).
14. [↑](./Modal_window#cite_ref-java_14-0) ["How to Use Modality in Dialogs"](https://download.oracle.com/javase/tutorial/uiswing/misc/modality.html). [Oracle Corporation](./Oracle_Corporation).
15. [↑](./Modal_window#cite_ref-15) ["Modal Panel"](https://web.archive.org/web/20130506101851/http://quince.infragistics.com/Patterns/Modal%20Panel.aspx#Problem). *quince.infragistics.com*. Archived from [the original](http://quince.infragistics.com/Patterns/Modal%20Panel.aspx#Problem) on 2013-05-06.
16. [↑](./Modal_window#cite_ref-Implementation_16-0) ["Modal Panel - Implementation"](https://web.archive.org/web/20130506101851/http://quince.infragistics.com/Patterns/Modal%20Panel.aspx#Implementation). *quince.infragistics.com*. Archived from [the original](http://quince.infragistics.com/Patterns/Modal%20Panel.aspx#Implementation) on 2013-05-06.
17. [↑](./Modal_window#cite_ref-17) Apple Inc. ["Themes - macOS - macOS - Human Interface Guidelines - Apple Developer"](https://developer.apple.com/library/mac/documentation/UserExperience/Conceptual/OSXHIGuidelines/WindowDialogs.html#//apple_ref/doc/uid/20000957-CH43-SW1). *developer.apple.com*. Retrieved 18 September 2018.

 
| vteGraphical control elements |
| --- |
| Commandinput | Adjustment handleButtonContext menuDrop-down listHamburger buttonMenuPie menu |
| Datainput-output | CheckboxColor pickerCombo boxCycle buttonDate pickerGrid viewToggle switchList boxList builderRadio buttonScrollbarSearch boxSliderSpinnerText box |
| Informational | Balloon helpHead-up display in computingHUD in video gamesIconInfobarLabelLoading screenProgress indicatorProgress barSplash screenThrobberSidebarStatus barToastTooltip |
| Containers | AccordionTree viewClient-side decorationDisclosure widgetFrame / FieldsetMenu barPanelPopoverRibbonTabToolbarWindowWindow decorationWorkspace |
| Navigational | Address barBookmarks barBreadcrumb navigationHyperlinkNavigation barVirtual desktop |
| Specialwindows | Alert dialog boxDialog boxFile dialogInspector windowModal windowPalette window |
| Relatedconcepts | File viewerList of graphical user interface elementsLayout managerLook and feelMouseoverScrollingWidget toolkitWIMPZoomable user interface |