---
source: https://en.wikipedia.org/wiki/Widget_(GUI)
fetched: 2026-06-20
---

Element of interaction in a graphical user interface This article is about reusable components for building user interfaces. For small desktop/web applications, see [Software widget](./Software_widget). For other uses, see [Widget](./Widget_(disambiguation)). 
|  | This articleneeds additional citations forverification.Please helpimprove this articlebyadding citations to reliable sources. Unsourced material may be challenged and removed.Find sources:"Graphical widget"–news·newspapers·books·scholar·JSTOR(March 2015)(Learn how and when to remove this message) |
| --- | --- |

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/0/0d/Gtk3-demo_3.11.8.png/250px-Gtk3-demo_3.11.8.png)](./File:Gtk3-demo_3.11.8.png)gtk3-demo, a program to demonstrate the **widgets** in [GTK+](./GTK+) version 3 

In a [graphical user interface](./Graphical_user_interface) (GUI), a **graphical widget** (also **graphical control element** or **control**) is an [element of interaction](./Human–machine_interface), such as a [button](./Button_(computing)) or a [scroll bar](./Scrollbar). Controls are [software components](./Software_component) that a computer user interacts with through [direct manipulation](./Direct_manipulation) to read or edit information about an application. User interface libraries such as [Windows Presentation Foundation](./Windows_Presentation_Foundation), [Qt](./Qt_(software)), [GTK](./GTK), and [Cocoa](./Cocoa_(API)), contain a collection of controls and the logic to render these.[[1]](./Graphical_widget#cite_note-Microsoft-1)

 

Each widget facilitates a specific type of user-computer interaction, and appears as a visible part of the application's GUI as defined by the theme and rendered by the rendering engine. The theme makes all widgets adhere to a unified aesthetic design and creates a sense of overall cohesion. Some widgets support interaction with the user, for example labels, [buttons](./Button_(computing)), and [check boxes](./Checkbox). Others act as [containers](./Container_(abstract_data_type)#Graphic_containers) that group the widgets added to them, for example [windows](./Window_(computing)), [panels](./Panel_(computer_software)), and tabs.

 

Structuring a user interface with [widget toolkits](./Widget_toolkit) allows developers to reuse code for similar tasks, and provides users with a common language for interaction, maintaining consistency throughout the whole information system.

 

[Graphical user interface builders](./Graphical_user_interface_builder) facilitate the authoring of GUIs in a [WYSIWYG](./What_You_See_Is_What_You_Get) manner employing a [user interface markup language](./User_interface_markup_language).  They automatically generate all the [source code](./Source_code) for a widget from general descriptions provided by the developer, usually through [direct manipulation](./Direct_manipulation).

 

## History

 Further information: [History of the graphical user interface](./History_of_the_graphical_user_interface) 

Around 1920, *widget* entered American English, as a generic term for any useful device, particularly a product manufactured for sale; a [gadget](./Gadget).

 

In 1988, the term *widget* is attested in the context of [Project Athena](./Project_Athena) and the [X Window System](./X_Window_System). In *An Overview of the [X Toolkit](./X_Toolkit_Intrinsics)* by [Joel McCormack](./Joel_McCormack) and Paul Asente, it says:[[2]](./Graphical_widget#cite_note-2)

  

The toolkit provides a library of user-interface components ("widgets") like text labels, scroll bars, command buttons, and menus; enables programmers to write new widgets; and provides the glue to assemble widgets into a complete user interface.

  

The same year, in the manual *X Toolkit Widgets - C Language X Interface* by Ralph R. Swick and Terry Weissman, it says:[[3]](./Graphical_widget#cite_note-3)

  

In the X Toolkit, a widget is the combination of an X window or sub window and its associated input and output semantics.

  

Finally, still in the same year, Ralph R. Swick and Mark S. Ackerman explain where the term *widget* came from:[[4]](./Graphical_widget#cite_note-4)

  

We chose this term since all other common terms were overloaded with inappropriate connotations. We offer the observation to the skeptical, however, that the principal realization of a widget is its associated X window and the common initial letter is not un-useful.

  

## Usage

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/e/e3/GUI_Frame.svg/250px-GUI_Frame.svg.png)](./File:GUI_Frame.svg)Example of enabled and disabled widgets; the [frame](./Frame_(GUI)) at the bottom is disabled, they are grayed out. 

Any widget displays an information arrangement changeable by the user, such as a [window](./Window_(computing)) or a [text box](./Text_box). The defining characteristic of a widget is to provide a single interaction point for the [direct manipulation](./Direct_manipulation) of a given kind of data. In other words, widgets are basic visual building blocks which, combined in an application, hold all the data processed by the application and the available interactions on this data.

 

GUI widgets are graphical elements used to build the human-machine-interface of a program. GUI widgets are implemented like [software components](./Software_component). Widget toolkits and software frameworks, like e.g. [GTK+](./GTK+) or [Qt](./Qt_(software)), contain them in [software libraries](./Software_library) so that programmers can use them to build GUIs for their programs.

 

A family of common reusable widgets has evolved for holding general information based on the [Palo Alto Research Center Inc.](./PARC_(company)) research for the [Xerox Alto](./Xerox_Alto) User Interface.  Various implementations of these generic widgets are often packaged together in [widget toolkits](./Widget_toolkit), which programmers use to build graphical user interfaces (GUIs). Most operating systems include a set of ready-to-tailor widgets that a programmer can incorporate in an application, specifying how it is to behave.[[5]](./Graphical_widget#cite_note-5) Each type of widget generally is defined as a class by object-oriented programming ([OOP](./Object-oriented_programming)). Therefore, many widgets are derived from class inheritance.

 

In the context of an application, a widget may be *enabled* or *disabled* at a given point in time.  An enabled widget has the capacity to respond to events, such as keystrokes or mouse actions.  A widget that cannot respond to such events is considered disabled.  The appearance of a widget typically differs depending on whether it is enabled or disabled; when disabled, a widget may be drawn in a lighter color ("**grayed out**") or be obscured visually in some way.  See the adjacent image for an example.

 

The benefit of disabling unavailable controls rather than hiding them entirely is that users are shown that the control exists but is currently unavailable (with the implication that changing some other control may make it available), instead of possibly leaving the user uncertain about where to find the control at all. On pop-up dialogues, buttons might appear greyed out shortly after appearance to prevent accidental clicking or inadvertent double-tapping.

 

Widgets are sometimes qualified as *[virtual](./Virtuality)* to distinguish them from their physical counterparts, e.g. [*virtual* buttons](./Button_(computing)) that can be clicked with a [pointer](./Pointer_(computing_WIMP)), vs. physical [buttons](./Button_(control)) that can be pressed with a finger (such as those on a [computer mouse](./Computer_mouse)).

 

A related (but different) concept is the [desktop widget](./Desktop_widget), a small specialized GUI application that provides some visual information and/or easy access to frequently used functions such as clocks, calendars, news aggregators, calculators and desktop notes. These kinds of widgets are hosted by a [widget engine](./Widget_engine).

 

## List of common generic widgets

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/d/d5/Widgets.png/330px-Widgets.png)](./File:Widgets.png)Various widgets shown in [Ubuntu](./Ubuntu) [![](//upload.wikimedia.org/wikipedia/commons/thumb/d/db/Qtskins.png/250px-Qtskins.png)](./File:Qtskins.png)[Qt](./Qt_(software)) 'widgets rendered according to three different [skins](./Skin_(computing)) (artistic design): Plastik, Keramik, and Windows See also: [Graphical user interface elements](./Graphical_user_interface_elements) 

### Selection and display of collections

 
- [Button](./Button_(computing)) – control which can be clicked upon to perform an action. An equivalent to a [push-button](./Push-button) as found on mechanical or electronic instruments.

- [Radio button](./Radio_button) – control which can be clicked upon to select one option from a selection of options, similar to selecting a radio station from a group of buttons dedicated to radio tuning. Radio buttons always appear in pairs or larger groups, and only one option in the group can be selected at a time; selecting a new item from the group's buttons also de-selects the previously selected button.
- [Check box](./Check_box) – control which can be clicked upon to enable or disable an option. Also called a tick box. The box indicates an "on" or "off" state via a [check mark](./Check_mark)/tick ☑ or a cross ☒. Can be shown in an intermediate state (shaded or with a dash) to indicate that various objects in a [multiple selection](./Multiple_selection) have different values for the property represented by the check box. Multiple check boxes in a group may be selected, in contrast with radio buttons.
- [Toggle switch](./Toggle_switch_(widget)) - Functionally similar to a check box. Can be toggled on and off, but unlike check boxes, this typically has an immediate effect.
- Toggle Button - Functionally similar to a check box, works as a [switch](./Switch), though appears as a button. Can be toggled on and off.
- Split button – control combining a button (typically invoking some default action) and a drop-down list with related, secondary actions
- [Cycle button](./Cycle_button) - a button that cycles its content through two or more values, thus enabling selection of one from a group of items.

- [Slider](./Slider_(computing)) – control with a handle that can be moved up and down (vertical slider) or right and left (horizontal slider) on a bar to select a value (or a range if two handles are present). The bar allows users to make adjustments to a value or process throughout a range of allowed values.
- [List box](./List_box) – a graphical control element that allows the user to select one or more items from a list contained within a static, multiple line text box.
- [Spinner](./Spinner_(computing)) – value input control which has small up and down buttons to step through a range of values
- [Drop-down list](./Drop-down_list) – A list of items from which to select. The list normally only displays items when a special button or indicator is clicked.
- [Menu](./Menu_(computing)) – control with multiple actions which can be clicked upon to choose a selection to activate

- [Context menu](./Context_menu) – a type of menu whose contents depend on the *context* or state in effect when the menu is invoked
- [Pie menu](./Pie_menu) – a circular context menu where selection depends on direction

- [Menu bar](./Menu_bar) – a graphical control element which contains drop down menus
- [Toolbar](./Toolbar) – a graphical control element on which on-screen buttons, icons, menus, or other input or output elements are placed

- [Ribbon](./Ribbon_(computing)) – a hybrid of menu and toolbar, displaying a large collection of commands in a visual layout through a tabbed interface.

- [Combo box](./Combo_box) ([text box](./Text_box) with attached [menu](./Menu_(computing)) or [List box](./List_box)) – A combination of a single-line [text box](./Text_box) and a [drop-down list](./Drop-down_list) or [list box](./List_box), allowing the user to either type a value directly into the control or choose from the list of existing options.
- [Icon](./Computer_icon) – a quickly comprehensible symbol of a software tool, function, or a data file.
- [Tree view](./Tree_view) – a graphical control element that presents a hierarchical view of information
- [Grid view](./Grid_view) or [datagrid](./Datagrid) – a [spreadsheet](./Spreadsheet)-like [tabular](./Table_(information)) view of data that allows numbers or text to be entered in rows and columns.

 

### Navigation

 
- [Link](./Hyperlink) – Text with some kind of indicator (usually underlining and/or color) that indicates that clicking it will take one to another screen or page.
- [Tab](./Tab_(GUI)) – a graphical control element that allows multiple documents or panels to be contained within a single window
- [Scrollbar](./Scrollbar) – a graphical control element by which continuous text, pictures, or any other content can be scrolled in a predetermined direction (up, down, left, or right)

 

### Text/value input

 
- [Text box](./Text_box) – (edit field) - a graphical control element intended to enable the user to input text

 

### Output

 
- [Label](./Label_(control)) – text used to describe another widget
- [Tooltip](./Tooltip) – informational window which appears when the mouse hovers over another control
- [Balloon help](./Balloon_help)
- [Status bar](./Status_bar) – a graphical control element which poses an information area typically found at the window's bottom
- [Progress bar](./Progress_bar) – a graphical control element used to visualize the progression of an extended computer operation, such as a download, file transfer, or installation
- [Infobar](./Infobar) – a graphical control element used by many programs to display non-critical information to a user

 

### Container

 
- [Window](./Window_(computing)) – a graphical control element consisting of a visual area containing some of the graphical user interface elements of the program it belongs to
- [Collapsible panel](./Collapsible_panel?action=edit&redlink=1) – a panel that can compactly store content which is hidden or revealed by clicking the tab of the widget.

- Drawer: Side sheets or surfaces containing supplementary content that may be anchored to, pulled out from, or pushed away beyond the left or right edge of the screen.[[6]](./Graphical_widget#cite_note-6)

- [Accordion](./Accordion_(GUI)) – a vertically stacked list of items, such as labels or thumbnails where each item can be "expanded" to reveal the associated content
- [Modal window](./Modal_window) – a graphical control element subordinate to an application's main window which creates a mode where the main window can not be used.
- [Dialog box](./Dialog_box) – a small window that communicates information to the user and prompts for a response
- [Palette window](./Palette_window) – also known as "Utility window" - a graphical control element which floats on top of all regular windows and offers ready access tools, commands or information for the current application

- [Inspector window](./Inspector_window) – a type of dialog window that shows a list of the current attributes of a selected object and allows these parameters to be changed on the fly

- [Frame](./Frame_(GUI)) – a type of box within which a collection of graphical control elements can be grouped as a way to show relationships visually
- [Canvas](./Canvas_(GUI)) – generic drawing element for representing graphical information
- [Cover Flow](./Cover_Flow) – an animated, three-dimensional element to visually flipping through snapshots of documents, website bookmarks, album artwork, or photographs.
- [Bubble Flow](./Bubble_Flow?action=edit&redlink=1) – an animated, two-dimensional element that allows users to browse and interact the entire tree view of a discussion thread.
- [Carousel (computing)](./Carousel_(computing)?action=edit&redlink=1) – a graphical widget used to display visual cards in a way that's quick for users to browse, both on websites and on mobile apps

 

## See also

 
- [Graphical user interface elements](./Graphical_user_interface_elements)
- [Geometric primitive](./Geometric_primitive)
- [Widget engine](./Widget_engine) for mostly unrelated, physically inspired "widgets"
- [Widget toolkit](./Widget_toolkit) – a software library which contains a collection of widgets
- [Interaction technique](./Interaction_technique)

 

## References

  
1. [↑](./Graphical_widget#cite_ref-Microsoft_1-0) ["Microsoft: Graphic elements"](https://msdn.microsoft.com/en-us/library/windows/desktop/dn742484%28v=vs.85%29.aspx). *msdn.microsoft.com*. Microsoft. Retrieved 27 April 2015.
2. [↑](./Graphical_widget#cite_ref-2) McCormack, Joel; Asente, Paul (1988). ["An overview of the X toolkit"](https://dl.acm.org/doi/pdf/10.1145/62402.62407). *Proceedings of the 1st annual ACM SIGGRAPH symposium on User Interface Software*. pp. 46–55. [doi](./Doi_(identifier)):[10.1145/62402.62407](https://doi.org/10.1145%2F62402.62407). [ISBN](./ISBN_(identifier)) [0897912837](./Special:BookSources/0897912837). [S2CID](./S2CID_(identifier)) [12924752](https://api.semanticscholar.org/CorpusID:12924752).
3. [↑](./Graphical_widget#cite_ref-3) Swick, Ralph R.; Weissman, Terry (1988). [*X Toolkit Widgets - C Language X Interface*](https://archive.org/details/x-window-system/page/n45). p. [1](https://archive.org/details/x-window-system/page/n49).
4. [↑](./Graphical_widget#cite_ref-4) Ralph R. Swick, Mark S. Ackerman (1988). ["The X Toolkit: More Bricks for Building User-Interfaces –or– Widgets for Hire"](https://www-ftp.lip6.fr/ftp/pub/distributed_systems/athena/xtk.PS). *USENIX Winter*. pp. 221–228. Retrieved 2022-11-20.
5. [↑](./Graphical_widget#cite_ref-5) ["What is widget? - Definition from WhatIs.com"](https://whatis.techtarget.com/definition/widget). *WhatIs.com*. Retrieved 2020-06-03.
6. [↑](./Graphical_widget#cite_ref-6) [https://material-ui.com/demos/drawers/](https://material-ui.com/demos/drawers/) Drawer React component - Material-UI

 

## External links

 
- [Packaged Web Apps (Widgets) - Packaging and XML Configuration (Second Edition) - W3C Recommendation 27 November 2012](https://www.w3.org/TR/widgets)
- [Widgets 1.0: The Widget Landscape (Q1 2008). W3C Working Draft 14 April 2008](https://www.w3.org/TR/2008/WD-widgets-land-20080414/)
- [Requirement For Standardizing Widgets. W3C Working Group Note 27 September 2011](https://www.w3.org/TR/2011/NOTE-widgets-reqs-20110927/)

 
| vteGraphical control elements |
| --- |
| Commandinput | Adjustment handleButtonContext menuDrop-down listHamburger buttonMenuPie menu |
| Datainput-output | CheckboxColor pickerCombo boxCycle buttonDate pickerGrid viewToggle switchList boxList builderRadio buttonScrollbarSearch boxSliderSpinnerText box |
| Informational | Balloon helpHead-up display in computingHUD in video gamesIconInfobarLabelLoading screenProgress indicatorProgress barSplash screenThrobberSidebarStatus barToastTooltip |
| Containers | AccordionTree viewClient-side decorationDisclosure widgetFrame / FieldsetMenu barPanelPopoverRibbonTabToolbarWindowWindow decorationWorkspace |
| Navigational | Address barBookmarks barBreadcrumb navigationHyperlinkNavigation barVirtual desktop |
| Specialwindows | Alert dialog boxDialog boxFile dialogInspector windowModal windowPalette window |
| Relatedconcepts | File viewerList of graphical user interface elementsLayout managerLook and feelMouseoverScrollingWidget toolkitWIMPZoomable user interface |