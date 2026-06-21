---
source: https://en.wikipedia.org/wiki/WAI-ARIA
fetched: 2026-06-20
---

Technical specification for web accessibility 
| WAI-ARIA |
| --- |
| Web Accessibility Initiative - Accessible Rich Internet Applications |
| Abbreviation | WAI-ARIA |
| Status | W3C Recommendation |
| Year started | 2006;20years ago(2006) |
| First published | September26, 2006;19 years ago(2006-09-26) |
| Latest version | WAI-ARIA 1.2:W3C RecommendationJune6, 2023;3 years ago(2023-06-06) |
| Organization | W3CAdobeAppleIBMIgaliaKnowbilitySpec-Ops |
| Committee | ARIA WG |
| Editors | Joanmarie DiggsJames NurthenMichael CooperCarolyn MacLeodFormer editorsShane McCarron (until 2018(2018))Richard Schwerdtfeger (until October2017(2017-10))James Craig (Editor until May2016(2016-05)) |
| Domain | Assistive technologyProgressive web applicationsSemantic HTMLWeb accessibility |
| Website | www.w3.org/WAI/standards-guidelines/aria/ |

 

**Web Accessibility Initiative – Accessible Rich Internet Applications** (**WAI-ARIA**) is a [technical specification](./Specification_(technical_standard)) published by the [World Wide Web Consortium](./World_Wide_Web_Consortium) (W3C) that specifies how to increase the [accessibility](./Accessibility) of [web pages](./Web_page), in particular, [dynamic content](./Dynamic_web_page), and [user interface](./User_interface) components developed with [Ajax](./Ajax_(programming)), [HTML](./HTML), [JavaScript](./JavaScript), and related technologies.

 

In the 15 September 2008 working draft, [SVG](./Scalable_Vector_Graphics) 1.2 Tiny added support for WAI-ARIA.[[1]](./WAI-ARIA#cite_note-1) On 20 March 2014, WAI-ARIA 1.0 became a completed W3C Recommendation.[[2]](./WAI-ARIA#cite_note-2) 14 December 2017 saw the release of WAI-ARIA 1.1.[[3]](./WAI-ARIA#cite_note-3)

 

## The 5 Rules of ARIA

 
1. Don’t use ARIA if you can achieve the same semantics with a native HTML element or attribute[[4]](./WAI-ARIA#cite_note-4)
2. Do not change the semantics of native HTML (unless you really have to)[[5]](./WAI-ARIA#cite_note-5)
3. All interactive ARIA controls must be usable with the keyboard.[[6]](./WAI-ARIA#cite_note-6)
4. Do not remove semantics or hide focusable elements (using  role="presentation" or aria-hidden="true" on a focusable element)[[7]](./WAI-ARIA#cite_note-7)
5. Ensure all interactive elements have an accessible name (Accessibility API accessible name).[[8]](./WAI-ARIA#cite_note-8)

 

## Scope

 

Web developers increasingly use [client-side](./Client-side) scripts to create user interface controls that cannot be created with HTML alone. They also use client-side scripts to update sections of a page without requesting a completely new page from a [web server](./Web_server). Such techniques on websites are called [rich Internet applications](./Rich_Internet_applications). These user interface controls and content updates are often not accessible to users with [disabilities](./Disabilities), especially [screen reader](./Screen_reader) users and users who cannot use a [mouse](./Mouse_(computing)) or other [pointing device](./Pointing_device). WAI-ARIA allows [web pages](./Web_page) (or portions of pages) to declare themselves as [applications](./Application_software) rather than as [static documents](./Static_web_page), by adding role, property, and state information to dynamic web applications. ARIA is intended for use by developers of [web applications](./Web_application), [web browsers](./Web_browser), [assistive technologies](./Assistive_technology), and accessibility evaluation tools.[[9]](./WAI-ARIA#cite_note-wai-aria-overview-9)

 

WAI-ARIA describes how to add [semantics](./Semantics) and other [metadata](./Metadata) to HTML content in order to make user interface controls and dynamic content more accessible. For example, with WAI-ARIA it is possible to identify a list of [links](./Hyperlink) as a navigation [menu](./Menu_(computing)) and to state whether it is expanded or collapsed. Although originally developed to address accessibility issues in HTML, the use of WAI-ARIA is not limited to HTML: in principle, it can also be used in other [markup languages](./Markup_languages) such as Scalable Vector Graphics (SVG).[[10]](./WAI-ARIA#cite_note-ariasvg2008-10)[[11]](./WAI-ARIA#cite_note-11)

 

## Documents

 

The [Web Accessibility Initiative](./Web_Accessibility_Initiative) has published an overview of WAI-ARIA that introduces the subject and guides readers to the WAI-ARIA Suite documents:[[9]](./WAI-ARIA#cite_note-wai-aria-overview-9)

 Accessible Rich Internet Applications (WAI-ARIA) Version 1.0 This is primarily aimed at developers of [Web browsers](./Web_browsers), [assistive technologies](./Assistive_technology), and other [user agents](./User_agents), in addition to developers of other [technical specifications](./Technical_specifications), and developers of accessibility evaluation tools. The WAI-ARIA has been marked as completed on 20 March 2014 and is therefore a [W3C recommendation](./W3C_recommendation).[[12]](./WAI-ARIA#cite_note-w3.org-12) WAI-ARIA Overview This is a technical introduction to WAI-ARIA. It describes the problems WAI-ARIA tries to address, the underlying concepts, the technical approach and business reasons for adopting WAI-ARIA.[[9]](./WAI-ARIA#cite_note-wai-aria-overview-9) WAI-ARIA Authoring Practices This document describes best practices for delivering rich Internet applications with WAI-ARIA: it discusses subjects such as general steps for building accessible [widgets](./GUI_widget), keyboard navigation, relationships, [form](./Form_(web)) properties, [drag-and-drop](./Drag-and-drop) support, [alert](./Alert_dialog_box) and [dialog boxes](./Dialog_boxes), [reusable component](./Reusable_software_component) libraries, and [testing](./Software_testing).[[13]](./WAI-ARIA#cite_note-wai-aria-bp-13) Roadmap for Accessible Rich Internet Applications (WAI-ARIA Roadmap) Much of the content of this document has been moved into other documents.[[14]](./WAI-ARIA#cite_note-ariaroadmap-14) 

The ARIA specifications editors have included [Lisa Seeman](./Lisa_Seeman), [Rich Schwerdtfeger](./Rich_Schwerdtfeger?action=edit&redlink=1), James Craig, Michael Cooper, and Lisa Pappas.[[12]](./WAI-ARIA#cite_note-w3.org-12)

 

## See also

 
- [Accessibility](./Accessibility) and [Web accessibility](./Web_accessibility)
- [Ajax](./Ajax_(programming))
- [Rich Internet application](./Rich_Internet_application)
- [Universal design](./Universal_design)

 

## References

  
1. [↑](./WAI-ARIA#cite_ref-1) ["Scalable Vector Graphics (SVG) Tiny 1.2 Specification"](https://www.w3.org/TR/2008/WD-SVGMobile12-20080915/Overview.html). *www.w3.org*. Retrieved 2023-05-09.
2. [↑](./WAI-ARIA#cite_ref-2) ["Accessible Rich Internet Applications (WAI-ARIA) 1.0"](https://www.w3.org/TR/2014/REC-wai-aria-20140320/Overview.html). *www.w3.org*. Retrieved 2023-05-09.
3. [↑](./WAI-ARIA#cite_ref-3) ["Accessible Rich Internet Applications (WAI-ARIA) 1.1"](https://www.w3.org/TR/wai-aria-1.1/). *www.w3.org*. Retrieved 2023-05-09.
4. [↑](./WAI-ARIA#cite_ref-4) ["ARIA and HTML"](https://web.dev/learn/accessibility/aria-html/). *web.dev*. Retrieved 2023-05-09.
5. [↑](./WAI-ARIA#cite_ref-5) ["5 Rules of ARIA"](https://dev.to/konrud/5-rules-of-aria-40i). *DEV Community*. 25 February 2023. Retrieved 2023-05-09.
6. [↑](./WAI-ARIA#cite_ref-6) ["StackPath"](https://www.deque.com/blog/top-5-rules-of-aria/#crayon-6459211377b9f899714671). *www.deque.com*. 16 July 2019. Retrieved 2023-05-09.
7. [↑](./WAI-ARIA#cite_ref-7) ["WebAIM: Introduction to ARIA - Accessible Rich Internet Applications"](https://webaim.org/techniques/aria/). *webaim.org*. Retrieved 2023-05-09.
8. [↑](./WAI-ARIA#cite_ref-8) ["Using ARIA"](https://www.w3.org/TR/using-aria/Overview.html). *www.w3.org*. Retrieved 2023-05-09.
9. [1](./WAI-ARIA#cite_ref-wai-aria-overview_9-0) [2](./WAI-ARIA#cite_ref-wai-aria-overview_9-1) [3](./WAI-ARIA#cite_ref-wai-aria-overview_9-2) Cooper, Michael, ed. (2011-01-18). ["WAI-ARIA Overview"](https://www.w3.org/WAI/standards-guidelines/aria/). Accessible Rich Internet Applications Working Group, Education and Outreach Working Group. W3C (published December 2006). Retrieved 2021-04-21.
10. [↑](./WAI-ARIA#cite_ref-ariasvg2008_10-0) SVG Working Group (2008-12-22). ["Document Structure – SVG Tiny 1.2 § 5.10.1 Attributes common to all elements"](https://www.w3.org/TR/SVGMobile12/struct.html#RoleAttribute). *W3C*. Retrieved 2021-04-21.
11. [↑](./WAI-ARIA#cite_ref-11) SVG Working Group (2008-12-22). ["Document Structure – SVG Tiny 1.2 § 18.3 Extensible metadata attributes"](https://www.w3.org/TR/SVGMobile12/metadata.html#MetadataAttributes). *W3C*. Retrieved 2021-04-21..
12. [1](./WAI-ARIA#cite_ref-w3.org_12-0) [2](./WAI-ARIA#cite_ref-w3.org_12-1) ["Accessible Rich Internet Applications (WAI-ARIA) 1.0"](https://www.w3.org/TR/wai-aria/). W3.org. Retrieved 2014-04-11.
13. [↑](./WAI-ARIA#cite_ref-wai-aria-bp_13-0) King, Matt; Ku, JaEun Jemma; Nurthen, James; Bijl, Zoë; Cooper, Michael; Scheuhammer, Joseph; Pappas, Lisa; Schwerdtfeger, Rich, eds. (2019-08-14). ["WAI-ARIA Authoring Practices 1.1"](https://www.w3.org/TR/wai-aria-practices/). Accessible Rich Internet Applications Working Group. Retrieved 2021-04-09.
14. [↑](./WAI-ARIA#cite_ref-ariaroadmap_14-0) Schwerdtfeger, Richard, ed. (2008-02-04). ["Roadmap for Accessible Rich Internet Applications (WAI-ARIA Roadmap)"](https://www.w3.org/TR/wai-aria-roadmap/). *W3C*. Protocols & Formats Working Group. Retrieved 2012-12-06.

 

## External links

 
- [ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA) – [MDN Web Docs](./MDN_Web_Docs)

 
| vteWorld Wide Web Consortium(W3C) |
| --- |
| Products,standards | RecommendationsActivityPubActivity StreamsARIACanonical XMLCDFCSSAnimationsFlexboxGridDOMEXIEmotionMLGeolocation APIGRDDLHTMLHTML5IndexedDBITSJSON-LDLinked Data NotificationsMathMLMicropubMTOMOWLPLSRDFSchemaRDFaRIFSAWSDLSISRSKOSSMILSOAPSRGSSRISSMLSVGAnimationFilter EffectsSCXMLSHACLSPARQLTimed textVoiceXMLWebAssemblyWoTTDWeb storageWSDLWebmentionWebSubWebVTTWOFFWS-AddressingXHTML+RDFaXMLBaseEncryptionEventsInformation SetNamespaceSchemaSignatureXFormsXIncludeXLinkXOPXPath2.03.xXPointerXProcXQueryXSLXSL-FOXSLTelementsNotesIndieAuthXAdESXBLXHTML+SMILXUPWorking draftsCCXMLCURIEEMEInkMLMSESMIL TimesheetssXBLWebGPUWebXRXFDLXFramesXMLHttpRequestGuidelinesWeb Content Accessibility GuidelinesInitiativeMarkup Validation ServiceWeb Accessibility InitiativeWeb ComponentsDeprecatedC-HTMLHDMLJSSSPGMLVMLWebPlatformObsoletedP3PXHTML+MathML+SVG | Recommendations | ActivityPubActivity StreamsARIACanonical XMLCDFCSSAnimationsFlexboxGridDOMEXIEmotionMLGeolocation APIGRDDLHTMLHTML5IndexedDBITSJSON-LDLinked Data NotificationsMathMLMicropubMTOMOWLPLSRDFSchemaRDFaRIFSAWSDLSISRSKOSSMILSOAPSRGSSRISSMLSVGAnimationFilter EffectsSCXMLSHACLSPARQLTimed textVoiceXMLWebAssemblyWoTTDWeb storageWSDLWebmentionWebSubWebVTTWOFFWS-AddressingXHTML+RDFaXMLBaseEncryptionEventsInformation SetNamespaceSchemaSignatureXFormsXIncludeXLinkXOPXPath2.03.xXPointerXProcXQueryXSLXSL-FOXSLTelements | Notes | IndieAuthXAdESXBLXHTML+SMILXUP | Working drafts | CCXMLCURIEEMEInkMLMSESMIL TimesheetssXBLWebGPUWebXRXFDLXFramesXMLHttpRequest | Guidelines | Web Content Accessibility Guidelines | Initiative | Markup Validation ServiceWeb Accessibility InitiativeWeb Components | Deprecated | C-HTMLHDMLJSSSPGMLVMLWebPlatform | Obsoleted | P3PXHTML+MathML+SVG |
| Recommendations | ActivityPubActivity StreamsARIACanonical XMLCDFCSSAnimationsFlexboxGridDOMEXIEmotionMLGeolocation APIGRDDLHTMLHTML5IndexedDBITSJSON-LDLinked Data NotificationsMathMLMicropubMTOMOWLPLSRDFSchemaRDFaRIFSAWSDLSISRSKOSSMILSOAPSRGSSRISSMLSVGAnimationFilter EffectsSCXMLSHACLSPARQLTimed textVoiceXMLWebAssemblyWoTTDWeb storageWSDLWebmentionWebSubWebVTTWOFFWS-AddressingXHTML+RDFaXMLBaseEncryptionEventsInformation SetNamespaceSchemaSignatureXFormsXIncludeXLinkXOPXPath2.03.xXPointerXProcXQueryXSLXSL-FOXSLTelements |
| Notes | IndieAuthXAdESXBLXHTML+SMILXUP |
| Working drafts | CCXMLCURIEEMEInkMLMSESMIL TimesheetssXBLWebGPUWebXRXFDLXFramesXMLHttpRequest |
| Guidelines | Web Content Accessibility Guidelines |
| Initiative | Markup Validation ServiceWeb Accessibility InitiativeWeb Components |
| Deprecated | C-HTMLHDMLJSSSPGMLVMLWebPlatform |
| Obsoleted | P3PXHTML+MathML+SVG |
| Groups,organizations | WHATWGDefunct:World Wide Web FoundationElectedABBoardTAGWorkingCSSSVGWebAssemblyWebAuthnCommunity, businessWeb Advertising BGWebAssemblyCGClosedDevice Description(DDWG)HTMLMultimodal Interaction Activity(MMI) | WHATWGDefunct:World Wide Web Foundation | Elected | ABBoardTAG | Working | CSSSVGWebAssemblyWebAuthn | Community, business | Web Advertising BGWebAssemblyCG | Closed | Device Description(DDWG)HTMLMultimodal Interaction Activity(MMI) |
| WHATWGDefunct:World Wide Web Foundation |
| Elected | ABBoardTAG |
| Working | CSSSVGWebAssemblyWebAuthn |
| Community, business | Web Advertising BGWebAssemblyCG |
| Closed | Device Description(DDWG)HTMLMultimodal Interaction Activity(MMI) |
| Software | CERN httpdLibwwwBrowsersLine Mode(1990–)Arena(1993–98)Agora(1994–97)Argo(1994–97)Amaya(browser/editor, 1996–2012) | CERN httpdLibwww | Browsers | Line Mode(1990–)Arena(1993–98)Agora(1994–97)Argo(1994–97)Amaya(browser/editor, 1996–2012) |
| CERN httpdLibwww |
| Browsers | Line Mode(1990–)Arena(1993–98)Agora(1994–97)Argo(1994–97)Amaya(browser/editor, 1996–2012) |
| Conferences | International World Wide Web Conference(IW3C)Steering Committee(IW3C2)First conference("WWW1", 1994) |