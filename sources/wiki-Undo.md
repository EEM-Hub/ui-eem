---
source: https://en.wikipedia.org/wiki/Undo
fetched: 2026-06-20
---

Computer command "Redo" redirects here; not to be confused with [Do over (disambiguation)](./Do_over_(disambiguation)). For how to "undo" an edit in Wikipedia, see [Wikipedia:Undo](./Wikipedia:Undo). For other uses, see [Undo (disambiguation)](./Undo_(disambiguation)). [![](//upload.wikimedia.org/wikipedia/commons/thumb/a/a2/Undo-redo.jpg/250px-Undo-redo.jpg)](./File:Undo-redo.jpg)Universal symbols for undo and redo 

**Undo** is an [interaction technique](./Interaction_technique) which is implemented in many [computer programs](./Computer_program). It erases the last change done to the [document](./Document), reverting it to an older state. In some more advanced programs, such as [graphic processing](./Graphics_software), undo will negate the last command done to the file being edited. With the possibility of undo,[[1]](./Undo#cite_note-1) users can explore and work without fear of making mistakes, because they can easily be undone.

 

The expectations for undo are easy to understand: to have a predictable functionality, and to include all "undoable" commands.[[2]](./Undo#cite_note-:0-2) Usually undo is available until the user undoes all executed operations. But there are some actions which are not stored in the undo list, and thus they cannot be undone. For example, *save file* is not undoable, but is queued in the list to show that it was executed. Another action which is usually not stored, and thus not undoable, is *scrolling* or *selection*.[[3]](./Undo#cite_note-3)

 

The opposite of to undo is to **redo**. The redo command reverses the undo or advances the buffer to a more recent state.

 

The [common components](./Common_Component_Architecture) of undo functionality are the *commands* which were executed of the user, the *history buffer(s)* which stores the completed actions, the *undo/redo manager* for controlling the history buffer, and the *[user interface](./User_interface)* for interacting with the user.[[4]](./Undo#cite_note-:1-4)

 

In most graphical applications for the majority of the mainstream [operating systems](./Operating_system) (such as [Microsoft Windows](./Microsoft_Windows), [Linux](./Linux) and [BSDs](./List_of_BSD_operating_systems)), the [keyboard shortcut](./Keyboard_shortcut) for the undo is [Ctrl](./Control_key)+Z, and the shortcut for redo is Ctrl+Y or Ctrl+⇧ [Shift](./Shift_key)+Z. In most [macOS](./MacOS) applications, the shortcut for the undo command is ⌘ [Command](./Command_key)+Z, and the shortcut for redo is ⌘ Command+⇧ Shift+Z. On all platforms, the undo/redo functions can also be accessed via the [Edit menu](./Edit_menu).

 

## History

 

The ability to undo an operation on a computer was independently invented multiple times, in response to how people used computers.[[5]](./Undo#cite_note-5)

 

The [File Retrieval and Editing System](./File_Retrieval_and_Editing_System), developed starting in 1968 at [Brown University](./Brown_University), is reported to be the first computer-based system to have had an "undo" feature.[[6]](./Undo#cite_note-6)[[7]](./Undo#cite_note-barnet-7)

 

[Warren Teitelman](./Warren_Teitelman) developed a *Programmer's Assistant* as part of BBN-LISP with an Undo function, by 1971.[[8]](./Undo#cite_note-8)

 

[Marvin Zelkowitz](./Marvin_Zelkowitz) proposed in his PhD thesis (Reversible Execution as a Diagnostic Tool) in 1971 at [Cornell University](./Cornell_University) the concept of reversible execution, which is essentially an undo. In his PhD thesis (An Interactive Analysis System for Execution-Time Errors) at the [University of Illinois at Urbana-Champaign](./University_of_Illinois_at_Urbana-Champaign) in 1975, [Alan M. Davis](./Alan_M._Davis) expanded on Zelkowitz's concept to show how multi-level undo (i.e., multi-level reversible execution) could be used for [debugging](./Debugging) software programs.

 

The [Xerox PARC](./Xerox_PARC) [Bravo](./Bravo_(software)) [text editor](./Text_editor) had an Undo command in 1974.[[9]](./Undo#cite_note-9) 
A 1976 research report by Lance A. Miller and John C. Thomas of [IBM](./IBM), *Behavioral Issues in the Use of Interactive Systems*,[[10]](./Undo#cite_note-10) noted that "it would be quite useful to permit users to 'take back' at least the immediately preceding command (by issuing some special 'undo' command)."[[11]](./Undo#cite_note-11) The programmers at the [Xerox PARC](./PARC_(company)) research center assigned the keyboard shortcut Ctrl-Z to the undo command, which became a crucial feature of text editors and word processors in the [personal computer](./Personal_computer) era.[[12]](./Undo#cite_note-BenZimmer_2009-12)  In 1980, [Larry Tesler](./Larry_Tesler) of Xerox PARC began working at [Apple Computer](./Apple_Computer). There, he and [Bill Atkinson](./Bill_Atkinson) advocated for the presence of an undo command as a standard fixture on the [Apple Lisa](./Apple_Lisa).  Atkinson was able to convince the individual developers of the Lisa's [application software](./Application_software) to include a single level of undo and redo, but was unsuccessful in lobbying for multiple levels.[*[citation needed](./Wikipedia:Citation_needed)*] When Apple introduced the Lisa's successor, the [Macintosh](./Macintosh), it stipulated that all standard applications should include an “Undo” as the first command in the “Edit” menu,[[13]](./Undo#cite_note-13) which has remained the standard on [macOS](./MacOS) and [Windows](./Windows) to this day.

 

Multi-level undo commands were introduced in the 1980s, allowing the users to take back a series of actions, not just the most recent one.[[12]](./Undo#cite_note-BenZimmer_2009-12) [EMACS](./EMACS) and other timeshared screen editors had it before personal [computer software](./Computer_software). [CygnusEd](./CygnusEd) was the first [Amiga](./Amiga) text editor with an unlimited undo/redo feature. [AtariWriter](./AtariWriter), a word-processing application introduced in 1982, featured undo. NewWord, another word-processing program released by NewStar in 1984, had an unerase command.[[12]](./Undo#cite_note-BenZimmer_2009-12) IBM's VisiWord also had an undelete command.

 

## Undo and redo models

 

Undo models can be categorized as linear or non-linear. The non-linear undo model can be sub-classified in script model, US&R model, triadic model, and selective undo.[[2]](./Undo#cite_note-:0-2)

 

Some common properties of models are:

 
- *stable execution property:* A state is represented as an ordered list of commands. This means that a command "is always undone in the state that was reached after the original execution."[[4]](./Undo#cite_note-:1-4)
- *weakened stable execution:* This means that if undo is executed all commands which depend on the undone command are undone dependent on the command.
- *stable result property:* This property has the similar meaning like the *stable execution property* except for the list. The ordered list of commands includes that they were executed instead of only the commands.
- *commutative:* That means that the reached state after undo and redo two different commands is the same when they are executed in the converse order.
- *minimalistic undo property:* It describes that "undo operation of command C undoes only command C and all commands younger than C which are dependent on C."[[4]](./Undo#cite_note-:1-4)

 

### Linear undo

 

Linear undo is implemented with a [stack](./Stack_(data_structure)) (last in first out (LIFO) [data structure](./Data_structure)) that stores a history of all executed commands. When a new command is executed it is added to the top of stack. Therefore, only the last executed command can be undone and removed from the history. Undo can be repeated as long as the history is not empty.[[2]](./Undo#cite_note-:0-2)

 

#### Restricted linear model

 

The restricted linear model is an augmentation of the linear undo model. It satisfies the above described *stable execution property* for linear undo, because this model does not keep the property if a command is done while the history list includes other commands. The restricted linear model clears the history list before a new command is added. But other restrictions are available, too. For example, the size of the history list can be restricted or when a defined size is reached, the first executed command is deleted from the list.[[2]](./Undo#cite_note-:0-2)

 

### Non-linear undo

 

The main difference between linear undo and non-linear undo is the possibility of the user to undo the executed commands in an arbitrary order. They have the chance to undo not the most recently command but rather choose a command from the list.[[4]](./Undo#cite_note-:1-4) For non linear model there are subclasses which implement this model.

 

#### Script model

 

The script model handles user actions as editing a script of commands. The history list of the executed commands are interpreted "as a script, the effect of an undo is defined to be the same as if the undone action had never occurred in the first place."[[2]](./Undo#cite_note-:0-2) As the result of undo the state has to be the way as if the undone command was never executed. A disadvantage of this model is that the user has to know the connection between undone command and the current state to avoid side effects. One of this can be for example duplication. Other problems are that if "subsequent commands are redone in a different state that they were originally executed in direct manipulation interfaces, this reinterpretation of the original user action is not always obvious or well defined".[[2]](./Undo#cite_note-:0-2)

 

#### US&R model

 

The special feature of this model is that it has the option of skipping a command. This means that redoing a command can be skipped. The command which is skipped is marked as skipped but not deleted. When new commands are executed, the history list is retained, so the order of the executed commands can be reproducible with that. The order can be described through a history tree which is a directed graph, "because it is possible to continue redoing commands from another branch creating a link in the graph".[[2]](./Undo#cite_note-:0-2) Even though the set of commands is simple and easy to understand, the complex structure with skipping and linking branches is hard to comprehend and to remember, when the user wants to undo more than one step.[[2]](./Undo#cite_note-:0-2)

 

#### Triadic model

 

This non-linear undo model has besides undo and redo the possibility to rotate. It has the same data structure as the above-mentioned models with a history list and a separated redo list which includes the redo operations. The rotate operation sets the last command of the redo list in front of it. On one hand this means that the next command to be redone can be selected by placing it in front. On the other hand, rotation can be used "to select the place in the redo list where the next undo operation will put the command".[[2]](./Undo#cite_note-:0-2) The list of redo is therefore unordered. "To undo an isolated command, the user has to undo a number of steps, rotate the redo list, and then redo a number of steps".[[2]](./Undo#cite_note-:0-2) For redo the list has to be rotated until the wanted command is above.

 

### Selective undo

 

Jakubec et al. say that selective undo is a feature which a model can offer but for selective undo there is no clear definition.[[4]](./Undo#cite_note-:1-4) The authors selected functions which a model should have when it supports selective undo. It should be possible to "undo any executed action in the history buffer. Actions independent of the action being undone should be left untouched".[[4]](./Undo#cite_note-:1-4) Just like that redo has to be possible to any undone command. The third function for selective undo is that "no command can be automatically discarded from history buffer without direct user’s request."[[4]](./Undo#cite_note-:1-4) For selective undo applies that undo and redo is executable outside of any context. There are three main issues. The first is that undone commands can be outside of the originally context. Through this there can be dead references which have to be handled. The second issue that modified commands can be undone and so it has to be solved which state after undo will be presented. The third issue is discarding command problems. Selective undo has no pointer in the lists, so this means that no command should be discarded of the stack.[[4]](./Undo#cite_note-:1-4)

 

#### Direct selective undo

 

Direct selective undo is an extension of restricted linear undo with a history tree. The operation creates a copy of the selected command, executes this and add it to the history list. There two non-linear operations selective undo and selective redo are defined, so it is more symmetric.[[2]](./Undo#cite_note-:0-2)

 

### Multiuser application

 

When multiple users can edit the same document simultaneously, a multi-user undo is needed. *Global* multi-user undo reverts the latest action made to the document, regardless of who performed the edit. *Local* multi-user undo only reverts actions done by the local user, which requires a non-linear undo implementation.

 

Where undo can be used to backtrack through multiple edits, the redo command goes forward through the action history. Making a new edit usually clears the redo list. If a branching redo model is used, the new edit *branches* the action history.

 

The number of previous actions that can be undone varies by program, version, and hardware or software capabilities. For example, the default undo/redo stack size in [Adobe Photoshop](./Adobe_Photoshop) is 20 but can be changed by the user. As another example, earlier[*[when?](./Wikipedia:Manual_of_Style/Dates_and_numbers#Chronological_items)*] versions of [Microsoft Paint](./Microsoft_Paint) only allowed up to three edits to be undone; the version introduced in [Windows 7](./Windows_7) increased this limit to 50.

 

Simplistic, single-edit undo features sometimes do away with "redo" by treating the undo command itself as an action that can be undone. This is known as the flip undo model, because the user can flip between two program states using the undo command.[[14]](./Undo#cite_note-14) This was the standard model prior to the widespread adoption of multiple-level undo in the early 1990s.

 

## Undo implementation

 

Undo can be implemented through different patterns. The most common patterns are [command pattern](./Command_pattern) and [memento pattern](./Memento_pattern).

 

### Command pattern

 

The [command pattern](./Command_pattern) is a [software design pattern](./Software_design_pattern) which encapsulates information from the operation into command objects. This means that every action is stored in an object. The abstract command class implements an abstract execute operation, so every command object has an execute operation. For undo there also have to be unexecuted operation, which undoes the effect of the executed command, which are stored in a history list. Undo and redo are implemented so that the list is run through forwards and backwards when the execute or unexecute command is called.[[15]](./Undo#cite_note-:2-15)

 

For single undo only the executed command is stored. In contrast to the multi level undo where not only the history list with the commands is saved but also the number of undo levels can be determined of the maximum length of the list.[[15]](./Undo#cite_note-:2-15)

 

### Memento pattern

 

With [memento pattern](./Memento_pattern) the internal state of an object is stored. The object in which the state is saved, is called memento and is organized through the memento originator. This returns a memento, initialized with information of the current state, when undo is executed, so that the state can be checked. The memento is only visible for the originator.

 

In memento pattern the undo mechanism is called caretaker. It is responsible for the safekeeping of the mementos but never change the contents of these. For undo the caretaker requests a memento of the originator and then applying the undo.[[15]](./Undo#cite_note-:2-15)

 

The most part of undo mechanism can implemented without dependency to specific applications or command classes. This includes "the management of history list, the history scroller, menu entries for undo and redo and update of the menu entries depending on the name of the next available command."[[2]](./Undo#cite_note-:0-2)

 

Every command class has a do method which is called when a command is executed. The undo-method implements the reverse operation of the do-method. To implement the reverse, there are several different strategies.

 
- *full checkpoint**:*** That means that the complete state is saved after a command is executed. This is the easiest implementation, but is not highly efficient and therefore not often used.
- *complete rerun:* Therefore, the initial state is saved and every state in the history list can be reached through "starting with the initial state and redoing all commands from the beginning of the history."[[2]](./Undo#cite_note-:0-2)
- *partial checkpoint**:*** This is the most used strategy. The changed application state is saved and with undo the part of the state is set back to the forward value.
- *inverse function:* Inverse function needs no saved state information. "For example, moving can be reversed by moving the object back by relative amount."[[2]](./Undo#cite_note-:0-2) For selective undo there is not enough information for saving the state.

 

## See also

 
- [Reversible computing](./Reversible_computing)
- [Rollback (data management)](./Rollback_(data_management))
- [Undeletion](./Undeletion)
- [Version control](./Version_control) ([native file format](./Native_and_foreign_format))

 

## References

  
1. [↑](./Undo#cite_ref-1) Myrtus (2026-01-31). ["The undo option changed what feels risky"](https://www.crumbs.top/the-undo-option-changed-what-feels-risky/). *crumbs.top*. Retrieved 2026-02-07.
2. [1](./Undo#cite_ref-:0_2-0) [2](./Undo#cite_ref-:0_2-1) [3](./Undo#cite_ref-:0_2-2) [4](./Undo#cite_ref-:0_2-3) [5](./Undo#cite_ref-:0_2-4) [6](./Undo#cite_ref-:0_2-5) [7](./Undo#cite_ref-:0_2-6) [8](./Undo#cite_ref-:0_2-7) [9](./Undo#cite_ref-:0_2-8) [10](./Undo#cite_ref-:0_2-9) [11](./Undo#cite_ref-:0_2-10) [12](./Undo#cite_ref-:0_2-11) [13](./Undo#cite_ref-:0_2-12) [14](./Undo#cite_ref-:0_2-13) Berlage, Thomas (1994-09-01). "A selective undo mechanism for graphical user interfaces based on command objects". *ACM Transactions on Computer-Human Interaction*. **1** (3): 269–294. [doi](./Doi_(identifier)):[10.1145/196699.196721](https://doi.org/10.1145%2F196699.196721). [ISSN](./ISSN_(identifier)) [1073-0516](https://search.worldcat.org/issn/1073-0516). [S2CID](./S2CID_(identifier)) [11848679](https://api.semanticscholar.org/CorpusID:11848679).
3. [↑](./Undo#cite_ref-3) Myers, Brad A.; Kosbie, David S. (1996-04-13). ["Reusable hierarchical command objects"](https://archive.org/details/commongroundchi900chi9/page/260). *Proceedings of the SIGCHI conference on Human factors in computing systems common ground - CHI '96*. ACM. pp. [260–267](https://archive.org/details/commongroundchi900chi9/page/260). [doi](./Doi_(identifier)):[10.1145/238386.238526](https://doi.org/10.1145%2F238386.238526). [ISBN](./ISBN_(identifier)) [0897917774](./Special:BookSources/0897917774). [S2CID](./S2CID_(identifier)) [17033810](https://api.semanticscholar.org/CorpusID:17033810).
4. [1](./Undo#cite_ref-:1_4-0) [2](./Undo#cite_ref-:1_4-1) [3](./Undo#cite_ref-:1_4-2) [4](./Undo#cite_ref-:1_4-3) [5](./Undo#cite_ref-:1_4-4) [6](./Undo#cite_ref-:1_4-5) [7](./Undo#cite_ref-:1_4-6) [8](./Undo#cite_ref-:1_4-7) Jakubec, Karel; Polák, Marek; Nečaský, Martin; Holubová, Irena (2014). ["Undo/Redo Operations in Complex Environments"](https://doi.org/10.1016%2Fj.procs.2014.05.461). *Procedia Computer Science*. **32**: 561–570. [doi](./Doi_(identifier)):[10.1016/j.procs.2014.05.461](https://doi.org/10.1016%2Fj.procs.2014.05.461). [ISSN](./ISSN_(identifier)) [1877-0509](https://search.worldcat.org/issn/1877-0509).
5. [↑](./Undo#cite_ref-5) Moran, Chuktropolis Welling (2013-01-01). [*Interactive Time*](https://web.archive.org/web/20210428122647/http://roger.ucsd.edu/record=b7759913~S9) (Ph.D.). La Jolla: University of California, San Diego. [ISBN](./ISBN_(identifier)) [9781303194450](./Special:BookSources/9781303194450). Archived from [the original](http://roger.ucsd.edu/record=b7759913~S9) on 2021-04-28. Retrieved 2016-07-07.
6. [↑](./Undo#cite_ref-6) Barnet, Belinda (2014-12-01). [*Memory Machines: The Evolution of Hypertext*](https://books.google.com/books?id=N1qWBQAAQBAJ). Anthem Press. p. 108. [ISBN](./ISBN_(identifier)) [9781783083442](./Special:BookSources/9781783083442). But the most popular development for novice users in FRESS was not its capacity to accommodate multiple displays and users; it was the 'undo' feature – the feature of which van Dam is most proud (van Dam 2011). FRESS pioneered a single-level undo for both word processing and hypertext. Every edit to a file was saved in a shadow version of the data structure, which allowed for both an 'autosave' and an undo. Brown staff and students understood immediately the importance and usefulness of this feature (van Dam 1999).
7. [↑](./Undo#cite_ref-barnet_7-0) Barnet, Belinda (2010-01-01). ["Crafting the User-Centered Document Interface: The Hypertext Editing System (HES) and the File Retrieval and Editing System (FRESS)"](http://www.digitalhumanities.org/dhq/vol/4/1/000081/000081.html). *Digital Humanities Quarterly*. **4** (1). [Archived](https://web.archive.org/web/20210501221147/http://www.digitalhumanities.org/dhq/vol/4/1/000081/000081.html) from the original on 2021-05-01. Retrieved 2016-05-27.
8. [↑](./Undo#cite_ref-8) Teitelman, Warren (1972-01-01). "Automated programmering: The programmer's assistant". *Proceedings of the December 5-7, 1972, fall joint computer conference, Part II on - AFIPS '72 (Fall, part II)*. New York, NY, USA: ACM. pp. 917–921. [doi](./Doi_(identifier)):[10.1145/1480083.1480119](https://doi.org/10.1145%2F1480083.1480119). [S2CID](./S2CID_(identifier)) [1276566](https://api.semanticscholar.org/CorpusID:1276566).
9. [↑](./Undo#cite_ref-9) ["Bravo Manual in Alto Non-Programmers Guide, p. 52"](http://history-computer.com/Library/AltoUsersHandbook.pdf) (PDF). [Archived](https://web.archive.org/web/20150505100802/http://history-computer.com/Library/AltoUsersHandbook.pdf) (PDF) from the original on 2015-05-05. Retrieved 2014-03-29.
10. [↑](./Undo#cite_ref-10) Miller, Lance A.; Thomas, John C. (1977-09-01). "Behavioral issues in the use of interactive systems". *International Journal of Man-Machine Studies*. **9** (5): 509–536. [doi](./Doi_(identifier)):[10.1016/S0020-7373(77)80002-3](https://doi.org/10.1016%2FS0020-7373%2877%2980002-3). [ISSN](./ISSN_(identifier)) [0020-7373](https://search.worldcat.org/issn/0020-7373).
11. [↑](./Undo#cite_ref-11) Miller, Lance A.; John C. Thomas Jr. (December 1976). ["Behavioral Issues in the Use of Interactive Systems"](https://web.archive.org/web/20120527163155/http://handle.dtic.mil/100.2/ADA043033). Archived from [the original](http://handle.dtic.mil/100.2/ADA043033) (PDF) on May 27, 2012. Retrieved 2011-05-21.
12. [1](./Undo#cite_ref-BenZimmer_2009_12-0) [2](./Undo#cite_ref-BenZimmer_2009_12-1) [3](./Undo#cite_ref-BenZimmer_2009_12-2) Ben Zimmer (2009-09-15). ["The Age of Undoing"](https://www.nytimes.com/2009/09/20/magazine/20FOB-onlanguage-t.html). *New York Times*. [Archived](https://web.archive.org/web/20130617212919/http://www.nytimes.com/2009/09/20/magazine/20FOB-onlanguage-t.html) from the original on 2013-06-17. Retrieved 2013-06-02.
13. [↑](./Undo#cite_ref-13) Apple Computer, Inc. (1984). "User Interface". *Inside Macintosh, Volume I*.
14. [↑](./Undo#cite_ref-14) Roberta Mancini, Alan Dix and Stefano Levialdi. 2006. ["Reflections on Undo"](http://www.hcibook.com/alan/papers/undo-techrep-96/tech9611.pdf)
15. [1](./Undo#cite_ref-:2_15-0) [2](./Undo#cite_ref-:2_15-1) [3](./Undo#cite_ref-:2_15-2) Erich Gamma; Richard Helm; Ralph Johnson; John Vlissides (1995). *[Design Patterns](./Design_Patterns)*. Reading, Mass.: Addison-Wesley. [ISBN](./ISBN_(identifier)) [0201633612](./Special:BookSources/0201633612). [OCLC](./OCLC_(identifier)) [31171684](https://search.worldcat.org/oclc/31171684).

 

## Further reading

 
- [Zimmer, Ben](./Ben_Zimmer) (15 Sep 2009). ["The Age of Undoing"](https://www.nytimes.com/2009/09/20/magazine/20FOB-onlanguage-t.html). *[The New York Times](./The_New_York_Times)*. [Archived](https://web.archive.org/web/20111130155601/https://www.nytimes.com/2009/09/20/magazine/20FOB-onlanguage-t.html) from the original on 2011-11-30.

 

## External links

 
- [![Wiktionary logo](//upload.wikimedia.org/wikipedia/commons/thumb/9/99/Wiktionary-logo-en-v2.svg/20px-Wiktionary-logo-en-v2.svg.png)](./File:Wiktionary-logo-en-v2.svg) The dictionary definition of [*undo*](https://en.wiktionary.org/wiki/Special:Search/undo) at Wiktionary