[android-components](../../index.md) / [mozilla.components.browser.thumbnails](../index.md) / [BrowserThumbnails](./index.md)

# BrowserThumbnails

`class BrowserThumbnails : `[`LifecycleAwareFeature`](../../mozilla.components.support.base.feature/-lifecycle-aware-feature/index.md) [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/browser/thumbnails/src/main/java/mozilla/components/browser/thumbnails/BrowserThumbnails.kt#L25)

Feature implementation for automatically taking thumbnails of sites.
The feature will take a screenshot when the page finishes loading,
and will add it to the [Session.thumbnail](../../mozilla.components.browser.session/-session/thumbnail.md) property.

If the OS is under low memory conditions, the screenshot will be not taken.
Ideally, this should be used in conjunction with [SessionManager.onLowMemory](../../mozilla.components.browser.session/-session-manager/on-low-memory.md) to allow
free up some [Session.thumbnail](../../mozilla.components.browser.session/-session/thumbnail.md) from memory.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | `BrowserThumbnails(context: <ERROR CLASS>, engineView: `[`EngineView`](../../mozilla.components.concept.engine/-engine-view/index.md)`, sessionManager: `[`SessionManager`](../../mozilla.components.browser.session/-session-manager/index.md)`)`<br>Feature implementation for automatically taking thumbnails of sites. The feature will take a screenshot when the page finishes loading, and will add it to the [Session.thumbnail](../../mozilla.components.browser.session/-session/thumbnail.md) property. |

### Functions

| Name | Summary |
|---|---|
| [start](start.md) | `fun start(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Starts observing the selected session to listen for when a session finish loading. |
| [stop](stop.md) | `fun stop(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)<br>Stops observing the selected session. |

### Extension Functions

| Name | Summary |
|---|---|
| [loadResourceAsString](../../mozilla.components.support.test.file/kotlin.-any/load-resource-as-string.md) | `fun `[`Any`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)`.loadResourceAsString(path: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`): `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)<br>Loads a file from the resources folder and returns its content as a string object. |
