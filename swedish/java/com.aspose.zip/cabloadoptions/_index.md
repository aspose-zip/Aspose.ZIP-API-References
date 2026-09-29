---
title: "CabLoadOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ med vilka arkivet laddas från en komprimerad fil."
type: docs
weight: 48
url: /sv/java/com.aspose.zip/cabloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class CabLoadOptions
```

Alternativ med vilka arkivet laddas från en komprimerad fil.

Tillåter att avbryta extrahering för .NET Framework 4.0 och senare.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [CabLoadOptions()](#CabLoadOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen. |
### CabLoadOptions() {#CabLoadOptions--}
```
public CabLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen.

Avbryt CAB-arkivextrahering efter en viss tid.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
CabLoadOptions options = new CabLoadOptions();
options.setCancellationFlag(cf);
try (CabArchive a = new CabArchive("big.cab", options)) {
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

