---
source: sources/wiki-Lazy_loading.md
source_url: https://en.wikipedia.org/wiki/Lazy_loading
---

## Lazy Loading Design Pattern

Lazy loading (also called asynchronous loading) is a software design pattern that defers the initialization of an object until the point at which it is needed. It improves efficiency by reducing initial load times and conserving resources, making it especially valuable in web development where network latency and bandwidth are concerns. The opposite strategy is eager loading, which initializes objects immediately.

## Key Concepts

- **Core idea**: Don't create or load an object until it is actually requested or accessed.
- **Primary benefit**: Reduces initial load time and resource consumption by avoiding unnecessary work upfront.
- **Trade-off**: Lazy loading adds complexity (null checks, proxies, synchronization) in exchange for deferred cost.
- **Web context**: Deferring image and iframe loading improves page speed, user retention, and SEO.
- **Native browser support**: Since 2020, major browsers support lazy loading natively via HTML attributes — no JavaScript framework required.
- **Four implementation methods** (from Fowler's *Patterns of Enterprise Application Architecture*):
  - **Lazy initialization** — field starts as `null`; loaded on first access.
  - **Virtual proxy** — a stand-in object with the same interface; delegates to the real object on first method call.
  - **Ghost** — a partially loaded object (e.g., only an ID); loads full data on first property access.
  - **Value holder** — a generic wrapper that encapsulates the lazy-loading logic, replacing the data field.
- **Thread safety caveat**: Lazy initialization in multithreaded environments requires synchronization to prevent race conditions.
- **Null ambiguity**: If `null` is a valid return value, a sentinel/placeholder object must distinguish "not yet loaded" from "loaded, value is null."

## Commands and Syntax

**HTML native lazy loading (web standard):**
```html
<!-- Eager (default) — loads immediately -->
<img src="header.jpg">
<img src="header.jpg" loading="eager">

<!-- Lazy — loads when scrolled into view -->
<img src="article.jpg" alt="..." loading="lazy">
<iframe src="video.html" title="..." loading="lazy"></iframe>
```
- The `loading` attribute accepts two values: `lazy` and `eager`.

**Lazy initialization in C#:**
```csharp
private Widget _myWidget = null;
public Widget MyWidget
{
    get => _myWidget ??= Widget.Load(_myWidgetID);
}
```

**Angular lazy-loaded route module (TypeScript):**
```typescript
{path: 'luxury', loadChildren: () => import('./luxury.module').then(m => m.LuxuryModule)}
```

## Relationships

- **Proxy pattern** — the virtual proxy method is a direct application of the structural Proxy pattern from the Gang of Four.
- **Lazy initialization / Lazy evaluation** — lazy loading is the object-lifecycle application of the broader lazy evaluation strategy.
- **Demand paging** — the OS-level analogue: memory pages are loaded from disk only when accessed.
- **Dynamic loading** — loading code modules at runtime rather than at program start; a related but distinct concept.
- **Software design patterns** — lazy loading is classified under "Other patterns" alongside dependency injection, null object, and object pool.
- **Eager loading** — the direct opposite; understanding when each is appropriate is essential.

## Exam-Relevant Points

- There are exactly **four** implementation methods: lazy initialization, virtual proxy, ghost, and value holder.
- The HTML `loading` attribute has two values: `lazy` and `eager`; `eager` is the **default**.
- Native browser lazy loading has been supported since **2020** and applies to `<img>` and `<iframe>` elements.
- Lazy initialization requires **synchronization** in multithreaded contexts to avoid race conditions.
- A **virtual proxy** shares the same interface as the real object and delegates on first use.
- A **ghost** starts with partial state (typically just an identifier) and self-populates on first property access.
- The pattern is catalogued in Martin Fowler's *Patterns of Enterprise Application Architecture* (2003), pages 200–214.
- Lazy loading can improve both **page load performance** and **SEO** in web applications.
