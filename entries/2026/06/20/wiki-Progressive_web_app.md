---
source: sources/wiki-Progressive_web_app.md
source_url: https://en.wikipedia.org/wiki/Progressive_web_app
---

## Progressive Web Apps (PWAs)

Progressive web apps are web applications built with standard web technologies (HTML, CSS, JavaScript, WebAssembly) that can be installed on a device as standalone applications. They use the device's browser offline cache for installation and work cross-platform without requiring separate bundling or distribution per platform. Introduced from 2016 as an alternative to native apps, the term was coined by Frances Berriman and Google Chrome engineer Alex Russell in 2015.

## Key Concepts

- A PWA is a web app that meets specific installability criteria, allowing it to function like a native app on desktop and mobile
- PWAs use **progressive enhancement** — they work on any standards-compliant browser but offer richer experiences on more capable ones
- The **App Shell Model** caches the basic UI shell offline via service workers, enabling native-like use with or without connectivity
- Two core required components: a **web app manifest** and a **service worker**
- PWAs are significantly smaller than native apps (Twitter Lite: 1–3% of native app size; Starbucks PWA: 99.84% smaller than iOS app)
- Publishing to app stores (Apple App Store, Google Play, Microsoft Store) is optional, not required
- Microsoft Store auto-publishes qualifying PWAs discovered via Bing indexing

## Commands and Syntax

**Web App Manifest (manifest.json)** — W3C-specified JSON file with required properties:
- `name` or `short_name`
- `start_url`
- `display` (value: `standalone`, `fullscreen`, or `minimal-ui`)
- `icons` (192px and 512px versions required)

**Technical installation criteria (three requirements):**
1. Served over **HTTPS** (TLS, no active mixed content)
2. Registers a **service worker** with a fetch handler
3. References a valid **web app manifest**

**Service worker lifecycle (three phases):**
1. **Registration** — browser told location of the service worker
2. **Installation** — occurs when no service worker exists or an update is available
3. **Activation** — occurs when all PWA pages are closed, preventing version conflicts

**iOS-specific:** Safari uses Apple-specific meta tag extensions instead of full manifest support for defining icons, splash screens, full-screen display, and app name.

**Data storage options:**
- `localStorage` — persists across sessions (key-value, Web Storage API)
- `sessionStorage` — cleared when browser session ends (key-value, Web Storage API)
- **IndexedDB** — W3C standard for storing JSON objects and structured data

## Relationships

- **Service Workers** are a specialized type of **Web Worker** that act as programmable network proxies
- **WebAssembly** extends PWA capabilities by allowing precompiled code (C, etc.) to run at near-native speed in-browser
- **Responsive Web Design** enabled PWA development by providing screen-size flexibility
- **Firefox OS** (2013–2017) was a predecessor that ran web apps as native apps; its fork became **KaiOS** for feature phones
- **Google Lighthouse** is the open-source audit tool for evaluating PWAs
- PWAs relate to the broader **progressive enhancement** strategy — baseline functionality everywhere, enhanced where supported

## Exam-Relevant Points

- Three mandatory technical criteria: HTTPS, service worker with fetch handler, web app manifest
- Manifest must include: `name`/`short_name`, `start_url`, `display`, and `icons` (192px + 512px)
- Valid `display` values: `standalone`, `fullscreen`, `minimal-ui`
- Service worker lifecycle: Registration → Installation → Activation
- Only one service worker can be active per domain at a time
- Service workers can handle push notifications, background sync, and network interception even when the registering document is not loaded
- Browser support as of 2025: Chromium-based browsers have full support; Firefox added Windows PWA support in v143 (Sept 2025); Safari has partial support on macOS and iOS; Firefox desktop (non-Windows) abandoned PWA support in Dec 2020
- App store support: Google Play, Microsoft Store, and Samsung Galaxy Store support PWAs; Apple App Store does not
- Service worker caches differ from HTTP caches — they can **prefetch** content before first use and **explicitly discard** when no longer needed
- WebAssembly became a W3C Recommendation on December 5, 2019
- The term "progressive web apps" was coined in 2015 by Frances Berriman and Alex Russell
