---
title: MediaSource.canConstructInDedicatedWorker
slug: Web/API/MediaSource/canConstructInDedicatedWorker
page-type: web-api-static-property
tags:
  - API
  - canConstructInDedicatedWorker
  - Experimental
  - Media Source Extensions
  - MediaSource
  - Property
  - Static Property
  - Reference
browser-compat: api.MediaSource.canConstructInDedicatedWorker
---

{{APIRef("Media Source Extensions")}}{{seecompattable}}

The **`canConstructInDedicatedWorker`** static property of the {{domxref("MediaSource")}} interface returns `true` if `MediaSource` worker support is implemented, providing a low-latency feature detection mechanism.

If this were not available, the alternative would be a much higher latency approach such as attempting the creation of a `MediaSource` object from a dedicated worker and transferring the result back to the main thread.

## Value

A boolean. Returns `true` if `MediaSource` worker support is implemented, or `false` otherwise.

## Examples

```js
if(MediaSource.canConstructInDedicatedWorker) {
  // MSE is available in workers; let's do this
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [MSE-in-Workers Demo by Matt Wolenetz](https://wolenetz.github.io/mse-in-workers-demo/mse-in-workers-demo.html)
- {{domxref("Media Source Extensions API", "Media Source Extensions API", "", "nocode")}}
- {{domxref("MediaSource")}}
- {{domxref("SourceBuffer")}}
