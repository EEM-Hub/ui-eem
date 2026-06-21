---
source: https://en.wikipedia.org/wiki/Hick%27s_law
fetched: 2026-06-20
---

Time to make a decision as a result of the possible choices 
|  | This article includes a list ofgeneral references, butit lacks sufficient correspondinginline citations.Please help toimprovethis article byintroducingmore precise citations.(October 2013)(Learn how and when to remove this message) |
| --- | --- |

 

**Hick's law**, or the **Hick–Hyman law**, named after British and American psychologists [William Edmund Hick](./W._E._Hick) and [Ray Hyman](./Ray_Hyman), describes the time it takes for a person to make a decision as a result of the possible choices: increasing the number of choices will increase the decision time [logarithmically](./Logarithm). The Hick–Hyman law assesses cognitive information capacity in choice reaction experiments. The amount of time taken to process a certain amount of bits in the Hick–Hyman law is known as the "rate of gain of information". The plain language implication of the finding is that increasing the number of choices does not directly increase the time to choose. In other words, twice as many choices does not result in twice as long to choose. Also, because the relationship is logarithmic, the increase in time it takes to choose becomes less and less as the number of choices increases.

 

## Background

 

In 1868, [Franciscus Donders](./Franciscus_Donders) reported the relationship between having multiple [stimuli](./Stimulus_(psychology)) and choice reaction time. In 1885, J. Merkel discovered that the response time is longer when a stimulus belongs to a larger set of stimuli. Psychologists began to see similarities between this phenomenon and [information theory](./Information_Theory).[*[who?](./Wikipedia:Manual_of_Style/Words_to_watch#Unsupported_attributions)*]

 

Hick first began experimenting with this theory in 1951.[[1]](./Hick's_law#cite_note-1) In his first experiment, 10 lamps were arranged in a circle around the subject, each paired with a [Morse key](./Telegraph_key) operated by a different finger. A pre-punched tape activated a random lamp every 5 seconds. Four electric pens recorded each lamp activation on a moving paper strip as a [4-bit binary](./4-bit_computing#:~:text=With_4_bits,_it_is,digit_represented_by_four_bits.) code; when the subject pressed the corresponding key, the same pens recorded the response in the same format. The distance between the two marks on the paper gave the reaction time. Although the 4-bit encoding could represent up to 16 states (15 lamp positions plus "all clear"), Hick used only 10.

 

Hick performed a second experiment using the same task, while keeping the number of alternatives at 10. The participant performed the task the first two times with the instruction to perform the task as accurately as possible. For the last task, the participant was asked to perform the task as quickly as possible.

 

While Hick was stating that the relationship between reaction time and the number of choices was logarithmic, Hyman wanted to better understand the relationship between the reaction time and the mean number of choices. In Hyman's experiment, he had eight different lights arranged in a 6x6 matrix.[[2]](./Hick's_law#cite_note-2) Each of these different lights was given a name, so the participant was timed in the time it took to say the name of the light after it was lit. Further experiments changed the number of each different type of light. Hyman was responsible for determining a [linear relation](./Linear_relation) between reaction time and the information transmitted.

 

## Law

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/5/58/Hick%27s_law_plotted_data.svg/330px-Hick%27s_law_plotted_data.svg.png)](./File:Hick's_law_plotted_data.svg)Data from W. E. Hick (1952) demonstrating Hick's Law: The relationship between reaction time and number of response options across two participants (red and blue). 

Given *n* equally probable choices, the average reaction time *T* required to choose among the choices is approximately:

     T = b ⋅ ⋅   log  2   ⁡ ⁡  ( n + 1 )   {\displaystyle T=b\cdot \log _{2}(n+1)}  ![{\displaystyle T=b\cdot \log _{2}(n+1)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/0cef7e82355b3f5365f4f3eae52516ae042719da) 

where *b* is a constant that can be determined empirically by fitting a line to measured data. The [logarithm](./Logarithm) expresses depth of "choice tree" hierarchy – log2 indicates [binary search](./Binary_search) was performed. Addition of 1 to *n* takes into account the "uncertainty about whether to respond or not, as well as about which response to make."[[3]](./Hick's_law#cite_note-3)

 

In the case of choices with unequal probabilities, the law can be generalized as:

     T = b H   {\displaystyle T=bH}  ![{\displaystyle T=bH}](https://wikimedia.org/api/rest_v1/media/math/render/svg/7a35a7a1d9a8066a9928a8323009057a58952ebf) 

where *H* is strongly related to the [information-theoretic](./Information_theory) entropy of the decision, defined as

     H =  ∑ ∑   i   n    p  i    log  2   ⁡ ⁡  ( 1  /   p  i   + 1 )   {\displaystyle H=\sum _{i}^{n}p_{i}\log _{2}(1/p_{i}+1)}  ![{\displaystyle H=\sum _{i}^{n}p_{i}\log _{2}(1/p_{i}+1)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/265403ffa84fe0d0b8375e20c4187abe2c0e0de0) 

where *pi* refers to the probability of the *i*th alternative yielding the information-theoretic entropy.

 

Hick's law is similar in form to [Fitts's law](./Fitts's_law). Hick's law has a logarithmic form because people subdivide the total collection of choices into categories, eliminating about half of the remaining choices at each step, rather than considering each and every choice one-by-one, which would require linear time.

 

### Relation to IQ

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/1/1c/EN_HICK.png/250px-EN_HICK.png)](./File:EN_HICK.png)Roth's application of Hick's law
"Bit" is the unit of log2(n). 

E. Roth (1964) demonstrated a correlation between IQ and information processing speed, which is the [reciprocal](./Multiplicative_inverse) of the slope of the function:[[4]](./Hick's_law#cite_note-roth1964-4)

      Reaction Time  =  Movement Time  +     log  2   ⁡ ⁡  ( n )  Processing Speed     {\displaystyle {\text{Reaction Time}}={\text{Movement Time}}+{\frac {\log _{2}(n)}{\text{Processing Speed}}}}  ![{\displaystyle {\text{Reaction Time}}={\text{Movement Time}}+{\frac {\log _{2}(n)}{\text{Processing Speed}}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/74de26f1ffde8519c57b1b0325853c548c82d301) 

where *n* is the number of choices. The time it takes to come to a decision is proportional to:

 

        log  2   ⁡ ⁡  ( n )  Processing Speed     {\displaystyle {\frac {\log _{2}(n)}{\text{Processing Speed}}}}  ![{\displaystyle {\frac {\log _{2}(n)}{\text{Processing Speed}}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/e7aff1a168f4beb118c3f591e120e207d74a58da)

 

## Stimulus–response compatibility

 

The [stimulus–response compatibility](./Stimulus–response_compatibility) is known to also affect the choice [reaction time](./Reaction_time) for the Hick–Hyman law. This means that the response should be similar to the stimulus itself (such as turning a steering wheel to turn the wheels of the car). The action the user performs is similar to the response the driver receives from the car.

 

## Exceptions

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/3/31/Sigmoid2.jpg/250px-Sigmoid2.jpg)](./File:Sigmoid2.jpg)The sigmoid function remains a better representation than the linear function of the relationship between predictability and reaction time. 

Studies suggest that the search for a word within a randomly ordered list—in which the reaction time increases linearly according to the number of items—does not allow for the [generalization](./Generalization) of the [scientific law](./Scientific_law), considering that, in other conditions, the reaction time may not be linearly associated to the logarithm of the number of elements or even show other variations of the basic plane.

 

Exceptions to Hick's law have been identified in studies of verbal response to familiar stimuli, where there is no relationship or only a subtle increase in the reaction time associated with an increased number of elements,[[5]](./Hick's_law#cite_note-Longstreth1985-5) and saccade responses, where it was shown that there is either no relationship,[[6]](./Hick's_law#cite_note-Kveraga2002-6) or a decrease in the saccadic time with the increase of the number of elements, thus an antagonistic effect to that postulated by Hick's law.[[7]](./Hick's_law#cite_note-Lawrence2008-7)

 

The generalization of Hick's law was also tested in studies on the predictability of transitions associated with the reaction time of elements that appeared in a structured sequence.[[8]](./Hick's_law#cite_note-Stadler1992-8)[[9]](./Hick's_law#cite_note-Remillard2001-9) This process was first described as being in accordance to Hick's law,[[10]](./Hick's_law#cite_note-Jamieson2009-10) but more recently it was shown that the relationship between predictability and reaction time is [sigmoid](./Sigmoid_function), not [linear](./Linear_function) associated with different modes of action.[[11]](./Hick's_law#cite_note-Pavão2016-11)

 

Hick's law is sometimes cited to justify [menu](./Menu_(computing)) design decisions. For example, to find a given word (e.g. the name of a command) in a randomly ordered word list (e.g. a menu), scanning of each word in the list is required, consuming linear time, so Hick's law does not apply. However, if the list is alphabetical and the user knows the name of the command, he or she may be able to use a subdividing strategy that works in logarithmic time.[[12]](./Hick's_law#cite_note-12)

 

## See also

 
- [Power law of practice](./Power_law_of_practice)
- *[The Paradox of Choice](./The_Paradox_of_Choice)*
- [Fitts's Law](./Fitts's_law)

 

## Notes

  
1. [↑](./Hick's_law#cite_ref-1) Hick, W.E. (1952). ["On the rate of gain of information"](http://www2.psychology.uiowa.edu/faculty/mordkoff/InfoProc/pdfs/Hick%201952.pdf) (PDF). *Quarterly Journal of Experimental Psychology*. **4** (1): 11–26. [doi](./Doi_(identifier)):[10.1080/17470215208416600](https://doi.org/10.1080%2F17470215208416600). [S2CID](./S2CID_(identifier)) [39060506](https://api.semanticscholar.org/CorpusID:39060506).
2. [↑](./Hick's_law#cite_ref-2) Hyman, R (March 1953). "Stimulus information as a determinant of reaction time". *Journal of Experimental Psychology*. **45** (3): 188–96. [doi](./Doi_(identifier)):[10.1037/h0056940](https://doi.org/10.1037%2Fh0056940). [PMID](./PMID_(identifier)) [13052851](https://pubmed.ncbi.nlm.nih.gov/13052851). [S2CID](./S2CID_(identifier)) [17559281](https://api.semanticscholar.org/CorpusID:17559281).
3. [↑](./Hick's_law#cite_ref-3) Card, Stuart K.; Moran, Thomas P.; [Newell, A.](./Allen_Newell) (1983). *The Psychology of Human–Computer Interaction*. Hilldale, London: Lawrence Erlbaum.
4. [↑](./Hick's_law#cite_ref-roth1964_4-0) Roth, Erwin (1964). "Die Geschwindigkeit der Verarbeitung von Information und ihr Zusammenhang mit Intelligenz" [The speed of processing information and its connection with intelligence]. *Zeitschrift für Experimentelle und Angewandte Psychologie* (in German). **11**: 616–622.
5. [↑](./Hick's_law#cite_ref-Longstreth1985_5-0) Longstreth, L. E.; El-Zahhar, N.; Alcorn, M. B. (1985). "Exceptions to Hick's Law: Explorations With a Response Duration Measure". *Journal of Experimental Psychology: General*. **114** (4): 417–434. [doi](./Doi_(identifier)):[10.1037/0096-3445.114.4.417](https://doi.org/10.1037%2F0096-3445.114.4.417). [PMID](./PMID_(identifier)) [2934496](https://pubmed.ncbi.nlm.nih.gov/2934496).
6. [↑](./Hick's_law#cite_ref-Kveraga2002_6-0) Kveraga, K.; Boucher, L.; Hughes, H. C. (2002). "Saccades operate in Violation of Hick's law". *Experimental Brain Research*. **146** (3): 307–314. [doi](./Doi_(identifier)):[10.1007/s00221-002-1168-8](https://doi.org/10.1007%2Fs00221-002-1168-8). [PMID](./PMID_(identifier)) [12232687](https://pubmed.ncbi.nlm.nih.gov/12232687). [S2CID](./S2CID_(identifier)) [21845688](https://api.semanticscholar.org/CorpusID:21845688).
7. [↑](./Hick's_law#cite_ref-Lawrence2008_7-0) Lawrence, B. M.; St. John, A.; Abrams, R. A.; Snyder, L. H. (2008). ["An anti-Hick's effect in monkey and human saccade reaction times"](https://doi.org/10.1167%2F8.3.26). *Journal of Vision*. **8** (26): 26.1–7. [doi](./Doi_(identifier)):[10.1167/8.3.26](https://doi.org/10.1167%2F8.3.26). [PMID](./PMID_(identifier)) [18484832](https://pubmed.ncbi.nlm.nih.gov/18484832).
8. [↑](./Hick's_law#cite_ref-Stadler1992_8-0) Stadler, M. A. (1992). "Statistical Structure and Implicit Learning Serial". *Journal of Experimental Psychology: Learning, Memory, and Cognition*. **18** (2): 318–327. [doi](./Doi_(identifier)):[10.1037/0278-7393.18.2.318](https://doi.org/10.1037%2F0278-7393.18.2.318).
9. [↑](./Hick's_law#cite_ref-Remillard2001_9-0) Remillard, G.; Clark (2001). "Implicit Learning of First-, second-, and Third-Order Transition Probabilities". *Journal of Experimental Psychology: Learning, Memory, and Cognition*. **27** (2): 483–498. [doi](./Doi_(identifier)):[10.1037/0278-7393.27.2.483](https://doi.org/10.1037%2F0278-7393.27.2.483). [PMID](./PMID_(identifier)) [11294445](https://pubmed.ncbi.nlm.nih.gov/11294445).
10. [↑](./Hick's_law#cite_ref-Jamieson2009_10-0) Jamieson, R. K.; Mewhort (2009). "Applying an exemplary model to the serial reaction-time task: Anticipating from experience". *The Quarterly Journal of Experimental Psychology*. **62** (9): 1757–1783. [doi](./Doi_(identifier)):[10.1080/17470210802557637](https://doi.org/10.1080%2F17470210802557637). [PMID](./PMID_(identifier)) [19219752](https://pubmed.ncbi.nlm.nih.gov/19219752). [S2CID](./S2CID_(identifier)) [24593123](https://api.semanticscholar.org/CorpusID:24593123).
11. [↑](./Hick's_law#cite_ref-Pavão2016_11-0) Pavão, R.; Savietto, J.P.; Sato, J.R.; Xavier, G. F.; Helene, A. F. (2016). ["On Sequence Learning Models: Open-loop Control Not Strictly Guided by Hick's Law"](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4792158). *Scientific Reports*. **6** 23018. [Bibcode](./Bibcode_(identifier)):[2016NatSR...623018P](https://ui.adsabs.harvard.edu/abs/2016NatSR...623018P). [doi](./Doi_(identifier)):[10.1038/srep23018](https://doi.org/10.1038%2Fsrep23018). [PMC](./PMC_(identifier)) [4792158](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4792158). [PMID](./PMID_(identifier)) [26975409](https://pubmed.ncbi.nlm.nih.gov/26975409).
12. [↑](./Hick's_law#cite_ref-12) Landauer, T. K.; Nachbar, D. W. (1985). "Selection from alphabetic and numeric menu trees using a touch screen". *Proceedings of the SIGCHI conference on Human factors in computing systems - CHI '85*. p. 73. [doi](./Doi_(identifier)):[10.1145/317456.317470](https://doi.org/10.1145%2F317456.317470). [ISBN](./ISBN_(identifier)) [978-0-89791-149-8](./Special:BookSources/978-0-89791-149-8). [S2CID](./S2CID_(identifier)) [17669570](https://api.semanticscholar.org/CorpusID:17669570).

 

## References

 
- Cockburn, Andy; Gutwin, Carl; Greenberg, Saul (April 28 – May 3, 2007). ["A predictive model of menu performance"](http://ir.canterbury.ac.nz/bitstream/10092/662/1/12602883_paper191-cockburn.pdf) (PDF). *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*. San Jose, California. pp. 627–636. [doi](./Doi_(identifier)):[10.1145/1240624.1240723](https://doi.org/10.1145%2F1240624.1240723). [hdl](./Hdl_(identifier)):[10092/662](https://hdl.handle.net/10092%2F662). [ISBN](./ISBN_(identifier)) [978-1-59593-593-9](./Special:BookSources/978-1-59593-593-9). [S2CID](./S2CID_(identifier)) [7340315](https://api.semanticscholar.org/CorpusID:7340315).`{{cite book}}`:  CS1 maint: location missing publisher ([link](./Category:CS1_maint:_location_missing_publisher))
- Hick, W. E. (1 March 1952). ["On the rate of gain of information"](http://www2.psychology.uiowa.edu/faculty/mordkoff/InfoProc/pdfs/Hick%201952.pdf) (PDF). *Quarterly Journal of Experimental Psychology*. **4** (1): 11–26. [doi](./Doi_(identifier)):[10.1080/17470215208416600](https://doi.org/10.1080%2F17470215208416600). [S2CID](./S2CID_(identifier)) [39060506](https://api.semanticscholar.org/CorpusID:39060506).
- Hyman, R (March 1953). "Stimulus information as a determinant of reaction time". *Journal of Experimental Psychology*. **45** (3): 188–96. [doi](./Doi_(identifier)):[10.1037/h0056940](https://doi.org/10.1037%2Fh0056940). [PMID](./PMID_(identifier)) [13052851](https://pubmed.ncbi.nlm.nih.gov/13052851). [S2CID](./S2CID_(identifier)) [17559281](https://api.semanticscholar.org/CorpusID:17559281).
- Rosati, L. (October 24–25, 2013). ["How to design interfaces for choice: Hick-Hyman law and classification for information architecture"](https://www.researchgate.net/publication/270890224). In Slavic, A.; Salah, A.; Davies, C. (eds.). *Classification and visualization: interfaces to knowledge: proceedings of the International UDC Seminar*. The Hague, The Netherlands. pp. 125–138.`{{cite book}}`:  CS1 maint: location missing publisher ([link](./Category:CS1_maint:_location_missing_publisher))
- Roy, Q.; Malacria, S.; Lecolinet, E.; Guiard, Y.; Eagan, J. (April 27 – May 2, 2013). ["Augmented letters: Mnemonic gesture-based shortcuts"](http://biblio.telecom-paristech.fr/cgi-bin/download.cgi?id=12999). [*Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*](https://hal.archives-ouvertes.fr/hal-01164207/file/aletters-author-version.pdf) (PDF). Paris, France. pp. 2325–2328. [doi](./Doi_(identifier)):[10.1145/2470654.2481321](https://doi.org/10.1145%2F2470654.2481321). [ISBN](./ISBN_(identifier)) [978-1-4503-1899-0](./Special:BookSources/978-1-4503-1899-0). [S2CID](./S2CID_(identifier)) [15928158](https://api.semanticscholar.org/CorpusID:15928158).`{{cite book}}`:  CS1 maint: location missing publisher ([link](./Category:CS1_maint:_location_missing_publisher))
- Seow, Steven C. (2005). "Information Theoretic Models of HCI: A Comparison of the Hick–Hyman Law and Fitts' Law". *Human-Computer Interaction*. **20** (3): 315–352. [CiteSeerX](./CiteSeerX_(identifier)) [10.1.1.86.4509](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.86.4509). [doi](./Doi_(identifier)):[10.1207/s15327051hci2003_3](https://doi.org/10.1207%2Fs15327051hci2003_3). [S2CID](./S2CID_(identifier)) [14436546](https://api.semanticscholar.org/CorpusID:14436546).
- Welford, Alan T. (1968). *Fundamentals of Skill*. Methuen, Massachusetts. pp. 61–65.`{{cite book}}`:  CS1 maint: location missing publisher ([link](./Category:CS1_maint:_location_missing_publisher))

 

## External links

 
- [Usability Glossary: Hick's Law](http://www.usabilityfirst.com/glossary/hicks-law/)