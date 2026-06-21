---
source: https://en.wikipedia.org/wiki/User_story
fetched: 2026-06-20
---

Informal description of one or more features of a software system 
|  | Some of this article'slisted sourcesmay not bereliable.Please help improve this article by looking for better, more reliable sources. Unreliable citations may be challenged and removed.(August 2017)(Learn how and when to remove this message) |
| --- | --- |

 

 
| Part of a series on |
| --- |
| Software development |
| Core activitiesData modelingProcessesRequirementsDesignConstructionEngineeringTestingDebuggingDeploymentMaintenance |
| Paradigms, modelsAgileCleanroomIncrementalPrototypingSpiralV modelWaterfall |
| Methodologies, frameworksASDDADDevOpsDSDMFDDIIDKanbanLean SDLeSSMDEMSFPSPRADRUPSAFeScrumSEMATTDDTSPUPXP |
| Supporting disciplinesConfiguration managementDeployment managementDocumentationProject managementQuality assuranceUser experience |
| PracticesATDDBDDCCOCDCIDDDPPSBEStand-upTDDXP |
| ToolsBuild automationCompilerDebuggerGUI builderIDEInfrastructure as codeProfilerRelease automationUML modeling |
| Standards, bodies of knowledgeCMMIIEEE standardsIREBISO 9001ISO/IEC standardsITILOMGPMBOKSWEBOK |
| GlossariesArtificial intelligenceComputer scienceElectrical and electronics engineering |
| OutlinesSoftware developmentComputer programmingProgramming languagesCC++C#JavaJavaScriptPerlPythonRust |
| vte |

 

In [software development](./Software_development) and [product management](./Product_management), a **user story** is an informal, natural language description of [features](./Software_feature) of a software system. They are written from the perspective of an [end user](./User_(computing)#End_user) or [user of a system](./User_(system)), and may be recorded on index cards, [Post-it notes](./Post-it_note), or digitally in specific management software.[[1]](./User_story#cite_note-1) Depending on the product, user stories may be written by different stakeholders like client, user, manager, or development team.

 

User stories are a type of [boundary object](./Boundary_object). They facilitate [sensemaking](./Sensemaking) and communication; and may help software teams document their understanding of the system and its context.[[2]](./User_story#cite_note-2)

 

## History

 
- 1997: [Kent Beck](./Kent_Beck) introduces user stories at the [Chrysler C3 project](./Chrysler_Comprehensive_Compensation_System) in Detroit.
- 1998: [Alistair Cockburn](./Alistair_Cockburn) visited the C3 project and coined the phrase "A user story is a promise for a conversation."[[3]](./User_story#cite_note-3)
- 1999: [Kent Beck](./Kent_Beck) published the first edition of the book *Extreme Programming Explained*, introducing [Extreme Programming](./Extreme_Programming) (XP),[[4]](./User_story#cite_note-4) and the usage of user stories in the [planning game](./Planning_game).
- 2001: [Ron Jeffries](./Ron_Jeffries) proposed a "Three Cs" formula for user story creation:[[5]](./User_story#cite_note-5) 
- The *Card* (or often a [post-it note](./Post-it_note)) is a tangible physical token to hold the concepts;
- The *Conversation* is between the stakeholders (customers, users, developers, testers, etc.). It is verbal and often supplemented by documentation;
- The *Confirmation* ensures that the objectives of the conversation have been reached.

- 2001: The XP team at Connextra[[6]](./User_story#cite_note-Connextra-6) in London devised the user story format and shared examples with others.
- 2004: [Mike Cohn](./Mike_Cohn) generalized the principles of user stories beyond the usage of cards in his book *User Stories Applied: For Agile Software Development*[[7]](./User_story#cite_note-Cohn2004-7) that is now considered the standard reference for the topic according to [Martin Fowler](./Martin_Fowler_(software_engineer)).[[8]](./User_story#cite_note-8) Cohn names Rachel Davies as the inventor of user stories.[[9]](./User_story#cite_note-9) While Davies was a team member at Connextra she credits the team as a whole with the invention.[*[citation needed](./Wikipedia:Citation_needed)*]
- 2014: After a first article in 2005[[10]](./User_story#cite_note-10) and a blog post in 2008,[[11]](./User_story#cite_note-11) in 2014 Jeff Patton published the user-story mapping technique, which intends to improve with a systematic approach the identification of user stories and to structure the stories to give better visibility to their interdependence.[[12]](./User_story#cite_note-12)

 

## Principle

 

User stories are written by or for users or customers to influence the functionality of the system being developed. In some teams, the product manager (or [product owner](./Product_owner) in [Scrum](./Scrum_(development))), is primarily responsible for formulating user stories and organizing them into a [product backlog](./Product_backlog). In other teams, anyone can write a user story. User stories can be developed through discussion with stakeholders, based on [personas](./Persona_(user_experience)) or are simply made up.

 

### Common templates

 

User stories may follow one of several formats or templates.

 

The most common is the *Connextra template*, stated below.[[13]](./User_story#cite_note-13)[[7]](./User_story#cite_note-Cohn2004-7)[[14]](./User_story#cite_note-14) [Mike Cohn](./Mike_Cohn) suggested the "so that" clause is optional although still often helpful.[[15]](./User_story#cite_note-so-that-optional-15)

 
```
As a <role> I can <capability>, so that <receive benefit>

```
 

Chris Matts suggested that "hunting the value" was the first step in successfully delivering software, and proposed this alternative:[[16]](./User_story#cite_note-feature-injection-template-16)

 
```
In order to <receive benefit> as a <role>, I can <goal/desire>

```
 

Another template based on the [Five Ws](./Five_Ws) specifies:[[17]](./User_story#cite_note-17)

 
```
As <who> <when> <where>, I want <what> because <why>

```
 

A template that's commonly used to improve security is called the "Evil User Story" or "Abuse User Story" and is used as a way to think like a hacker in order to consider scenarios that might occur in a cyber-attack. These stories are written from the perspective of an attacker attempting to compromise or damage the application, rather the typical personae found in a user story:[[18]](./User_story#cite_note-evil-storytemplate-18)

 
```
As a disgruntled employee, I want to wipe out the user database to hurt the company

```
 

## Examples

 Screening quiz (epic story)As the HR manager, I want to create a screening quiz so that I can understand whether I want to send possible recruits to the functional manager.[[19]](./User_story#cite_note-alexandercowan-19) Quiz recallAs a manager, I want to browse my existing quizzes so I can recall what I have in place and figure out if I can just reuse or update an existing quiz for the position I need now.[[19]](./User_story#cite_note-alexandercowan-19) Limited backupAs a user, I can indicate folders not to back up so that my backup drive is not filled up with things I do not need to be saved.[[20]](./User_story#cite_note-:1-20) 

## Usage

 

A central part of many agile development methodologies, such as in [extreme programming](./Extreme_programming)'s  [planning game](./Extreme_Programming_Practices#Planning_game), user stories describe what may be built in the software product. User stories are prioritized by the customer (or the product owner in [Scrum](./Scrum_(development))) to indicate which are most important for the system and will be broken down into tasks and estimated by the developers. One way of estimating is by giving each task a number of story points selected from the [Fibonacci sequence](./Fibonacci_sequence): 1, 2, 3, 5, 8, 13, with the simplest tasks given a score of 1 and more complex tasks 
given higher scores. 

 

When user stories are about to be implemented, the developers should have the possibility to talk to the customer about it. The short stories may be
difficult to interpret, may require some background knowledge or the requirements may have changed since the story was written.

 

User stories can be expanded to add detail based on these conversations. This can include notes, attachments and acceptance criteria.

 

### Acceptance criteria

 

Mike Cohn defines acceptance criteria as "notes about what the story must do in order for the product owner to accept it as complete."[[21]](./User_story#cite_note-mikecohn-21) They define the boundaries of a user story and are used to confirm when a story is completed and working as intended.

 

The appropriate amount of information to be included in the acceptance criteria varies by team, program and project. Some may include 'predecessor criteria', "The user has already logged in and has already edited his information once".[*[quote needs citation](./Wikipedia:Inline_citation#When_you_must_use_inline_citations)*] Some may write the acceptance criteria in typical agile format, [Given-When-Then](./Given-When-Then). Others may simply use bullet points taken from original requirements gathered from customers or stakeholders.[[21]](./User_story#cite_note-mikecohn-21)
In order for a story to be considered done or complete, all acceptance criteria must be met.

 

## Benefits

 

There is no good evidence that using user stories increases software success or developer productivity. However, user stories facilitate sensemaking without undue problem structuring, which is linked to success.[[22]](./User_story#cite_note-22)

 

## Limitations

 

Limitations of user stories include:

 
- **Scale-up problem**: User stories written on small physical cards are hard to maintain, difficult to scale to large projects and troublesome for geographically distributed teams.
- **Vague, informal and incomplete**: User story cards are regarded as conversation starters. Being informal, they are open to many interpretations. Being brief, they do not state all of the details necessary to implement a feature. Stories are therefore inappropriate for reaching formal agreements or writing legal contracts.[[23]](./User_story#cite_note-23)
- **Lack of non-functional requirements**: User stories rarely include performance or non-functional requirement details, so non-functional tests (e.g. response time) may be overlooked.
- **Don't necessarily represent how technology has to be built:** Since user stories are often written from the business perspective, once a technical team begins to implement, it may find that technical constraints require effort which may be broader than the scope of an individual story. Sometimes splitting stories into smaller ones can help resolve this. Other times, 'technical-only' stories are most appropriate. These 'technical-only' stories may be challenged by the business stakeholders as not delivering value that can be demonstrated to customers/stakeholders.

 

## Relationship to epics, themes and initiatives/programs

 

In many contexts, user stories are used and also summarized in groups for ontological, semantic and organizational reasons. Initiative is also referred to as Program in certain scaled agile frameworks. The different usages depend on the point-of-view, e.g. either looking from a user perspective as product owner in relation to features or a company perspective in relation to task organization.

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/b/bd/User_Story_Map_in_Action.png/500px-User_Story_Map_in_Action.png)](./File:User_Story_Map_in_Action.png)A story map in action, with epics on the top to structure stories  

While some suggest to use 'epic' and 'theme' as labels for any thinkable kind of grouping of user stories, organization management tends to use it for strong structuring and uniting work loads. For instance, [Jira](./Jira_(software)) seems to use a [hierarchically](./Hierarchy) organized [to-do-list](./To-do_list), in which they named the first level of to-do-tasks 'user-story', the second level 'epics' (grouping of user stories) and the third level 'initiatives' (grouping of epics). However, initiatives are not always present in product management development and just add another level of granularity. In Jira, 'themes' exist (for tracking purposes) that allow to cross-relate and group items of *different parts of the fixed hierarchy*.[[24]](./User_story#cite_note-24)[[25]](./User_story#cite_note-25)

 

In this usage, Jira shifts the meaning of themes in an organization perspective: e.g how much time did we spend on developing theme "xyz". But another definition of themes is: a set of stories, epics, features etc for a user that forms a *common semantic unit or goal*. There is probably not a common definition because different approaches exist for different styles of product design and development. In this sense, some also suggest to not use any kind of hard groups and hierarchies.[[26]](./User_story#cite_note-26)[[27]](./User_story#cite_note-27)[[28]](./User_story#cite_note-28)[[29]](./User_story#cite_note-29)[[30]](./User_story#cite_note-30)[[31]](./User_story#cite_note-31)

 

### Theme

 

Multiple epics or many very large stories that are closely related are summarized as themes. A common explanation of epics is also: so much work that requires many sprints, or in scaled frameworks -- a Release Train or Solution Train.

 

### Initiative

 

Multiple themes, epics, or stories grouped together hierarchically.[[32]](./User_story#cite_note-32)

 

### Epic

 

Multiple themes or stories grouped together by ontology and/or semantic relationship.

 

## Story map

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/7/73/User_story_mapping.jpg/960px-User_story_mapping.jpg)](./File:User_story_mapping.jpg)User story mapping 

A story map[[33]](./User_story#cite_note-33) organises user stories according to a narrative flow that presents the big picture of the product.  The technique was developed by Jeff Patton from 2005 to 2014 to address the risk of projects flooded with very detailed user stories that distract from realizing the product's main objectives.[*[citation needed](./Wikipedia:Citation_needed)*]

 

User story mapping[[34]](./User_story#cite_note-34) uses workshops with users to identify first the main business activities.  Each of these main activities may involve several kinds of users or personas.

 

The horizontal cross-cutting narrative line is then drawn by identifying the main tasks of the individual user involved in these business activities. The line is kept throughout the project. More detailed user stories are gathered and collected as usual with the user story practice. But each new user story is either inserted into the narrative flow or related vertically to a main task.

 

The horizontal axis corresponds to the coverage of the product objectives, and the vertical axis to the needs of the individual users.

 

In this way it becomes possible to describe even large systems without losing the big picture.

 

Story maps can easily provide a two-dimensional graphical visualization of the [product backlog](./Product_backlog): At the top of the map are the headings under which stories are grouped, usually referred to as 'epics' (big coarse-grained user stories), 'themes' (collections of related user stories[[35]](./User_story#cite_note-35)) or 'activities'. These are identified by orienting at the user’s workflow or "the order you'd explain the behavior of the system". Vertically, below the epics, the actual story cards are allocated and ordered by priority. The first horizontal row is a "walking skeleton"[[36]](./User_story#cite_note-36)  and below that represents increasing sophistication.[[37]](./User_story#cite_note-37)[*[clarification needed](./Wikipedia:Please_clarify)*]

 

## User journey map

 

A user journey map[[38]](./User_story#cite_note-38) intends to show the big picture but for a single user category.  Its narrative line focuses on the chronology of phases and actions that a single user has to perform in order to achieve their objectives.

 

This allows to map the user experience beyond a set of user stories. Based on user feedback, the positive and negative emotions can be identified across the journey. Points of friction or unfulfilled needs can be identified on the map.  This technique is used to improve the design of a product,[[39]](./User_story#cite_note-39) allowing to engage users in participatory approaches.[[40]](./User_story#cite_note-40)

 

## Comparing with use cases

 

A [use case](./Use_case) has been described as "a generalized description of a set of interactions between the system and one or more actors, where an actor is either a user or another system."[[41]](./User_story#cite_note-41) While user stories and use cases have some similarities, there are several differences between them.

 
|  | User Stories | Use Cases |
| --- | --- | --- |
| Similarities | Generally formulated in users' everyday language. They should help the reader understand what the software should accomplish. | Written in users' everyday business language, to facilitate stakeholder communications. |
| Differences | Provide a small-scale and easy-to-use presentation of information, with little detail, thus remaining open to interpretation, through conversations with on-site customers. | Use cases organize requirements to form a narrative of how users relate to and use a system. Hence they focus on user goals and how interacting with a system satisfies the goals.[42]Use case flows describe sequences of interactions, and may be worded in terms of a formal model. A use case is intended to provide sufficient detail for it to be understood on its own. |
| Template | As a <type of user>, I can <some goal> so that <some reason>.[20] | Title: "goal the use case is trying to satisfy"Main Success Scenario: numbered list of stepsStep: "a simple statement of the interaction between the actor and a system"Extensions: separately numbered lists, one per ExtensionExtension: "a condition that results in different interactions from .. the main success scenario". An extension from main step 3 is numbered 3a, etc. |

 

[Kent Beck](./Kent_Beck), [Alistair Cockburn](./Alistair_Cockburn), [Martin Fowler](./Martin_Fowler_(software_engineer)) and others discussed this topic further on the c2.com wiki (the home of [extreme programming](./Extreme_programming)).[[43]](./User_story#cite_note-43)

 

## See also

 
- [Kanban board](./Kanban_board)
- [Persona (user experience)](./Persona_(user_experience))
- [Scenario (computing)](./Scenario_(computing))
- [Use case](./Use_case)

 

## References

  
1. [↑](./User_story#cite_ref-1) Dimitrijević, Sonja; Jovanović, Jelena; Devedžić, Vladan (2015). "A comparative study of software tools for user story management". *Information and Software Technology*. **57**: 352–368. [doi](./Doi_(identifier)):[10.1016/j.infsof.2014.05.012](https://doi.org/10.1016%2Fj.infsof.2014.05.012). a great number of software tools that provide, inter alia, support for practices based on user stories have emerged in recent years.
2. [↑](./User_story#cite_ref-2) Ralph, Paul (2015). "The Sensemaking-coevolution-implementation theory of software design". *Science of Computer Programming*. **101**: 21–41. [arXiv](./ArXiv_(identifier)):[1302.4061](https://arxiv.org/abs/1302.4061). [doi](./Doi_(identifier)):[10.1016/j.scico.2014.11.007](https://doi.org/10.1016%2Fj.scico.2014.11.007). [S2CID](./S2CID_(identifier)) [6154223](https://api.semanticscholar.org/CorpusID:6154223).
3. [↑](./User_story#cite_ref-3) ["Origin of story card is a promise for a conversation : Alistair.Cockburn.us"](https://web.archive.org/web/20210622215759/https://alistair.cockburn.us/coming-soon/). *alistair.cockburn.us*. Archived from [the original](http://alistair.cockburn.us/Origin+of+user+story+is+a+promise+for+a+conversation) on 22 June 2021. Retrieved 16 August 2017.
4. [↑](./User_story#cite_ref-4) [Beck, Kent](./Kent_Beck) (1999). *Extreme Programming Explained: Embrace Change*. Addison-Wesley. [ISBN](./ISBN_(identifier)) [9780201616415](./Special:BookSources/9780201616415). [OCLC](./OCLC_(identifier)) [41834882](https://search.worldcat.org/oclc/41834882).
5. [↑](./User_story#cite_ref-5) Jeffries, Ron (30 August 2001). ["Essential XP: Card, Conversation, Confirmation"](http://ronjeffries.com/xprog/articles/expcardconversationconfirmation/). [Archived](https://web.archive.org/web/20170512211534/http://ronjeffries.com/xprog/articles/expcardconversationconfirmation/) from the original on 12 May 2017. Retrieved 14 April 2017.
6. [↑](./User_story#cite_ref-Connextra_6-0) ["User Story Template"](https://www.agilealliance.org/glossary/user-story-template/). *agilealliance.org*. 17 December 2015. [Archived](https://web.archive.org/web/20200606161737/https://www.agilealliance.org/glossary/user-story-template/) from the original on 6 June 2020. Retrieved 18 April 2020.
7. [1](./User_story#cite_ref-Cohn2004_7-0) [2](./User_story#cite_ref-Cohn2004_7-1) Cohn, Mike (2004). *User Stories Applied: For Agile Software Development*. Addison-Wesley. [ISBN](./ISBN_(identifier)) [0321205685](./Special:BookSources/0321205685). [OCLC](./OCLC_(identifier)) [54365622](https://search.worldcat.org/oclc/54365622).
8. [↑](./User_story#cite_ref-8) Fowler, Martin (22 April 2013). ["User Story"](https://martinfowler.com/bliki/UserStory.html). *martinfowler.com*. [Archived](https://web.archive.org/web/20190714210315/https://martinfowler.com/bliki/UserStory.html) from the original on 14 July 2019. Retrieved 14 July 2019.
9. [↑](./User_story#cite_ref-9) Cohn, Mike. ["What Is a User Story Template and Why Does It Work So Well?"](https://www.mountaingoatsoftware.com/blog/why-the-three-part-user-story-template-works-so-well). *Mountain Goat Software*. Retrieved 9 January 2025.
10. [↑](./User_story#cite_ref-10) Patton, Jeff (January 2005). ["It's All In How You Slice It"](https://www.stickyminds.com/better-software-magazine-volume-issue/2005-01). *Better Software Magazine*: 16–22, 40. [Archived](https://web.archive.org/web/20190716193104/https://www.stickyminds.com/better-software-magazine-volume-issue/2005-01) from the original on 16 July 2019. Retrieved 16 July 2019.
11. [↑](./User_story#cite_ref-11) Patton, Jeff (8 October 2008). ["The New User Story Backlog is a Map"](https://www.jpattonassociates.com/the-new-backlog/). *Jeff Patton & Associates*. [Archived](https://web.archive.org/web/20190718153846/https://www.jpattonassociates.com/the-new-backlog/) from the original on 18 July 2019. Retrieved 16 July 2019.
12. [↑](./User_story#cite_ref-12) Patton, Jeff (2014). *User story mapping*. Economy, Peter, Fowler, Martin, Cooper, Alan, Cagan, Marty (First ed.). Beijing. [ISBN](./ISBN_(identifier)) [9781491904909](./Special:BookSources/9781491904909). [OCLC](./OCLC_(identifier)) [880566740](https://search.worldcat.org/oclc/880566740).`{{cite book}}`:  CS1 maint: location missing publisher ([link](./Category:CS1_maint:_location_missing_publisher))
13. [↑](./User_story#cite_ref-13) Lucassen, Garm; Dalpiaz, Fabiano; Werf, Jan Martijn E. M. van der; Brinkkemper, Sjaak (2016), Daneva, Maya; Pastor, Oscar (eds.), "The Use and Effectiveness of User Stories in Practice", *Requirements Engineering: Foundation for Software Quality*, Lecture Notes in Computer Science, vol. 9619, Springer International Publishing, pp. 205–222, [doi](./Doi_(identifier)):[10.1007/978-3-319-30282-9_14](https://doi.org/10.1007%2F978-3-319-30282-9_14), [ISBN](./ISBN_(identifier)) [978-3-319-30281-2](./Special:BookSources/978-3-319-30281-2), [S2CID](./S2CID_(identifier)) [26458219](https://api.semanticscholar.org/CorpusID:26458219), The most prevalent user story template is the 'original' one proposed by Connextra`{{citation}}`:  CS1 maint: work parameter with ISBN ([link](./Category:CS1_maint:_work_parameter_with_ISBN))
14. [↑](./User_story#cite_ref-14) ["Glossary: User Story Template"](https://www.agilealliance.org/glossary/user-story-template/). *agilealliance.org*. [Agile Alliance](./Agile_Alliance). 17 December 2015. [Archived](https://web.archive.org/web/20200203101132/https://www.agilealliance.org/glossary/user-story-template/) from the original on 3 February 2020. Retrieved 3 February 2020. Another name is the "Connextra format", in recognition of its origins
15. [↑](./User_story#cite_ref-so-that-optional_15-0) [Cohn, Mike](./Mike_Cohn) (25 April 2008). ["Advantages of the "As a user, I want" user story template"](http://www.mountaingoatsoftware.com/blog/advantages-of-the-as-a-user-i-want-user-story-template). *Mountaingoatsoftware.com*. [Archived](https://web.archive.org/web/20161218210740/http://www.mountaingoatsoftware.com/blog/advantages-of-the-as-a-user-i-want-user-story-template) from the original on 18 December 2016. Retrieved 18 December 2016. While I consider the so-that clause optional, I really like this template.
16. [↑](./User_story#cite_ref-feature-injection-template_16-0) Marcano, Antony (24 March 2011). ["Old Favourite: Feature Injection User Stories on a Business Value Theme"](http://antonymarcano.com/blog/2011/03/fi_stories/). *Antonymarcano.com*. [Archived](https://web.archive.org/web/20120702040122/http://antonymarcano.com/blog/2011/03/fi_stories/) from the original on 2 July 2012. Retrieved 23 February 2017.
17. [↑](./User_story#cite_ref-17) ["User Story"](https://t2informatik.de/en/smartpedia/user-story/). *t2informatik GmbH*. 25 September 2019. [Archived](https://web.archive.org/web/20200203095858/https://t2informatik.de/en/smartpedia/user-story/) from the original on 3 February 2020. Retrieved 3 February 2020. "As (who) (when) (where), I (want) because (why)." – this phrase is based on typical W questions: who, when, where, what and why.
18. [↑](./User_story#cite_ref-evil-storytemplate_18-0) Van der Veer, Rob (18 May 2020). ["SAMM Agile guidance"](https://github.com/OWASP/samm/blob/master/Current%20Releases/head/agile-guidance/agilenotes.md#abuse-stories). *[GitHub](./GitHub)*.
19. [1](./User_story#cite_ref-alexandercowan_19-0) [2](./User_story#cite_ref-alexandercowan_19-1) Cowan, Alexander. ["Your Best Agile User Story"](http://www.alexandercowan.com/best-agile-user-story/). *Cowan+*. [Archived](https://web.archive.org/web/20160325215047/http://www.alexandercowan.com/best-agile-user-story/) from the original on 25 March 2016. Retrieved 29 April 2016.
20. [1](./User_story#cite_ref-:1_20-0) [2](./User_story#cite_ref-:1_20-1) Cohn, Mike. ["User Stories"](https://www.mountaingoatsoftware.com/agile/user-stories). *Mountain Goat Software*. [Archived](https://web.archive.org/web/20160430023753/https://www.mountaingoatsoftware.com/agile/user-stories) from the original on 30 April 2016. Retrieved 27 April 2016.
21. [1](./User_story#cite_ref-mikecohn_21-0) [2](./User_story#cite_ref-mikecohn_21-1) Cohn, Mike. ["The Two Ways to Add Detail to User Stories"](https://www.mountaingoatsoftware.com/blog/preview/1691). *Mountain Goat Software blog*. [Archived](https://web.archive.org/web/20190408062320/https://www.mountaingoatsoftware.com/blog/preview/1691) from the original on 8 April 2019. Retrieved 8 April 2019.
22. [↑](./User_story#cite_ref-22) Ralph, Paul; Mohanani, Rahul (2015). "Is Requirements Engineering Inherently Counterproductive?". *2015 IEEE/ACM 5th International Workshop on the Twin Peaks of Requirements and Architecture*. IEEE. pp. 20–23. [doi](./Doi_(identifier)):[10.1109/TwinPeaks.2015.12](https://doi.org/10.1109%2FTwinPeaks.2015.12). [ISBN](./ISBN_(identifier)) [978-1-4673-7100-1](./Special:BookSources/978-1-4673-7100-1). [S2CID](./S2CID_(identifier)) [2873385](https://api.semanticscholar.org/CorpusID:2873385).
23. [↑](./User_story#cite_ref-23) ["Limitations of user stories"](http://www.ferolen.com/blog/limitations-of-user-stories/). Ferolen.com. 15 April 2008. [Archived](https://web.archive.org/web/20140413142352/http://www.ferolen.com/blog/limitations-of-user-stories/) from the original on 13 April 2014. Retrieved 9 April 2014.
24. [↑](./User_story#cite_ref-24) ["Epics, Themes, Stories, and Initiatives"](https://www.atlassian.com/agile/project-management/epics-stories-themes). *Atlassian*. [Archived](https://web.archive.org/web/20190130231414/https://www.atlassian.com/agile/project-management/epics-stories-themes) from the original on 30 January 2019. Retrieved 8 February 2019.
25. [↑](./User_story#cite_ref-25) ["User Stories"](https://www.atlassian.com/agile/project-management/user-stories). *Atlassian*. [Archived](https://web.archive.org/web/20190205002630/https://www.atlassian.com/agile/project-management/user-stories) from the original on 5 February 2019. Retrieved 8 February 2019.
26. [↑](./User_story#cite_ref-26) Britsch, Marcel (5 September 2017). ["The Basics: Epics, Stories, Themes & Features"](https://thedigitalbusinessanalyst.co.uk/epics-stories-themes-and-features-4637712cff5c). *The Digital Business Analyst*. [Archived](https://web.archive.org/web/20170921082050/https://thedigitalbusinessanalyst.co.uk/epics-stories-themes-and-features-4637712cff5c) from the original on 21 September 2017. Retrieved 8 February 2019.
27. [↑](./User_story#cite_ref-27) Cohn, Mike. ["User Stories, Epics and Themes"](https://www.mountaingoatsoftware.com/blog/stories-epics-and-themes). *Mountain Goat Software*. [Archived](https://web.archive.org/web/20190204205711/https://www.mountaingoatsoftware.com/blog/stories-epics-and-themes) from the original on 4 February 2019. Retrieved 8 February 2019.
28. [↑](./User_story#cite_ref-28) ["Scrum Alliance Member-Submitted Informational Articles"](https://www.scrumalliance.org/community/articles/2014/march/stories-versus-themes-versus-epics). [Archived](https://web.archive.org/web/20180911152200/https://www.scrumalliance.org/community/articles/2014/march/stories-versus-themes-versus-epics) from the original on 11 September 2018. Retrieved 11 September 2018.
29. [↑](./User_story#cite_ref-29) Guay, Constantin (26 January 2018). ["Scrum tips: Differences between epics, stories, themes and features"](https://const.fr/blog/agile/scrum-differences-epics-stories-themes-features/). [Archived](https://web.archive.org/web/20181119085244/https://const.fr/blog/agile/scrum-differences-epics-stories-themes-features/) from the original on 19 November 2018. Retrieved 8 February 2019.
30. [↑](./User_story#cite_ref-30) ["User Stories, Epics & Themes"](https://www.agile-academy.com/de/product-owner/user-stories-epics-themes/). 8 December 2021. [Archived](https://web.archive.org/web/20190209124534/https://www.scrum-academy.de/product-owner/wissen/user-stories-epics-themes/) from the original on 9 February 2019. Retrieved 8 December 2021.
31. [↑](./User_story#cite_ref-31) Cohn, Mike. ["You Don't Need a Complicated Story Hierarchy"](https://www.mountaingoatsoftware.com/blog/you-dont-need-a-complicated-story-hierarchy). *Mountain Goat Software*. [Archived](https://web.archive.org/web/20190510142725/https://www.mountaingoatsoftware.com/blog/you-dont-need-a-complicated-story-hierarchy) from the original on 10 May 2019. Retrieved 8 February 2019.
32. [↑](./User_story#cite_ref-32) ["Configuring initiatives and other hierarchy levels - Atlassian Documentation"](https://confluence.atlassian.com/jiraportfoliocloud/configuring-initiatives-and-other-hierarchy-levels-828785179.html). *confluence.atlassian.com*. [Archived](https://web.archive.org/web/20200205092403/https://confluence.atlassian.com/jiraportfoliocloud/configuring-initiatives-and-other-hierarchy-levels-828785179.html) from the original on 5 February 2020. Retrieved 5 February 2020. An 'initiative' is a very large body of work, which spans multiple epics and sometimes, multiple teams. [...] An initiative is also an issue type in Jira.
33. [↑](./User_story#cite_ref-33) Patton, Jeff (8 October 2008). ["The new user story backlog is a map"](http://jpattonassociates.com/the-new-backlog/). [Archived](https://web.archive.org/web/20170514005903/http://jpattonassociates.com/the-new-backlog/) from the original on 14 May 2017. Retrieved 17 May 2017.
34. [↑](./User_story#cite_ref-34) Patton, Jeff (Software developer) (2014). *User story mapping*. Economy, Peter,, Fowler, Martin, 1963-, Cooper, Alan, 1952-, Cagan, Marty (First ed.). Beijing. [ISBN](./ISBN_(identifier)) [978-1-4919-0490-9](./Special:BookSources/978-1-4919-0490-9). [OCLC](./OCLC_(identifier)) [880566740](https://search.worldcat.org/oclc/880566740).`{{cite book}}`:  CS1 maint: location missing publisher ([link](./Category:CS1_maint:_location_missing_publisher))
35. [↑](./User_story#cite_ref-35) Cohn, Mike. ["User Stories, Epics and Themes"](https://www.mountaingoatsoftware.com/blog/stories-epics-and-themes/). *Mountaingoatsoftware.com*. [Archived](https://web.archive.org/web/20170927041658/http://www.mountaingoatsoftware.com/blog/stories-epics-and-themes) from the original on 27 September 2017. Retrieved 26 September 2017.
36. [↑](./User_story#cite_ref-36) Cockburn, Alistair. ["Walking Skeleton"](http://alistair.cockburn.us/Walking+skeleton). [Archived](https://web.archive.org/web/20130924061832/http://alistair.cockburn.us/Walking+skeleton) from the original on 24 September 2013. Retrieved 4 March 2013.
37. [↑](./User_story#cite_ref-37) ["Story Mapping"](https://www.agilealliance.org/glossary/storymap/). Agile Alliance. 17 December 2015. [Archived](https://web.archive.org/web/20160623192419/https://www.agilealliance.org/glossary/storymap/) from the original on 23 June 2016. Retrieved 1 May 2016.
38. [↑](./User_story#cite_ref-38) Experience, World Leaders in Research-Based User. ["Journey Mapping 101"](https://www.nngroup.com/articles/journey-mapping-101/). *Nielsen Norman Group*. [Archived](https://web.archive.org/web/20200319021655/https://www.nngroup.com/articles/journey-mapping-101/) from the original on 19 March 2020. Retrieved 15 March 2020. `{{cite web}}`: `|first=` has generic name ([help](./Help:CS1_errors#generic_name))
39. [↑](./User_story#cite_ref-39) Richardson, Adam (15 November 2010). ["Using Customer Journey Maps to Improve Customer Experience"](https://hbr.org/2010/11/using-customer-journey-maps-to). *Harvard Business Review*. [ISSN](./ISSN_(identifier)) [0017-8012](https://search.worldcat.org/issn/0017-8012). [Archived](https://web.archive.org/web/20200322173349/https://hbr.org/2010/11/using-customer-journey-maps-to) from the original on 22 March 2020. Retrieved 15 March 2020.
40. [↑](./User_story#cite_ref-40) "Subversive participatory design | Proceedings of the 14th Participatory Design Conference: Short Papers, Interactive Exhibitions, Workshops - Volume 2". [doi](./Doi_(identifier)):[10.1145/2948076.2948085](https://doi.org/10.1145%2F2948076.2948085). [hdl](./Hdl_(identifier)):[11572/167104](https://hdl.handle.net/11572%2F167104). [S2CID](./S2CID_(identifier)) [15915593](https://api.semanticscholar.org/CorpusID:15915593). `{{cite journal}}`: Cite journal requires `|journal=` ([help](./Help:CS1_errors#missing_periodical))
41. [↑](./User_story#cite_ref-41) Cohn, Mike. ["Project Advantages of User Stories as Requirements"](http://www.mountaingoatsoftware.com/articles/27-advantages-of-user-stories-for-requirements). *Mountaingoatsoftware.com*. [Archived](https://web.archive.org/web/20120418001257/http://www.mountaingoatsoftware.com/articles/27-advantages-of-user-stories-for-requirements) from the original on 18 April 2012. Retrieved 26 September 2017.
42. [↑](./User_story#cite_ref-fowlercompare_42-0) Fowler, Martin (18 August 2003). ["UseCasesAndStories"](https://martinfowler.com/bliki/UseCasesAndStories.html). [Archived](https://web.archive.org/web/20170927112047/https://martinfowler.com/bliki/UseCasesAndStories.html) from the original on 27 September 2017. Retrieved 26 September 2017.
43. [↑](./User_story#cite_ref-43) ["User Story And Use Case Comparison"](http://www.c2.com/cgi/wiki?UserStoryAndUseCaseComparison). *C2.com*. [Archived](https://web.archive.org/web/20160902181205/http://c2.com/cgi/wiki?UserStoryAndUseCaseComparison) from the original on 2 September 2016. Retrieved 26 September 2017.

 

## Further reading

 
- Daniel H. Steinberg, Daniel W. Palmer, *Extreme Software Engineering*, Pearson Education, Inc., [ISBN](./ISBN_(identifier)) [0-13-047381-2](./Special:BookSources/0-13-047381-2).
- Mike Cohn, *User Stories Applied*, 2004, Addison Wesley, [ISBN](./ISBN_(identifier)) [0-321-20568-5](./Special:BookSources/0-321-20568-5).
- Mike Cohn, *Agile Estimating and Planning*, 2006, Prentice Hall, [ISBN](./ISBN_(identifier)) [0-13-147941-5](./Special:BookSources/0-13-147941-5).
- [Business Analyst Time](http://www.batimes.com/articles/user-stories-and-use-cases-dont-use-both.html)
- [Payton Consulting 'How user stories are different from IEEE requirements](http://www.payton-consulting.com/user-stories-different-requirements/) [Archived](https://web.archive.org/web/20150214125458/http://www.payton-consulting.com/user-stories-different-requirements/) 14 February 2015 at the [Wayback Machine](./Wayback_Machine)