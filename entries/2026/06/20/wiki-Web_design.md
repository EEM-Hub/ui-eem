---
source: sources/wiki-Web_design.md
source_url: https://en.wikipedia.org/wiki/Web_design
---

## Web Design: Disciplines, History, and Core Techniques

Web design encompasses the skills and disciplines involved in creating and maintaining websites, focusing on the front-end (client-side) experience. It spans graphic design, UI/UX design, markup authoring, and SEO, and partially overlaps with web engineering and the broader field of web development.

## Key Concepts

- **Web design** covers: web graphic design, UI design, UX design, standardized/proprietary code authoring, and SEO
- **Progressive enhancement**: a layered strategy — serve content via HTML first, style with CSS, then enhance with JavaScript — ensuring universal access and backward compatibility
- **Static websites**: pre-built pages served as-is; simpler hosting, faster serving, fewer security risks; static site generators (e.g., Jekyll) gained popularity around 2015
- **Dynamic websites**: generated on the fly using server-side technology and back-end databases (relational or document-based like MongoDB/NoSQL)
- **Fluid layouts**: adjust to browser/screen characteristics; alternative to fixed HTML-table layouts, slow to adopt due to screen reader and window-size variability
- **Responsive web design**: CSS3-based approach using `@media` rules for per-device styling; Google announced mobile-first indexing in March 2018
- **Homepage importance is debated**: usability experts (Jakob Nielsen) emphasized it, but growing search/RSS traffic bypasses homepages; Jared Spool (2007) argued it's the *least* important page
- **Carousels/sliders**: popular homepage element (2012-2013) but widely criticized for hurting SEO and usability

## Commands and Syntax

- **HTML `<table>` tag**: originally for tabular data, historically misused for page layout (multi-column structures); replaced by CSS-based layouts
- **CSS `@media` rule**: enables responsive design by applying device-specific styles within a stylesheet
- **W3C Markup Validation**: validates HTML against doctype declaration to identify standards-compliance errors
- **Font downloading** (CSS3 fonts module): allows custom web fonts; supported in Safari 3.1, Opera 10, Firefox 3.5+
- **Content management systems** (CMS): higher-level tools (blogs, wikis, forums) that abstract away direct coding
- **WYSIWYG website builders**: visual editors for creating sites without hand-coding markup

## Relationships

- **UI Design / UX Design**: core subdisciplines of web design; UX focuses on usability, content understanding, and interaction patterns
- **Web Accessibility (W3C guidelines)**: web designers must follow accessibility standards, including allowing users to disable animations
- **Web Engineering / Web Development**: web design is a subset; development includes server-side and database work beyond front-end design
- **SEO**: directly tied to design decisions — responsive design supports mobile-first indexing; carousels can hurt SEO
- **Browser Wars (1996-2001)**: Microsoft vs. Netscape competition drove adoption of CSS, JavaScript, and Dynamic HTML
- **W3C Standards**: HTML5, CSS3, JavaScript APIs — W3C (est. 1994) sets interoperability standards to prevent proprietary lock-in
- **Content Management Systems**: bridge between web design and dynamic content — WordPress, wikis, forums abstract layout from content

## Exam-Relevant Points

- **Tim Berners-Lee** proposed the World Wide Web in 1989 at CERN; text-only HTML pages viewable 1991-1993
- **Mosaic browser** (1993, Andreessen & Bina) was first to integrate graphic design elements into browsing
- **W3C** founded October 1994 to develop common protocols and prevent proprietary monopolization
- **CSS introduced December 1996** by W3C, separating presentation from semantic HTML (tableless web design)
- **Flash** (originally FutureSplash, 1996) enabled rich media but required plug-ins, limiting adoption
- **IE for Mac (2000)**: first browser to fully support HTML 4.01, CSS 1, and PNG format
- **By 2001**, Internet Explorer held 96% browser market share, ending the first browser wars
- **Progressive enhancement order**: HTML (content) → CSS (styling) → JavaScript (interactivity)
- **Mobile-first approach**: emerged with 3G/LTE growth; design for mobile first, then adapt to larger screens
- **Google mobile-first indexing**: announced March 2018; responsive design is essential
- **Two primary roles**: web designer (visual/layout) and web developer (programming/functionality)
- **Static vs. dynamic sites**: static = pre-built files, simpler/faster/more secure; dynamic = server-generated, requires broader skillset, typically a team effort
- **Accessibility requirement**: W3C standards mandate that users can disable motion graphics/animations
