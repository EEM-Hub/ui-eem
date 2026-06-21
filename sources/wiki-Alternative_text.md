---
source: https://en.wikipedia.org/wiki/Alternative_text
fetched: 2026-06-20
---

Alternative text that appears when a HTML element cannot be rendered  For the use of alt attributes in Wikipedia, see [Wikipedia:Alternative text for images](./Wikipedia:Alternative_text_for_images). 

 

 
| HTML |
| --- |
|  |
| HTML and variants |
| Dynamic HTMLHTML5XHTMLBasicMobile Profile |
| HTML elements and attributes |
| HTML elementarticleaudioblinkcanvasdiv and spanmarqueemetavideoHTML attributealt attributeHTML frame |
| Editing |
| HTML editorText editor |
| Character encodings and language |
| Character encodingsCharacter entity references (named characters)UnicodeLanguage code |
| Document and browser models |
| Document Object ModelBrowser Object ModelStyle sheetsCSSFont familyWeb colors |
| Client-side scripting and APIs |
| JavaScriptWebCLHTMX |
| Graphics and Web3D technology |
| Web3DWebGLWebGPUWebXRW3CValidatorWHATWGQuirks modeWeb storageRendering engine |
| Comparisons |
| Document markup languagesComparison of browser engines |
| vte |

 

The **alt attribute** is the [HTML attribute](./HTML_attribute) used in [HTML](./HTML) and [XHTML](./XHTML) documents to specify alternative [text](./Plain_text) (**alt text**) that is to be displayed in place of an [element](./HTML_element) that cannot be rendered. The alt attribute is used for short descriptions, with longer descriptions using the [longdesc attribute](./Longdesc_attribute). The standards organization for the [World Wide Web](./World_Wide_Web), the [World Wide Web Consortium](./World_Wide_Web_Consortium) (W3C), recommends that every image displayed through HTML have an alt attribute, though the alt attribute does not need to contain text. The lack of proper alt attributes on website images has led to several accessibility-related lawsuits.

 

The alt attribute is used to increase accessibility and user friendliness, including for blind internet users who rely on special software for web browsing. The use of the alt attribute for images displayed within HTML is part of W3C's [Web Content Accessibility Guidelines](./Web_Content_Accessibility_Guidelines) (WCAG). [Screen readers](./Screen_reader) and [text-based web browsers](./Text-based_web_browser) read the alt attribute in place of the image. The text within the alt attribute substitutes the image when [copy-pasted](./Copy-paste) as text and makes images more [machine-readable](./Machine-readable_data), which improves [search engine optimization](./Search_engine_optimization) (SEO).

 

## History

 

The attribute was first introduced in the HTML 1.2 draft in 1993 to provide support for text-based browsers.[[1]](./Alt_attribute#cite_note-ietfiiir-1) In [HTML 4.01](./HTML_4.01), which was released in 1999, the attribute was made to be a requirement for the img and area [tags](./HTML_tag).[[2]](./Alt_attribute#cite_note-w3c1999-2) It is optional for the input tag and the deprecated [applet](./Applet) tag.[[3]](./Alt_attribute#cite_note-hazaël-massieux-3)

 

[Internet Explorer 7](./Internet_Explorer_7) and earlier render text in alt attributes as [tooltip](./Tooltip) text, which is not compliant with the [World Wide Web Consortium](./World_Wide_Web_Consortium) (W3C)'s HTML standards.[[4]](./Alt_attribute#cite_note-moz-4) This behavior led many [web developers](./Web_developer) to misuse the alt attribute when they wished to display tooltips containing additional information about images, instead of using the title attribute that was intended for that use.[[5]](./Alt_attribute#cite_note-flavell-5)[[6]](./Alt_attribute#cite_note-6) As of [Internet Explorer 8](./Internet_Explorer_8), released in 2009, alt attributes no longer render as tooltips on Internet Explorer.[[7]](./Alt_attribute#cite_note-7)

 

## Usage

 [![Example image of what displays when the alt text is shown](//upload.wikimedia.org/wikipedia/commons/thumb/0/03/Alt_attribute_example.png/250px-Alt_attribute_example.png)](./File:Alt_attribute_example.png)An example of alt attribute text being displayed in place of an unavailable image, with the underlying HTML displayed below it [![A screenshot of a Wikipedia article using alt text in the Lynx browser](//upload.wikimedia.org/wikipedia/commons/thumb/c/c2/Wikipedia_Wolf_article_displayed_on_Lynx.png/250px-Wikipedia_Wolf_article_displayed_on_Lynx.png)](./File:Wikipedia_Wolf_article_displayed_on_Lynx.png)The [Wikipedia article for Wolf](./Wolf) on the [Lynx web browser](./Lynx_(web_browser)), displaying the text of the alt attribute in orange in place of the images 

The text in the alt attribute is used to replace the image when the image cannot be loaded, without changing the intended meaning of the page's contents.[[8]](./Alt_attribute#cite_note-mozilladev-8) The W3C's web content accessibility guidelines state that the alt attribute is used to convey the meaning and intent of the image, rather than being a literal description of the image itself.[[9]](./Alt_attribute#cite_note-wcag_h37-9) For example, an alt attribute for an image of an institution's logo should convey that it is the institution's logo rather than describing details of what the logo looks like.[[10]](./Alt_attribute#cite_note-sc_logo-10)[[11]](./Alt_attribute#cite_note-11) The alt attribute is intended to be used for short and concise descriptions of the image. Longer descriptions can be given using the longdesc attribute, which provides more detailed information and complements but does not replace the alt attribute.[[2]](./Alt_attribute#cite_note-w3c1999-2)

 

A screen reader such as [Orca](./Orca_(assistive_technology)) will read out the alt text in place of the image.[[12]](./Alt_attribute#cite_note-hofmann-12) A text-based web browser such as [Lynx](./Lynx_(web_browser)) will display the alt text instead of the image (or will display the value attribute if the image is a [clickable button](./Button_(computing))).[[13]](./Alt_attribute#cite_note-lynxman-13) A graphical browser typically will display only the image, and will display the alt text only if the user views the image's properties, or has configured the browser not to display images, or if the browser was unable to retrieve or to decode the image.[[14]](./Alt_attribute#cite_note-pennstate-14)

 

The use of descriptions in the alt attribute improves search engine optimization and allows image-specific search engines, such as [Google Images](./Google_Images), to search for and display relevant images that are used on websites in search results.[[15]](./Alt_attribute#cite_note-googledev-15) For non-image search results, the text within the alt attribute is read by search engines the same way that regular text on the page is read.[[16]](./Alt_attribute#cite_note-southern-16)

 

The W3C recommends that images that convey no information, but are purely decorative, be specified in [CSS](./CSS) rather than in the HTML markup. If decorative images are rendered using HTML that do not add to the content and provide no additional information, then the W3C recommends that a blank alt attribute be included in the form of `alt=""`.[[17]](./Alt_attribute#cite_note-w3c-17) This makes the page more navigable for users of screen readers or non-graphical browsers by skipping over images that do not convey any meaning. If no alt attribute has been supplied, then browsers that cannot display the image will not overlook the image but instead will read or display the URL or another identifying marker.[[18]](./Alt_attribute#cite_note-solovieva-18) This creates ambiguity since the user is generally unable to determine from a bare reading of a URL if the image is relevant to the text or if it is a purely decorative element of the webpage.[[19]](./Alt_attribute#cite_note-curl-19) A 2021 [Google Lighthouse](./Google_Lighthouse) audit showed that 27% of alt text attributes audited were empty, despite the fact that the majority of those images were non-decorative informational images.[[20]](./Alt_attribute#cite_note-almanac-20)

 

## Lawsuits

 

There have been many lawsuits over website accessibility and the lack of proper alt attributes on websites.[[18]](./Alt_attribute#cite_note-solovieva-18) *[Maguire v Sydney Organising Committee for the Olympic Games](./Maguire_v_Sydney_Organising_Committee_for_the_Olympic_Games_(2000))* was a 2000 lawsuit in which a blind man in Australia sued the [Sydney Organising Committee for the Olympic Games](./Sydney_Organising_Committee_for_the_Olympic_Games) because their website www.olympics.com was not accessible to him because of the lack of alt attributes on images.[[21]](./Alt_attribute#cite_note-white-21) The [Australian Human Rights Commission](./Australian_Human_Rights_Commission) ruled that the website had discriminated against him for failing to conform to accessibility standards that enable blind individuals to navigate websites.[[22]](./Alt_attribute#cite_note-barkham-22) During the lawsuit, the Australian commonwealth, state and territory governments issued a joint statement through the [Department of Broadband, Communications and the Digital Economy](./Department_of_Broadband,_Communications_and_the_Digital_Economy) that they were adopting the W3C's accessibility guidelines for all .gov.au websites.[[23]](./Alt_attribute#cite_note-dbcde-23)

 

In the United States, there have been several high-profile lawsuits involving the lack of alt attributes on images that cite a violation of the [Americans with Disabilities Act](./Americans_with_Disabilities_Act) (ADA).[[24]](./Alt_attribute#cite_note-cohen-24) The [United States Department of Justice](./United_States_Department_of_Justice) gives the lack of alt attributes as an example of a barrier to website accessibility.[[25]](./Alt_attribute#cite_note-ada.gov-25) *[National Federation of the Blind v. Target Corp.](./National_Federation_of_the_Blind_v._Target_Corp.)* was a 2006 class-action lawsuit that alleged that [Target.com](./Target.com) violated the ADA because the images did not use alt attributes.[[26]](./Alt_attribute#cite_note-daniels-26) This lawsuit set a legal precedent in the United States for website accessibility and compliance with the ADA.[[27]](./Alt_attribute#cite_note-frank-27)

 

## References

  
1. [↑](./Alt_attribute#cite_ref-ietfiiir_1-0) [Berners-Lee, Tim](./Tim_Berners-Lee); [Connolly, Daniel](./Dan_Connolly_(computer_scientist)) (June 1993). ["Hypertext Markup Language (HTML) Internet Draft version 1.2"](https://www.w3.org/MarkUp/draft-ietf-iiir-html-01.txt). IETF IIIR Working Group. [Archived](https://web.archive.org/web/20170103041713/https://www.w3.org/MarkUp/draft-ietf-iiir-html-01.txt) from the original on 3 January 2017. Retrieved 18 September 2010.
2. [1](./Alt_attribute#cite_ref-w3c1999_2-0) [2](./Alt_attribute#cite_ref-w3c1999_2-1) ["13 Objects, Images, and Applets"](http://www.w3.org/TR/html401/struct/objects.html#adef-alt). [World Wide Web Consortium](./World_Wide_Web_Consortium). 24 December 1999. [Archived](https://web.archive.org/web/20080906001213/http://www.w3.org/TR/html401/struct/objects.html#adef-alt) from the original on 6 September 2008. Retrieved 4 December 2005.
3. [↑](./Alt_attribute#cite_ref-hazaël-massieux_3-0) Hazaël-Massieux, Dominique (20 November 2002). ["Use the alt attribute to describe the function of each visual"](https://www.w3.org/QA/Tips/altAttribute). *[World Wide Web Consortium](./World_Wide_Web_Consortium)*. [Archived](https://web.archive.org/web/20220320214305/https://www.w3.org/QA/Tips/altAttribute) from the original on 20 March 2022. Retrieved 14 October 2022.
4. [↑](./Alt_attribute#cite_ref-moz_4-0) ["Why does not Mozilla display my alt tooltips?"](https://web.archive.org/web/20081015232141/http://developer.mozilla.org/en/Mozilla_Web_Developer_FAQ#Why_doesn.E2.80.99t_Mozilla_display_my_alt_tooltips.3F). *[MDN Web Docs](./MDN_Web_Docs)*. Archived from [the original](https://developer.mozilla.org/en/Mozilla_Web_Developer_FAQ#Why_doesn.E2.80.99t_Mozilla_display_my_alt_tooltips.3F) on 15 October 2008. Retrieved 22 July 2009.
5. [↑](./Alt_attribute#cite_ref-flavell_5-0) Flavell, A.J. ["Use of ALT texts in IMGs"](https://www.htmlhelp.com/feature/art3.htm). *www.htmlhelp.com*. [Archived](https://web.archive.org/web/20220108230541/https://www.htmlhelp.com/feature/art3.htm) from the original on 8 January 2022. Retrieved 16 October 2022.
6. [↑](./Alt_attribute#cite_ref-6) W3C HTML WG (24 December 1999). ["7.4.3 The title attribute"](http://www.w3.org/TR/html4/struct/global.html#h-7.4.3). *HTML 4.01 Specification*. W3C. [Archived](https://web.archive.org/web/20090726044334/http://www.w3.org/TR/html4/struct/global.html#h-7.4.3) from the original on 26 July 2009. Retrieved 22 July 2009.
7. [↑](./Alt_attribute#cite_ref-7) ["What's New in Internet Explorer 8 – Accessibility and ARIA"](http://msdn.microsoft.com/en-us/library/cc288472.aspx#access). *MSDN*. Microsoft. [Archived](https://web.archive.org/web/20090228115639/http://msdn.microsoft.com/en-us/library/cc288472.aspx) from the original on 28 February 2009. Retrieved 22 July 2009.
8. [↑](./Alt_attribute#cite_ref-mozilladev_8-0) ["HTMLImageElement.alt"](https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/alt). *[Mozilla](./Mozilla)*. [Archived](https://web.archive.org/web/20220822212522/https://developer.mozilla.org/en-US/docs/Web/API/HTMLImageElement/alt) from the original on 22 August 2022. Retrieved 14 October 2022.
9. [↑](./Alt_attribute#cite_ref-wcag_h37_9-0) ["Using alt attributes on img elements"](https://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/H37). *[World Wide Web Consortium](./World_Wide_Web_Consortium)*. [Archived](https://web.archive.org/web/20220516223146/https://www.w3.org/TR/2016/NOTE-WCAG20-TECHS-20161007/H37) from the original on 16 May 2022. Retrieved 13 October 2022.
10. [↑](./Alt_attribute#cite_ref-sc_logo_10-0) ["Logo Alt Text"](https://sc.edu/about/offices_and_divisions/digital-accessibility/guides_tutorials/alternative_text/logo-alt-text/index.php). *[University of South Carolina](./University_of_South_Carolina)*. [Archived](https://web.archive.org/web/20220722213601/https://sc.edu/about/offices_and_divisions/digital-accessibility/guides_tutorials/alternative_text/logo-alt-text/index.php) from the original on 22 July 2022. Retrieved 15 October 2022.
11. [↑](./Alt_attribute#cite_ref-11) Montti, Roger (1 November 2022). ["Google Explains Alt Text for Logos & Buttons"](https://www.searchenginejournal.com/alt-text-for-logos-and-buttons/469801/). *Search Engine Journal*. [Archived](https://web.archive.org/web/20221103152738/https://www.searchenginejournal.com/alt-text-for-logos-and-buttons/469801/) from the original on 3 November 2022. Retrieved 3 November 2022.
12. [↑](./Alt_attribute#cite_ref-hofmann_12-0) Hofmann, Frank; Beckert, Axel (2021). ["Text Art: Rendering images as text"](https://www.linux-magazine.com/Online/Features/Converting-Images-to-Text/(offset)/3). *[Linux Magazine](./Linux_Magazine)*. [Archived](https://web.archive.org/web/20221015064058/https://www.linux-magazine.com/Online/Features/Converting-Images-to-Text/%28offset%29/3) from the original on 15 October 2022. Retrieved 14 October 2022.
13. [↑](./Alt_attribute#cite_ref-lynxman_13-0) ["Lynx Users Guide v2.8.9"](https://lynx.invisible-island.net/lynx_help/Lynx_users_guide.html). *lynx.invisible-island.net*. [Archived](https://web.archive.org/web/20190204065859/https://lynx.invisible-island.net/lynx_help/Lynx_users_guide.html) from the original on 4 February 2019. Retrieved 15 October 2022.
14. [↑](./Alt_attribute#cite_ref-pennstate_14-0) ["Image ALT Text"](https://accessibility.psu.edu/images/alttext/). *[Pennsylvania State University](./Pennsylvania_State_University)*. 6 October 2014. [Archived](https://web.archive.org/web/20221012021810/https://accessibility.psu.edu/images/alttext/) from the original on 12 October 2022. Retrieved 14 October 2022.
15. [↑](./Alt_attribute#cite_ref-googledev_15-0) ["Google Images best practices"](https://developers.google.com/search/docs/appearance/google-images). *[Google Developers](./Google_Developers)*. 20 September 2022. [Archived](https://web.archive.org/web/20221014094659/https://developers.google.com/search/docs/appearance/google-images) from the original on 14 October 2022. Retrieved 14 October 2022.
16. [↑](./Alt_attribute#cite_ref-southern_16-0) Southern, Matt G. (22 March 2022). ["Google: Alt Text Only A Factor For Image Search"](https://www.searchenginejournal.com/google-alt-text-only-a-factor-for-image-search/442865/#close). *Search Engine Journal*. [Archived](https://web.archive.org/web/20220422141742/https://www.searchenginejournal.com/google-alt-text-only-a-factor-for-image-search/442865/#close) from the original on 22 April 2022. Retrieved 14 October 2022.
17. [↑](./Alt_attribute#cite_ref-w3c_17-0) ["Embedded content – HTML 5"](http://www.w3.org/TR/html5/embedded-content-0.html#a-purely-decorative-image-that-does%20not-add-any-information). *W3C*. [Archived](https://web.archive.org/web/20170702051717/http://www.w3.org/TR/html5/embedded-content-0.html#a-purely-decorative-image-that-does%20not-add-any-information) from the original on 2 July 2017. Retrieved 29 June 2017.
18. [1](./Alt_attribute#cite_ref-solovieva_18-0) [2](./Alt_attribute#cite_ref-solovieva_18-1) Solovieva, Tatiana I.; Bock, Jeremy M. (2014). ["Monitoring for Accessibility and University Websites: Meeting the Needs of People with Disabilities"](https://eric.ed.gov/?id=EJ1040525). *Journal of Postsecondary Education and Disability*. **27** (2): 113–127. [Archived](https://web.archive.org/web/20221014232614/https://eric.ed.gov/?id=EJ1040525) from the original on 14 October 2022. Retrieved 14 October 2022 – via [Education Resources Information Center](./Education_Resources_Information_Center).
19. [↑](./Alt_attribute#cite_ref-curl_19-0) Curl, Angela L.; Bowers, Deborah D. (23 April 2009). ["A Longitudinal Study of Website Accessibility: Have Social Work Education Websites Become More Accessible?"](http://www.tandfonline.com/doi/abs/10.1080/15228830902749229). *Journal of Technology in Human Services*. **27** (2): 93–105. [doi](./Doi_(identifier)):[10.1080/15228830902749229](https://doi.org/10.1080%2F15228830902749229). [hdl](./Hdl_(identifier)):[2374.MIA/5279](https://hdl.handle.net/2374.MIA%2F5279). [S2CID](./S2CID_(identifier)) [143667951](https://api.semanticscholar.org/CorpusID:143667951). [Archived](https://web.archive.org/web/20221014232615/https://www.tandfonline.com/doi/abs/10.1080/15228830902749229) from the original on 14 October 2022. Retrieved 14 October 2022.
20. [↑](./Alt_attribute#cite_ref-almanac_20-0) Tait, Alex; Davis, Scott; Niyi-Awosusi, Olu; Wilhelm, Gary; Dixon, Carlie (30 November 2021). ["Part II Chapter 9 – Accessibility"](https://almanac.httparchive.org/en/2021/accessibility). *Web Almanac by HTTParchive.org*. Retrieved 14 October 2022.
21. [↑](./Alt_attribute#cite_ref-white_21-0) White, Caroline (2 November 2000). ["Battle to be equal"](https://www.newspapers.com/clip/111280702/battle-to-be-equal/). *[The Guardian](./The_Guardian)*. [Archived](https://web.archive.org/web/20221014084006/https://www.newspapers.com/clip/111280702/battle-to-be-equal/) from the original on 14 October 2022. Retrieved 14 October 2022 – via [Newspapers.com](./Newspapers.com).
22. [↑](./Alt_attribute#cite_ref-barkham_22-0) Barkham, Patrick (30 August 2000). ["Website 'discriminated against blind'"](https://www.theguardian.com/technology/2000/aug/30/internetnews.sydney). *[The Guardian](./The_Guardian)*. [Archived](https://web.archive.org/web/20160823132558/https://www.theguardian.com/technology/2000/aug/30/internetnews.sydney) from the original on 23 August 2016. Retrieved 14 October 2022.
23. [↑](./Alt_attribute#cite_ref-dbcde_23-0) ["Seventh Ministerial meeting of the Online Council – Media release"](https://web.archive.org/web/20130620081938/http://www.dbcde.gov.au/Article/0,,0_4-2_4008-4_15092,00.html). *[Australian Department of Broadband, Communications and the Digital Economy](./Department_of_Broadband,_Communications_and_the_Digital_Economy)*. 30 June 2000. Archived from [the original](http://www.dbcde.gov.au/Article/0,,0_4-2_4008-4_15092,00.html) on 20 June 2013. Retrieved 14 October 2022.
24. [↑](./Alt_attribute#cite_ref-cohen_24-0) Cohen, Alex H.; Fresneda, Jorge E.; Anderson, Rolph E. (September 2020). ["What retailers need to understand about website inaccessibility and disabled consumers: Challenges and opportunities"](https://onlinelibrary.wiley.com/doi/10.1111/joca.12307). *Journal of Consumer Affairs*. **54** (3): 854–889. [doi](./Doi_(identifier)):[10.1111/joca.12307](https://doi.org/10.1111%2Fjoca.12307). [ISSN](./ISSN_(identifier)) [0022-0078](https://search.worldcat.org/issn/0022-0078). [S2CID](./S2CID_(identifier)) [225771708](https://api.semanticscholar.org/CorpusID:225771708).
25. [↑](./Alt_attribute#cite_ref-ada.gov_25-0) ["Guidance on Web Accessibility and the ADA"](https://beta.ada.gov/resources/web-guidance/). *ADA.gov*. 18 March 2022. [Archived](https://web.archive.org/web/20221013080830/https://beta.ada.gov/resources/web-guidance/) from the original on 13 October 2022. Retrieved 14 October 2022.
26. [↑](./Alt_attribute#cite_ref-daniels_26-0) Daniels, Linda Markus (13 September 2006). ["Websites for the Blind: Is This The Next 'Year 2000 Compliant' Requirement?"](https://web.archive.org/web/20080916100355/http://localtechwire.com/business/local_tech_wire/biotech/story/1167848/). [WRAL-TV](./WRAL-TV). Archived from [the original](http://localtechwire.com/business/local_tech_wire/biotech/story/1167848/) on 16 September 2008. Retrieved 14 October 2022.
27. [↑](./Alt_attribute#cite_ref-frank_27-0) Frank, Jonathan (January 2008). "Web Accessibility for the Blind: Corporate Social Responsibility or Litigation Avoidance?". *Proceedings of the 41st Annual Hawaii International Conference on System Sciences (HICSS 2008)*. Waikoloa, HI: IEEE. p. 284. [doi](./Doi_(identifier)):[10.1109/HICSS.2008.497](https://doi.org/10.1109%2FHICSS.2008.497). [S2CID](./S2CID_(identifier)) [16280255](https://api.semanticscholar.org/CorpusID:16280255).

 

## External links

 
- [Appropriate Use of Alternative Text](http://webaim.org/techniques/alttext/) from WebAIM
- [Mini-FAQ about the alternate text of images](http://www.hixie.ch/advocacy/alttext) by [Ian Hickson](./Ian_Hickson)