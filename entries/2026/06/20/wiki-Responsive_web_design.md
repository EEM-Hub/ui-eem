---
source: sources/wiki-Responsive_web_design.md
source_url: https://en.wikipedia.org/wiki/Responsive_web_design
---

## Responsive Web Design (RWD)

Responsive web design is an approach to web design that makes web pages render well across a variety of devices and screen sizes — from phones to desktops — by using fluid grids, flexible images, and CSS3 media queries. The term was coined by Ethan Marcotte in 2010 and has become a foundational practice in modern front-end development.

## Key Concepts

- **RWD** stands for Responsive Web Design; the approach ensures usability across minimum to maximum display sizes.
- **Three core techniques**: fluid proportion-based grids, flexible images, and CSS3 media queries.
- **Fluid grids** size page elements in relative units (percentages) rather than absolute units (pixels or points).
- **Flexible images** are sized in relative units to prevent them from overflowing their containing element.
- **Media queries** (`@media` rule extension) apply different CSS rules based on device characteristics such as browser window width or physical display size.
- **Mobile-first design** is a related philosophy: build a baseline experience for basic devices, then progressively enhance for smartphones and desktops.
- **Progressive enhancement** vs. **graceful degradation**: RWD favors progressive enhancement — start simple, add complexity — rather than building complex and hoping it degrades gracefully.
- **User interface plasticity**: RWD is an instance of UI plasticity — the capacity of an interface to withstand variations in physical characteristics and environment while preserving usability.
- **RESS** (Responsive design with Server-Side components): a hybrid approach combining client-side RWD with server-side adaptation for better mobile optimization.

## Commands and Syntax

- **Media query example (CSS3)**:
  ```css
  @media (max-width: 768px) {
    .container { width: 100%; }
  }
  ```
- **Fluid grid sizing**: use `%`, `em`, `rem`, or `vw`/`vh` units instead of `px`.
- **Flexible images**:
  ```css
  img { max-width: 100%; height: auto; }
  ```
- **Viewport meta tag** (standard practice, implied by the approach):
  ```html
  <meta name="viewport" content="width=device-width, initial-scale=1">
  ```
- **Testing tools**: browser dev tools in Chrome, Firefox, and Safari all include responsive design viewport resizers.

## Relationships

- **CSS3 and media queries**: RWD depends on media queries, which are an extension of the CSS `@media` rule standardized by W3C.
- **CSS frameworks**: Bootstrap, Foundation, and Tailwind CSS all implement responsive design patterns out of the box.
- **CSS preprocessors**: Sass, Less, and Stylus can be used in server-side RESS approaches.
- **Progressive enhancement**: a precursor philosophy; RWD builds on its principle of layering capability.
- **Adaptive web design**: a related but distinct approach that uses fixed layout sizes for specific breakpoints rather than fully fluid layouts.
- **Tableless web design**: an earlier movement away from HTML tables for layout, which paved the way for CSS-based responsive layouts.
- **SEO / Google ranking**: Google's 2015 "Mobilegeddon" update boosted rankings for mobile-friendly (responsive) sites in mobile search results.
- **Ajax**: used in some implementations to serve different ad variants or content on responsive pages.

## Exam-Relevant Points

- **Definition**: RWD uses three techniques — fluid grids, flexible images, and media queries — coined by Ethan Marcotte in a May 2010 *A List Apart* article.
- **Fluid grids use relative units** (percentages), not absolute units (pixels/points).
- **Flexible images use `max-width: 100%`** to stay within their container.
- **Media queries** are an extension of the CSS `@media` rule and apply styles conditionally based on device characteristics.
- **Mobile-first** means designing the base experience for the smallest screen first, then enhancing — this is the progressive enhancement approach.
- **Graceful degradation** is the opposite philosophy: build for desktop first, then adapt down.
- **Google's Mobilegeddon (2015)** made mobile-friendliness a ranking factor, making RWD an SEO concern.
- **First responsive site**: Audi.com (late 2001), created by a Razorfish team.
- **RESS** combines responsive client-side design with server-side components for better mobile optimization — Google still recommends pure responsive design over RESS for smartphone sites.
- **Challenges**: banner ads and video were historically non-fluid; hybrid fixed+fluid layouts used CSS tables as a workaround.
- **RWD is an example of user interface plasticity** — the ability to preserve usability across varying physical and environmental conditions.
