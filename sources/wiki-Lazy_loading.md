---
source: https://en.wikipedia.org/wiki/Lazy_loading
fetched: 2026-06-20
---

Design pattern in computer programming 

**Lazy loading** (also known as **asynchronous loading**) is a technique used in [computer programming](./Computer_programming), especially [web design](./Web_design) and [web development](./Web_development), to defer initialization of an [object](./Object_(computer_science)) until it is needed. It can contribute to efficiency in the program's operation if properly and appropriately used. This makes it ideal in use cases where [network](./Computer_network) content is accessed and initialization times are to be kept at a minimum, such as in the case of [web pages](./Web_page). For example, deferring loading of images on a web page until they are needed for viewing can make the initial display of the web page faster. The opposite of lazy loading is **eager loading**.[[1]](./Lazy_loading#cite_note-1)

 

## Examples

 

### With web frameworks

 

Prior to being established as a web standard, [web frameworks](./Web_framework) were generally used to implement lazy loading.

 

One of these is [Angular](./Angular_(web_framework)). Since lazy loading decreases bandwidth and subsequently server resources, it is a strong contender to implement in a website, especially in order to improve [user retention](./Retention_rate) by having less delay when loading the page, which may also improve [search engine optimization](./Search_engine_optimization) (SEO).[[2]](./Lazy_loading#cite_note-2)

 

Below is an example of lazy loading being used in Angular, programmed in [TypeScript](./TypeScript), from [Farata Systems](https://github.com/Farata/angulartypescript/blob/master/code-samples/Angular9/chapter4/router-advanced-samples/src/app/lazy/app.module.ts)[[3]](./Lazy_loading#cite_note-3)

 
```
@NgModule({
  imports: [ BrowserModule,
    RouterModule.forRoot([
      {path: '',        component: HomeComponent},
      {path: 'product', component: ProductDetailComponent},

      {path: 'luxury', loadChildren: () => import('./luxury.module').then(m => m.LuxuryModule), data: {preloadme: true} } ]
//      , {preloadingStrategy: CustomPreloadingStrategy}
      )
  ],
  declarations: [ AppComponent, HomeComponent, ProductDetailComponent],
  providers:[{provide: LocationStrategy, useClass: HashLocationStrategy}, CustomPreloadingStrategy],
  bootstrap:    [ AppComponent ]
})

```
 

### As a web standard

 

Since 2020, major web browsers have enabled native handling of lazy loading by default.[[4]](./Lazy_loading#cite_note-4)[[5]](./Lazy_loading#cite_note-5)

 

This allows lazy loading to be incorporated into a webpage by adding [HTML attributes](./HTML_attributes).

 

The `loading` attribute support two values, `lazy` and `eager`.[[6]](./Lazy_loading#cite_note-6) Setting the value to `lazy` will fetch the resource only when it is required (such as when an image scrolls into view when a user scrolls down), while setting it to `eager`, the default state, the resource will be immediately loaded.

 
```
<!-- These resources will be loaded immediately -->
<img src="header_image.jpg">
<img src="header_image2.jpg" loading="eager">

<!-- While these resources will be lazy loaded -->
<img src="article_image.jpg" alt="..." loading="lazy"> 
<iframe src="video-player.html" title="..." loading="lazy"></iframe>

```
 

## Methods

 

There are four common ways of implementing the lazy load design pattern: *lazy initialization*; a *virtual proxy*; a *ghost*, and a *value holder*.[[7]](./Lazy_loading#cite_note-7) Each has its own advantages and disadvantages.

 

### Lazy initialization

 Main article: [Lazy initialization](./Lazy_initialization) 

With lazy initialization, the object is first set to `null`.

 

Whenever the object is requested, the object is checked, and if it is `null`, the object is then immediately created and returned.

 

For example, lazy loading for a widget can be implemented in the [C#](./C_Sharp_(programming_language)) programming language as such:

 
```
private int _myWidgetID;
private Widget _myWidget = null;

public Widget MyWidget
{
    get
    {
        if (_myWidget == null)
        {
            _myWidget = Widget.Load(_myWidgetID);
        }

        return _myWidget;
    }
}

```
 

Or alternatively, with the [null-coalescing assignment operator](./Null_coalescing_operator) `??=`

 
```
private int _myWidgetID;
private Widget _myWidget = null;

public Widget MyWidget
{
    get => _myWidget ??= Widget.Load(_myWidgetID);
}

```
 

This method is the simplest to implement, although if `null` is a legitimate return value, it may be necessary to use a placeholder object to signal that it has not been initialized. If this method is used in a [multithreaded application](./Multithreading_(software)), synchronization must be used to avoid [race conditions](./Race_condition).

 

### Virtual proxy

 

A virtual proxy is an object with the same interface as the real object.  The first time one of its methods is called it loads the real object and then delegates.

 

### Ghost

 

A *ghost* is the object that is to be loaded in a partial state.  It may initially only contain the object's identifier, but it loads its own data the first time one of its properties is accessed.  For example, consider that a user is about to request content via an online form.  At the time of creation, the only information available is that content will be accessed, but the specific action and content is unknown.

 

An example in [PHP](./PHP):

 
```
$userData = array (
    "UID" = > uniqid(),
    "requestTime" => microtime(true),
    "dataType" => "",
    "request" => ""
);

if (isset($_POST['data']) && $userData) {
    // ...
}

```
 

### Value holder

 

A *value holder* is a generic object that handles the lazy loading behavior, and appears in place of the object's data fields:

 
```
private ValueHolder<Widget> valueHolder;

public Widget MyWidget => valueHolder.GetValue();

```
 

## See also

 
- [Demand paging](./Demand_paging)
- [Dynamic loading](./Dynamic_loading)
- [Proxy pattern](./Proxy_pattern)
- [Lazy evaluation](./Lazy_evaluation)
- [Lazy initialization](./Lazy_initialization)
- [Software design pattern](./Software_design_pattern)

 

## References

  
1. [↑](./Lazy_loading#cite_ref-1) ["What is Lazy Loading | Lazy vs. Eager Loading | Imperva"](https://www.imperva.com/learn/performance/lazy-loading/). *Learning Center*. Retrieved 2022-02-02.
2. [↑](./Lazy_loading#cite_ref-2) ["What Is Lazy Loading? Understanding Lazy Loading for SEO"](https://www.wordstream.com/blog/ws/2020/12/08/lazy-loading-seo).
3. [↑](./Lazy_loading#cite_ref-3) Fain, Y., Moiseev, A. (2018). Angular Development with TypeScript, Second Edition. December   [ISBN](./ISBN_(identifier)) [9781617295348](./Special:BookSources/9781617295348).
4. [↑](./Lazy_loading#cite_ref-4) ["A Deep Dive into Native Lazy-Loading for Images and Frames"](https://css-tricks.com/a-deep-dive-into-native-lazy-loading-for-images-and-frames/). 15 May 2019.
5. [↑](./Lazy_loading#cite_ref-5) ["Firefox 75 gets lazy loading support for images and iframes"](https://www.ghacks.net/2020/02/15/firefox-75-gets-lazy-loading-support-for-images/). 15 February 2020.
6. [↑](./Lazy_loading#cite_ref-6) ["Lazy loading - Web Performance | MDN"](https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading). *developer.mozilla.org*. Retrieved 2022-03-15.
7. [↑](./Lazy_loading#cite_ref-7) Martin Fowler (2003). *Patterns of Enterprise Application Architecture*. Addison-Wesley. pp. 200–214. [ISBN](./ISBN_(identifier)) [0-321-12742-0](./Special:BookSources/0-321-12742-0).

 

## External links

 
- [Lazy Loading, Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/Performance/Lazy_loading)
- [URLs, WHATWG HTML Standard](https://html.spec.whatwg.org/multipage/urls-and-fetching.html#lazy-loading-attributes)
- [JS Lazy Loading](https://javahubscript.com/lazy-loading-in-javascript-examples/)

 
| vteSoftware design patterns |
| --- |
| Gang of Fourpatterns | CreationalAbstract factoryBuilderFactory methodPrototypeSingletonStructuralAdapterBridgeCompositeDecoratorFacadeFlyweightProxyBehavioralChain of responsibilityCommandInterpreterIteratorMediatorMementoObserverStateStrategyTemplate methodVisitor | Creational | Abstract factoryBuilderFactory methodPrototypeSingleton | Structural | AdapterBridgeCompositeDecoratorFacadeFlyweightProxy | Behavioral | Chain of responsibilityCommandInterpreterIteratorMediatorMementoObserverStateStrategyTemplate methodVisitor |
| Creational | Abstract factoryBuilderFactory methodPrototypeSingleton |
| Structural | AdapterBridgeCompositeDecoratorFacadeFlyweightProxy |
| Behavioral | Chain of responsibilityCommandInterpreterIteratorMediatorMementoObserverStateStrategyTemplate methodVisitor |
| Concurrencypatterns | Active objectBalkingBinding propertiesDouble-checked lockingEvent-based asynchronousGuarded suspensionJoinLockMonitorProactorReactorRead–write lockSchedulerScheduled-task patternSemaphoreThread poolThread-local storage |
| Architecturalpatterns | Front controllerInterceptorMVCMVPMVVMADRECSn-tierSpecificationPublish–subscribeNaked objectsService locatorActive recordIdentity mapData access object (DAO)Data transfer object (DTO)Inversion of controlModel 2Broker |
| Otherpatterns | BlackboardBusiness delegateComposite entityComposition over inheritanceDependency injectionGuard clauseIntercepting filterLazy loadingMock objectNull objectObject poolServantTwinType tunnelMethod chainingDelegation |
| Books | Design PatternsEnterprise Integration Patterns |
| People | Christopher AlexanderErich GammaRalph JohnsonJohn VlissidesGrady BoochKent BeckWard CunninghamMartin FowlerRobert MartinJim CoplienDouglas SchmidtLinda Rising |
| Communities | The Hillside GroupPortland Pattern Repository |
| See also | Anti-patternArchitectural pattern |

   

 

 
|  | Thiscomputer-programming-related article is astub. You can help Wikipedia byadding missing information. |
| --- | --- |

- [v](./Template:Compu-prog-stub)
- [t](./Template_talk:Compu-prog-stub)
- [e](./Special:EditPage/Template:Compu-prog-stub)