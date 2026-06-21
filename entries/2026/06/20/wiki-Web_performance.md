---
source: sources/wiki-Web_performance.md
source_url: https://en.wikipedia.org/wiki/Web_performance
---

## Web Performance Optimization (WPO)

Web performance refers to the speed at which web pages are downloaded and displayed in a user's browser. Web Performance Optimization (WPO) is the discipline of improving this speed through front-end and back-end techniques. Faster sites increase visitor retention, user satisfaction (especially on mobile/slow connections), and reduce power consumption and environmental impact. Steve Souders coined the term "WPO" in 2004 and established that at least 80% of page load time is controlled by front-end structure.

## Key Concepts

- **Front End Optimization (FEO):** Also called content optimization — focuses on reducing file sizes and minimizing the number of HTTP requests per page load.
- **Resource consolidation:** Bundling smaller files (e.g., images) into one to reduce HTTP round trips, since browsers limit simultaneous TCP connections per host.
- **File compression:** Reduces code file sizes by ~40%, improving responsiveness.
- **Code minification:** Removes comments, whitespace, and shortens variable names — can reduce file size by up to 60%.
- **Image optimization:** Lossy compression removes non-essential header data and lowers quality imperceptibly; vector graphics can replace raster graphics for simple geometric images.
- **Lazy loading:** Defers loading of images/video until they are needed (e.g., user scrolls into view), reducing initial page load time and resource usage.
- **Web caching:** Stores copies of documents to reduce server load, bandwidth, and latency. Caches can be client-side (forward) or server-side (reverse). HTTP cache uses request/response headers for configuration.
- **Content Delivery Network (CDN):** A network of geographically distributed proxy servers that selects the closest/fastest server for each user.
- **HTTP/2 improvements over HTTP/1.x:** Binary protocol, fully multiplexed (single connection for parallelism), header compression, and server push into client caches.

## Commands and Syntax

No CLI commands are specified in this source. Key tools and measurement approaches include:

- **Google Lighthouse:** Chrome DevTools component for measuring performance.
- **PageSpeed Insights:** Google site for measuring/comparing website performance against recommended thresholds.
- **core-web-vitals library:** Google-published JS library for measuring performance metrics in frontend apps.
- **Firefox Network Monitor:** Provides insight into network-level transmission slowdowns.
- **Framework integration:** React (`create-react-app` measuring-performance), NuxtJS (`@nuxtjs/web-vitals`), Vue (`vue-web-vitals`) all provide modules for metric collection.

## Relationships

- **HTTP/TCP:** Web performance is fundamentally constrained by HTTP request overhead and TCP connection limits per host.
- **CDNs + HTTP/2:** Used together — CDNs serve static assets (JS, CSS, images) from locations closer to end users; HTTP/2 multiplexing reduces connection overhead.
- **User Experience (UX):** WPO directly improves UX; Google uses site speed as a search ranking factor.
- **Presentation layer / Asynchronous communication:** Lightweight presentation components and async server communication are architectural strategies for performance.
- **SSL/TLS:** Encryption adds rendering time — a trade-off between security and performance.

## Exam-Relevant Points

- **80% rule (Souders, 2007):** At least 80% of page load time is determined by front-end structure, not back-end.
- **File compression reduces code files by ~40%; minification can reduce by up to 60%.**
- **HTTP/2 vs HTTP/1 differences:** Binary (not textual), fully multiplexed (not ordered/blocked), single connection for parallelism, header compression, server push.
- **Google Core Web Vitals metrics:** TTFB (Time to First Byte), FCP (First Contentful Paint), FP (First Paint), FID (First Input Delay), CLS (Cumulative Layout Shift), LCP (Largest Contentful Paint) — introduced 2019.
- **Additional metrics:** Request Count, DOMContentLoaded, Above The Fold Time, Round Trip Time, Render Blocking Resources count, Onload Time, Connection Time, Total Page Size.
- **Lazy loading** reduces initial page load time, page weight, and system resource usage.
- **CDN selection logic:** Chooses the server with the quickest response time based on network proximity.
- **Web cache positions:** Forward (client-side) vs. reverse (server-side).
- **Steve Souders** coined "WPO" in 2004; predicted speed as a competitive differentiator and environmental impacts of optimization.
