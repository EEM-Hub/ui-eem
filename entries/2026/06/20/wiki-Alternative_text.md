---
source: sources/wiki-Alternative_text.md
source_url: https://en.wikipedia.org/wiki/Alternative_text
---

## HTML Alt Attribute: Alternative Text for Images

The `alt` attribute is an HTML/XHTML attribute that specifies alternative text to display when an HTML element (typically an image) cannot be rendered. It serves accessibility, SEO, and usability purposes and is recommended by the W3C for every image. Its absence has been the basis for accessibility-related lawsuits under disability discrimination laws.

## Key Concepts

- **Alt text** replaces images when they cannot be loaded, without changing the page's intended meaning
- The alt attribute conveys the **meaning and intent** of an image, not a literal visual description (e.g., a logo's alt text should say "Company logo," not describe the logo's appearance)
- Alt text should be **short and concise**; longer descriptions use the `longdesc` attribute
- **Decorative images** that convey no information should use an empty alt attribute (`alt=""`) so screen readers skip them; decorative images are better specified in CSS
- Omitting the alt attribute entirely causes browsers to display the URL or filename, creating ambiguity for users
- A 2021 Google Lighthouse audit found **27% of alt attributes were empty**, even though most of those images were non-decorative
- Screen readers (e.g., Orca) and text-based browsers (e.g., Lynx) read alt text in place of images
- Alt text improves **SEO** — search engines read it like regular text; image search engines (Google Images) use it to index and surface relevant images
- Alt text for non-image search is treated the same as regular page text by search engines
- IE7 and earlier incorrectly rendered alt text as tooltips; this led developers to misuse alt instead of the `title` attribute for tooltips (fixed in IE8)

## Commands and Syntax

```html
<!-- Informational image with descriptive alt text -->
<img src="logo.png" alt="Acme Corporation logo">

<!-- Decorative image with empty alt (screen readers skip it) -->
<img src="divider.png" alt="">

<!-- No alt attribute (avoid — browser shows URL/filename) -->
<img src="photo.jpg">
```

- **Required on**: `<img>` and `<area>` tags (since HTML 4.01, 1999)
- **Optional on**: `<input>` and the deprecated `<applet>` tag
- First introduced in **HTML 1.2 draft (1993)** for text-based browser support
- For tooltips, use the `title` attribute, not `alt`

## Relationships

- **WCAG (Web Content Accessibility Guidelines)**: Alt text usage is part of W3C's WCAG standards
- **longdesc attribute**: Complements alt for longer image descriptions; alt remains required even when longdesc is present
- **title attribute**: Intended for tooltips; commonly confused with alt due to IE's non-standard behavior
- **CSS**: W3C recommends decorative images be specified in CSS rather than HTML markup
- **Screen readers / text-based browsers**: Primary consumers of alt text for accessibility
- **SEO / Google Images**: Alt text is a ranking factor specifically for image search results
- **ADA / disability law**: Missing alt attributes cited as a barrier to web accessibility under the Americans with Disabilities Act

## Exam-Relevant Points

- Alt attribute became **required** on `<img>` and `<area>` in **HTML 4.01 (1999)**
- Alt text should describe the image's **purpose/meaning**, not its visual appearance
- Decorative images must use `alt=""` (empty string), not omit the attribute entirely
- Omitting alt causes browsers to show the URL/filename — worse than an empty alt
- The `title` attribute is for tooltips; `alt` is for alternative text — they are distinct
- **NFB v. Target Corp. (2006)**: Set U.S. legal precedent for website accessibility under the ADA
- **Maguire v. Sydney Olympic Committee (2000)**: Australian ruling that a website without alt attributes discriminated against blind users
- The U.S. Department of Justice cites missing alt attributes as an example of an ADA accessibility barrier
- Alt text is a factor for **image search** ranking but not for general web search ranking (per Google)
- W3C recommends every image have an alt attribute, but the attribute **does not need to contain text** (can be empty for decorative images)
