---
title: "Lz4LoadOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för att ladda ."
type: docs
weight: 82
url: /sv/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

Alternativ för att ladda [Lz4Archive](../../com.aspose.zip/lz4archive).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen. |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ställer in en avbrytningsflagga som används för att avbryta extraheringsoperationen.

Avbryt extrahering av lz4-arkivet efter en viss tid.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive("big.lz4", options)) {
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

