---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för att ladda ."
type: docs
weight: 70
url: /sv/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Alternativ för att ladda [GzipArchive](../../com.aspose.zip/gziparchive).

I .NET Framework 4.0 och senare kan den användas för att avbryta extrahering.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Hämtar värdet som indikerar om strömhuvudet ska analyseras för att fastställa egenskaper, inklusive namn. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Ställer in värdet som indikerar om strömhuvudet ska analyseras för att fastställa egenskaper, inklusive namn. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Hämtar värdet som indikerar om strömhuvudet ska analyseras för att fastställa egenskaper, inklusive namn. Gäller endast för sökbara strömmar.

**Returns:**
boolean - värdet som indikerar om strömhuvudet ska analyseras för att fastställa egenskaper, inklusive namn.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen.

Avbryt extrahering av gzip-arkiv efter en viss tid.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive(\"big.gz\", options)) {
try {
a.extract(\"data.bin\");
} catch (OperationCanceledException e) {
System.out.println("Extraheringen avbröts efter 60 sekunder");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

