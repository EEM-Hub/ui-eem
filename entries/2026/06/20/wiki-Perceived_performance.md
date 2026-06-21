---
source: sources/wiki-Perceived_performance.md
source_url: https://en.wikipedia.org/wiki/Perceived_performance
---

## Perceived Performance

Perceived performance refers to how quickly a software feature *appears* to perform its task from the user's perspective, as distinct from actual (real) performance. It is primarily a user acceptance concern — the goal is to satisfy human cognitive expectations around responsiveness, even when real performance cannot be improved due to physical or technical limitations.

## Key Concepts

- **Perceived vs. real performance**: Perceived performance is the user's subjective experience of speed; real performance is the measurable elapsed time. They are correlated but not identical.
- **Visual feedback**: Showing progress indicators (splash screens, progress bars, loading spinners) makes operations *feel* faster by acknowledging the user's request, even though rendering these elements consumes a small amount of processing time.
- **Exploiting perceptual limits**: All perceived-performance techniques rely on the user's inability to accurately judge real performance. If users could detect the overhead, the technique would be considered detrimental.
- **Increasing delay can help**: In some cases (e.g., smoothing user input via a running average), adding a small delay improves the *feeling* of control and smoothness, such as reducing jitter on a game controller input.
- **Precomputation**: Performing work ahead of time (e.g., pre-sorting data before the user requests it) shifts latency away from user-triggered actions, improving perceived responsiveness.
- **Render-blocking vs. non-blocking resources**: In web contexts, loading non-blocking content first (text, images) and deferring render-blocking resources (CSS, JS) lets users see content sooner.

## Commands and Syntax

No CLI commands per se, but key web performance practices:

- **Minimize initial page load**: Load only resources needed for first visible content; lazy-load the rest.
- **Prioritize interactivity**: Ensure clickable/interactive elements are functional as early as possible, even while the page is still loading.
- **Prevent layout shift/flicker**: Use placeholders with explicit width and height for images, charts, and embedded content. Match fallback font size/style to the web font to minimize visible swap.

**Tools for measurement:**
- **Chrome DevTools** — built-in performance profiling and rendering analysis.
- **WebPageTest** (webpagetest.org) — provides SpeedIndex, which measures the average time for the visible portion of a page to render.

## Relationships

- **Progress bars / splash screens**: Direct implementations of perceived performance — they provide visual feedback during long operations.
- **Web performance optimization**: Perceived performance is a core pillar alongside real performance metrics (TTFB, LCP, FID).
- **User experience (UX)**: Perceived performance directly impacts user satisfaction and acceptance; poor perceived performance drives abandonment regardless of actual speed.
- **Input smoothing / game design**: The running-average technique connects to control systems and human-computer interaction design in interactive applications.
- **Lazy loading / code splitting**: Technical strategies that operationalize perceived performance for the web by deferring non-critical resources.

## Exam-Relevant Points

- Perceived performance is about user *perception* of speed, not actual measured speed — a progress bar makes an operation feel faster even though it adds marginal overhead.
- Techniques work by exploiting the user's inability to accurately measure real performance.
- Sometimes *adding* latency (e.g., input smoothing) improves perceived performance.
- For web: load non-blocking resources first, defer render-blocking resources, use placeholders to prevent layout shift.
- SpeedIndex (via WebPageTest) is the key metric for measuring perceived web performance — it represents the average time for the visible area to be displayed.
- Increasing real performance generally increases perceived performance, but perceived performance can be improved independently when real performance hits physical limits.
