---
title: "XzLoadOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för att ladda ."
type: docs
weight: 152
url: /sv/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

Alternativ för att ladda [XzArchive](../../com.aspose.zip/xzarchive).

I .NET Framework 4.0 och senare kan den användas för att avbryta extrahering.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen. |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen.

Avbryt extrahering av lzip-arkivet efter en viss tid.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

