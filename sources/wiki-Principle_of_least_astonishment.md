---
source: https://en.wikipedia.org/wiki/Principle_of_least_astonishment
fetched: 2026-06-20
---

Principle in computer system design "Least surprise" redirects here. For the principle of least surprise in the Bayesian brain hypothesis, see [Free energy principle](./Free_energy_principle) and [Bayesian approaches to brain function](./Bayesian_approaches_to_brain_function). "Least astonishment" redirects here. For the principle as it applies to Wikipedia, see [WP:POLA](./Wikipedia:POLA). 

In [user interface design](./User_interface_design) and [software design](./Software_design),[[1]](./Principle_of_least_astonishment#cite_note-1) 
the **principle of least astonishment** (**POLA**), also known as **principle of least surprise** (**POLS**),[[a]](./Principle_of_least_astonishment#cite_note-4) proposes that a component of a system should behave in a way that most users will expect it to behave, and therefore not astonish or surprise users. The following is a corollary of the principle: "If a necessary feature has a high astonishment factor, it may be necessary to redesign the feature."[[4]](./Principle_of_least_astonishment#cite_note-rexx-5)

 

The principle has been in use in relation to computer interaction since at least the 1970s. Although first formalized in the field of computer technology, the principle can be applied broadly in other fields. For example, in [writing](./Writing), a [cross-reference](./Cross-reference) to another part of the work or a [hyperlink](./Hyperlink) should be phrased in a way that accurately tells the reader what to expect.

 

## Origin

 

An early reference to the "Law of Least Astonishment" appeared in the [PL/I](./PL/I) Bulletin in 1967 (PL/I is a programming language released by [IBM](./IBM) in 1966).[[5]](./Principle_of_least_astonishment#cite_note-6)  By the late 1960s, PL/I had become infamous for violating the law,[[6]](./Principle_of_least_astonishment#cite_note-7) for example because, due to PL/I's precision conversion rules,[[7]](./Principle_of_least_astonishment#cite_note-8) the expressions `25 + 1/3` and `1/3 + 25` would either produce a fatal error, or, if errors were suppressed, 5.33333333333 instead of the correct 25.33333333333. inaccessible <ref&#x3E;{{cite book |last1=Barron |first1=David William |title=Comparative programming languages |date=1968 |publisher=American Elsevier, NY}}{{page needed|date=March 2024}} </ref&#x3E;[[8]](./Principle_of_least_astonishment#cite_note-9)[[9]](./Principle_of_least_astonishment#cite_note-10)[[10]](./Principle_of_least_astonishment#cite_note-11)[[11]](./Principle_of_least_astonishment#cite_note-12)

 

The law first appeared in print in 1972:[[12]](./Principle_of_least_astonishment#cite_note-13)

 

For those parts of the system which cannot be adjusted to the peculiarities of the user, the designers of a systems programming language should obey the "Law of Least Astonishment." In short, this law states that every construct in the system should behave exactly as its syntax suggests. Widely accepted conventions should be followed whenever possible, and exceptions to previously established rules of the language should be minimal.

 

## Formulation

 

A textbook formulation is: "People are part of the system. The design should match the user's experience, expectations, and [mental models](./Mental_model)."[[13]](./Principle_of_least_astonishment#cite_note-SaltzerKaashoek2009-14)

 

The principle aims to leverage the existing knowledge of users to minimize the [learning curve](./Learning_curve), for instance by designing interfaces that borrow heavily from "functionally similar or analogous programs with which your users are likely to be familiar".[[2]](./Principle_of_least_astonishment#cite_note-Raymond2004-2) User expectations in this respect may be closely related to a particular [computing platform](./Computing_platform) or [tradition](./Tradition). For example, [Unix](./Unix) command line programs are expected to follow certain conventions with respect to [switches](./Switch_(command_line)),[[2]](./Principle_of_least_astonishment#cite_note-Raymond2004-2) and [widgets](./GUI_widget) of [Microsoft Windows](./Microsoft_Windows) programs are expected to follow certain conventions with respect to [keyboard shortcuts](./Keyboard_shortcut).[[14]](./Principle_of_least_astonishment#cite_note-Petroutsos2010-15) In more abstract settings like an [API](./Application_programming_interface), the expectation that [function](./Function_(computer_science)) or method names intuitively match their behavior is another example.[[15]](./Principle_of_least_astonishment#cite_note-16) This practice also involves the application of sensible [defaults](./Default_(computer_science)).[[4]](./Principle_of_least_astonishment#cite_note-rexx-5)

 

When two elements of an interface conflict, or are ambiguous, the behavior should be that which will least surprise the [user](./User_(computing)); in particular a [programmer](./Programmer) should try to think of the behavior that will least surprise someone who uses the program, rather than that behavior that is natural from knowing the inner workings of the program.[[4]](./Principle_of_least_astonishment#cite_note-rexx-5)

 

The choice of "least surprising" behavior can depend on the expected audience (for example, [end users](./End_user), [programmers](./Programmer), or [system administrators](./System_administrator)).[[2]](./Principle_of_least_astonishment#cite_note-Raymond2004-2)

 

## Examples

 

Websites offering [keyboard shortcuts](./Keyboard_shortcut) often allow pressing ? to see the available shortcuts.  Examples include [Gmail](./Gmail),[[16]](./Principle_of_least_astonishment#cite_note-Gmail_Keyboard_Shortcuts-17) [YouTube](./YouTube),[[17]](./Principle_of_least_astonishment#cite_note-18) and [Jira](./Jira_(software)).[[18]](./Principle_of_least_astonishment#cite_note-Jira_Using_Keyboard_Shortcuts-19)

 

In [Windows operating systems](./Microsoft_Windows) and some [desktop environments](./Desktop_environment) for [Linux](./Linux), the F1 [function key](./Function_key) typically opens the [help program](./User_assistance) for an [application](./Application_software).  A similar keyboard shortcut in [macOS](./MacOS) is ⌘ [Command](./Command_key)+⇧ Shift+/. Users expect a help [window](./Window_(computing)) or [context menu](./Context_menu) when they press the usual help shortcut key(s). Software that instead uses this shortcut for another feature is likely to cause astonishment if no help appears.[[19]](./Principle_of_least_astonishment#cite_note-20)

 

A [programming language](./Programming_language)'s [standard library](./Standard_library) usually provides a [function](./Subroutine) similar to the [pseudocode](./Pseudocode) `ParseInteger(string, radix)`, which creates a machine-readable [integer](./Integer_(computer_science)) from a [string](./String_(computer_science)) of human-readable [digits](./Numerical_digit). The [radix](./Radix) conventionally [defaults](./Default_argument) to 10, meaning the string is interpreted as [decimal](./Decimal) (base 10). This function usually supports other bases, like [binary](./Binary_number) (base 2) and [octal](./Octal) (base 8), but only when they are specified explicitly. In a departure from this convention, [JavaScript](./JavaScript) originally defaulted to base 8 for strings beginning with "0", causing [developer](./Programmer) confusion and [software bugs](./Software_bug).[[20]](./Principle_of_least_astonishment#cite_note-21) This was discouraged in ECMAScript 3 and dropped in ECMAScript 5.[[21]](./Principle_of_least_astonishment#cite_note-22)

 

Some development communities like FreeBSD[[22]](./Principle_of_least_astonishment#cite_note-23) use POLA as one of the guidelines for what makes an unsurprising user experience.

 

## See also

 
- [DWIM](./DWIM) (do what I mean)
- [Convention over configuration](./Convention_over_configuration)
- [Human interface guidelines](./Human_interface_guidelines)
- [Look and feel](./Look_and_feel)
- [Occam's razor](./Occam's_razor)
- [WYSIWYG](./WYSIWYG)
- [List of software development philosophies](./List_of_software_development_philosophies)
- [User experience design](./User_experience_design)

 

## Notes

  
1. [↑](./Principle_of_least_astonishment#cite_ref-4) Alternatively a **law of least surprise** or **rule of least surprise**[[2]](./Principle_of_least_astonishment#cite_note-Raymond2004-2)[[3]](./Principle_of_least_astonishment#cite_note-3)

 

## References

 
1. [↑](./Principle_of_least_astonishment#cite_ref-1) Seebach, Peter (2001-08-01). ["The Principle of Least Astonishment"](https://web.archive.org/web/20140201183037/https://www.ibm.com/developerworks/web/library/us-cranky10/index.html). *The cranky user*. IBM DeveloperWorks. Archived from [the original](https://www.ibm.com/developerworks/web/library/us-cranky10/index.html) on 2014-02-01. Retrieved 2014-01-23.
2. [1](./Principle_of_least_astonishment#cite_ref-Raymond2004_2-0) [2](./Principle_of_least_astonishment#cite_ref-Raymond2004_2-1) [3](./Principle_of_least_astonishment#cite_ref-Raymond2004_2-2) [4](./Principle_of_least_astonishment#cite_ref-Raymond2004_2-3) [Raymond, Eric Steven](./Eric_S._Raymond) (2003). "Applying the Rule of Least Surprise". [*The Art of Unix Programming*](http://www.catb.org/~esr/writings/taoup/html/ch11s01.html). faqs.org. p. 20. [ISBN](./ISBN_(identifier)) [978-0-13-142901-7](./Special:BookSources/978-0-13-142901-7). Retrieved 2020-08-23.
3. [↑](./Principle_of_least_astonishment#cite_ref-3) [James, Geoffrey](./Geoffrey_James_(journalist)) (1987). [*The Tao of Programming*](https://www.canonical.org/~kragen/tao-of-programming.html#book4). InfoBooks. 4.1. [ISBN](./ISBN_(identifier)) [0-931137-07-1](./Special:BookSources/0-931137-07-1). Retrieved 2014-02-05.
4. [1](./Principle_of_least_astonishment#cite_ref-rexx_5-0) [2](./Principle_of_least_astonishment#cite_ref-rexx_5-1) [3](./Principle_of_least_astonishment#cite_ref-rexx_5-2) [Cowlishaw, M. F.](./Mike_Cowlishaw) (1984). ["The design of the REXX language"](https://www.cs.tufts.edu/~nr/cs257/archive/mike-cowlishaw/rexx.pdf) (PDF). *IBM Systems Journal*. **23** (4): 333. [doi](./Doi_(identifier)):[10.1147/sj.234.0326](https://doi.org/10.1147%2Fsj.234.0326). Retrieved 2014-01-23. Could there be a high astonishment factor associated with the new feature? If a feature is accidentally misapplied by the user and causes what appears to him to be an unpredictable result, that feature has a high astonishment factor and is therefore undesirable. If a necessary feature has a high astonishment factor, it may be necessary to redesign the feature.
5. [↑](./Principle_of_least_astonishment#cite_ref-6) Southworth, R. N. (December 1967). Southworth, R. N. (ed.). ["Proposal for PL/I Pseudo-name"](https://dl.acm.org/doi/10.1145/1139502.1139504). *ACM SIGPLAN Notices*. **2** (12) (PL/I Bulletin no. 5 ed.): 6. [doi](./Doi_(identifier)):[10.1145/1139502.1139504](https://doi.org/10.1145%2F1139502.1139504). [ISSN](./ISSN_(identifier)) [0362-1340](https://search.worldcat.org/issn/0362-1340). [S2CID](./S2CID_(identifier)) [12180929](https://api.semanticscholar.org/CorpusID:12180929).
6. [↑](./Principle_of_least_astonishment#cite_ref-7) Date, C. J. (11 February 2022). [*Database Dreaming Volume I: Relational Writings Revised and Revived*](https://books.google.com/books?id=ISVeEAAAQBAJ&pg=PT47). Technics Publications. Ch.2, Reference 36. [ISBN](./ISBN_(identifier)) [978-1-63462-984-3](./Special:BookSources/978-1-63462-984-3). As a friend of mine once remarked to me—this must have been sometime in the late 1960s—whatever else you might say about it, there's one thing that PL/I is most definitely not, and that's 'the language of least astonishment.'
7. [↑](./Principle_of_least_astonishment#cite_ref-8) Tremblay, Jean-Paul; Sorenson, Paul G. (1985). *The theory and practice of compiler writing*. New York: McGraw-Hill. [ISBN](./ISBN_(identifier)) [9780070651616](./Special:BookSources/9780070651616). PL/I is the major bad example here; it is strewn with constructs which do not do what the programmer thinks, as exemplified with FIXED division.
8. [↑](./Principle_of_least_astonishment#cite_ref-9) Holt, Richard C. (May 1973). ["Teaching the fatal disease: (or) introductory computer programming using PL/I"](https://plg.uwaterloo.ca/~holt/papers/fatal_disease.html). *ACM SIGPLAN Notices*. **8** (5): 8–23. [doi](./Doi_(identifier)):[10.1145/986948.986950](https://doi.org/10.1145%2F986948.986950). unfortunately, the expression '25 + 1/3' yields 5.33333333333333
9. [↑](./Principle_of_least_astonishment#cite_ref-10) Golden, Donald (October 1980). ["A plea for friendly software"](https://doi.org/10.1145%2F1010884.1010885). *ACM SIGSOFT Software Engineering Notes*. **5** (4): 4–5. [doi](./Doi_(identifier)):[10.1145/1010884.1010885](https://doi.org/10.1145%2F1010884.1010885). Lest the non-PL/I programmer come to the erroneous conclusion that PL/I is without flaws, consider the following examples of PL/I's hostility. The rules for type conversion in PL/I are enough to give programmers ulcers. What other language would produce a fatal error when evaluating the expression (25 + 1/3)? (Just as bad, if you suppress the error checking, the result of evaluating the expression is 5.3333...)
10. [↑](./Principle_of_least_astonishment#cite_ref-11) Stansifer, Ryan D. (1995). [*The Study of Programming Languages*](https://archive.org/details/studyofprogrammi0000stan/page/122/mode/2up?q=astonishment). Englewood Cliffs, N.J. : Prentice Hall. p. 123. [ISBN](./ISBN_(identifier)) [978-0-13-726936-5](./Special:BookSources/978-0-13-726936-5). PL/I is infamous in this regard, as it converts nearly any type into any other type, sometimes with surprising results. Consider the expression 1/3 + 25. In PL/I this expression has the value 5.33333333333. Why? One-third is computed to 15 digits of precision, 14 to the right of the decimal point. Then 25 is coerced to the same precision, losing the most significant digit 2! This does raise an error in PL/I, but the default is to ignore it. This first appeared in print in Barron 1968, where it is given as a violation of a folk law of language design: 'the law of least astonishment.'
11. [↑](./Principle_of_least_astonishment#cite_ref-12) ["Enterprise PL/I for z/OS 5.3 - Language Reference"](https://www.ibm.com/docs/en/SSY2V3_5.3.0/lr/lrm.pdf#page=110) (PDF). IBM. March 2021. pp. 57–62. Consider the following expression: 25+1/3. The result of evaluating this expression is undefined and the FIXEDOVERFLOW condition is raised because FIXED division results in a value of maximum implementation defined precision. [...] The results of the two evaluations are reached as shown in Table 29.
12. [↑](./Principle_of_least_astonishment#cite_ref-13) Bergeron, R.D.; Gannon, J.D.; Shecter, D.P.; Tompa, F.W.; Dam, A. Van (1972). "Systems Programming Languages". *Advances in Computers*. **12**: 175–284. [doi](./Doi_(identifier)):[10.1016/s0065-2458(08)60510-0](https://doi.org/10.1016%2Fs0065-2458%2808%2960510-0). [ISBN](./ISBN_(identifier)) [9780120121120](./Special:BookSources/9780120121120).
13. [↑](./Principle_of_least_astonishment#cite_ref-SaltzerKaashoek2009_14-0) Saltzer, J. H.; [Kaashoek, Frans](./Frans_Kaashoek) (2009). [*Principles of computer system design: an introduction*](https://books.google.com/books?id=I-NOcVMGWSUC&pg=PA85). Morgan Kaufmann. p. 85. [ISBN](./ISBN_(identifier)) [978-0-12-374957-4](./Special:BookSources/978-0-12-374957-4).
14. [↑](./Principle_of_least_astonishment#cite_ref-Petroutsos2010_15-0) Petroutsos, Evangelos (2010). [*Mastering Microsoft Visual Basic 2010*](https://books.google.com/books?id=x7LZTSVKZDoC&pg=PA133). Wiley. p. 133. [ISBN](./ISBN_(identifier)) [978-0-470-53287-4](./Special:BookSources/978-0-470-53287-4).
15. [↑](./Principle_of_least_astonishment#cite_ref-16) [Bloch, Joshua](./Joshua_Bloch) (2006). ["How to design a good API and why it matters"](https://portal.acm.org/citation.cfm?id=1176622). *Proceeding OOPSLA '06 Companion to the 21st ACM SIGPLAN symposium on Object-oriented programming systems, languages, and applications*. Association for Computing Machinery. pp. 506–7. [doi](./Doi_(identifier)):[10.1145/1176617.1176622](https://doi.org/10.1145%2F1176617.1176622). [ISBN](./ISBN_(identifier)) [1-59593-491-X](./Special:BookSources/1-59593-491-X). [S2CID](./S2CID_(identifier)) [27230400](https://api.semanticscholar.org/CorpusID:27230400).
16. [↑](./Principle_of_least_astonishment#cite_ref-Gmail_Keyboard_Shortcuts_17-0) Vivian (2013-06-21). ["Keyboard shortcuts for Gmail"](https://support.google.com/mail/answer/6594). Google Inc. Retrieved 2013-07-27.
17. [↑](./Principle_of_least_astonishment#cite_ref-18) ["Keyboard shortcuts for YouTube - YouTube Help"](https://support.google.com/youtube/answer/7631406?hl=en). *support.google.com*. Retrieved 2022-08-16.
18. [↑](./Principle_of_least_astonishment#cite_ref-Jira_Using_Keyboard_Shortcuts_19-0) ["Using Keyboard Shortcuts"](https://confluence.atlassian.com/display/JIRA/Using+Keyboard+Shortcuts#UsingKeyboardShortcuts-AccessingtheKeyboardShortcutsDialogBox). Atlassian. Retrieved 2013-07-27.
19. [↑](./Principle_of_least_astonishment#cite_ref-20) Keizer, G. (1 March 2010). ["Microsoft: Don't press F1 key in Windows XP"](https://www.computerworld.com/article/2520194/microsoft--don-t-press-f1-key-in-windows-xp.html). *Computerworld*. Retrieved 10 Nov 2019.
20. [↑](./Principle_of_least_astonishment#cite_ref-21) ["Why does the radix for JavaScript's parseInt default to 8?"](https://stackoverflow.com/questions/5600366/why-does-the-radix-for-javascripts-parseint-default-to-8). *Stack Overflow*. 8 April 2011.
21. [↑](./Principle_of_least_astonishment#cite_ref-22) ["parseInt()"](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt), *Mozilla Developer Network (MDN)*, 15 March 2024, If the input string begins with "0" (a zero), radix is assumed to be 8 (octal) or 10 (decimal). Exactly which radix is chosen is implementation-dependent. ECMAScript 5 clarifies that 10 (decimal) should be used, but not all browsers support this yet.
22. [↑](./Principle_of_least_astonishment#cite_ref-23) ["Frequently Asked Questions for FreeBSD 2.X, 3.X and 4.X"](https://docs.freebsd.org/doc/4.6-RELEASE/usr/share/doc/faq/book.html#DEFINE-POLA). FreeBSD. 2002-06-11. Retrieved 2023-02-15.

 

## External links

 
- [Principle of Least Astonishment](https://c2.com/cgi/wiki?PrincipleOfLeastAstonishment) at [Portland Pattern Repository](./Portland_Pattern_Repository)