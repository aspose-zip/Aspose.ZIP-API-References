---
title: "LzxLoadOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ med vilka arkivet laddas från en komprimerad fil."
type: docs
weight: 91
url: /sv/java/com.aspose.zip/lzxloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzxLoadOptions
```

Alternativ med vilka arkivet laddas från en komprimerad fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LzxLoadOptions()](#LzxLoadOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen. |
### LzxLoadOptions() {#LzxLoadOptions--}
```
public LzxLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen.

Avbryt ISO-arkivextraktion efter en viss tid.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzxLoadOptions options = new LzxLoadOptions();
options.setCancellationFlag(cf);
try (LzxArchive a = new LzxArchive("big.lzx", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

