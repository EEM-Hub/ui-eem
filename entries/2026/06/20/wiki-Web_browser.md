---
source: sources/wiki-Web_browser.md
source_url: https://en.wikipedia.org/wiki/Web_browser
---

## Web Browsers: Architecture, Market, and Security

A web browser is application software that retrieves content from web servers using HTTP/HTTPS and renders it for display on a user's device. This page covers how browsers work, their history from the first browser in 1990 through the AI browser era, key features, market share data, and security/privacy considerations.

## Key Concepts

- A browser is an **HTTP client** (user agent) that fetches resources via URLs and renders them using a **browser engine** (layout/rendering engine)
- **Browser engine** converts downloaded HTML, CSS, images, and multimedia into an interactive visual page; a separate **JavaScript engine** handles dynamic content
- A **headless browser** renders pages without a graphical user interface
- A browser is **not** a search engine — a browser displays pages, a search engine indexes and links to them
- **Web cache** stores previously fetched resources locally; cache duration is controlled by HTTP response headers from the server
- **HTTPS** encrypts the connection between browser and server for secure, private data transfer
- **Content Decryption Module (CDM)** — e.g., Widevine — enables browsers to play DRM-restricted streaming content; licensing costs limit CDM availability in independent open-source browsers
- **Cookies** store login credentials and preferences but are also used for cross-site tracking
- **AI browsers** (mid-2020s onward) integrate chatbots and AI features directly into the browsing experience (e.g., Chrome+Gemini, Edge+Copilot, Perplexity Comet, ChatGPT Atlas)

## Commands and Syntax

No CLI commands per se, but key technical details:

- URLs begin with `http:` or `https:` — the protocol prefix determines whether the connection is encrypted
- The address bar accepts both URLs and search queries (merged with search bar in most modern browsers)
- Private/incognito mode disables browsing history logging for that session

## Relationships

- **HTTP/HTTPS** — the transport protocol browsers use; HTTPS adds TLS encryption
- **HTML, CSS, JavaScript** — the content languages browsers parse and render
- **Browser engines** — Blink (Chromium/Chrome/Edge/Opera/Samsung), WebKit (Safari), Gecko (Firefox) determine rendering behavior
- **Chromium** — Google's open-source project underpinning Chrome, Edge, Samsung Internet, Opera, Brave, and many others
- **Search engines** — commonly accessed via browsers but are distinct services (Google, Bing, DuckDuckGo)
- **DRM / Widevine** — gates access to streaming content within browsers
- **Web tracking / fingerprinting** — privacy concerns that drive features like tracker blocking and private browsing modes

## Exam-Relevant Points

- **First web browser**: WorldWideWeb, created by Tim Berners-Lee in 1990
- **First mainstream browser**: Mosaic (released April 1993), credited with sparking the 1990s Internet boom
- **Browser wars**: Microsoft bundled IE with Windows as freeware, reaching 95%+ market share in early 2000s; Chrome overtook IE in 2012
- **Market share (2025-2026)**: Chrome ~63-69%, Safari ~16-17%, Edge ~5-7%, Firefox ~2-4%, Samsung Internet ~2%, Opera ~1-2%
- **Three major engine families**: Chromium/Blink (Chrome, Edge, Opera, Samsung, Brave), WebKit (Safari), Gecko (Firefox)
- **Mobile vs desktop traffic**: Mobile surpassed desktop in late 2016; as of 2025, mobile is ~62%, desktop ~36%, tablet ~2%
- **Privacy-focused browsers** (Brave, DuckDuckGo, LibreWolf, Tor, Mullvad) outperform mainstream browsers on privacy by blocking fingerprinting, trackers, and ads
- **Netscape** released Navigator in 1994 (from Mosaic developers); founded Mozilla in 1998, which produced Firefox (released 2004, peaked at 32% share in 2010)
- **Edge Legacy** replaced IE in Windows 10 (2015); rebuilt on Chromium in 2020
- An estimated **5.4 billion people** had used a browser as of 2023
