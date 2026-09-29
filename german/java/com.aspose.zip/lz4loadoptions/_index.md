---
title: "Lz4LoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Laden ."
type: docs
weight: 82
url: /de/java/com.aspose.zip/lz4loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Lz4LoadOptions
```

Optionen zum Laden von [Lz4Archive](../../com.aspose.zip/lz4archive).
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Lz4LoadOptions()](#Lz4LoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
### Lz4LoadOptions() {#Lz4LoadOptions--}
```
public Lz4LoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen.

Abbrechen der LZ4-Archivextraktion nach einer bestimmten Zeit.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
Lz4LoadOptions options = new Lz4LoadOptions();
options.setCancellationFlag(cf);
try (Lz4Archive a = new Lz4Archive("big.lz4", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("Extraktion wurde nach 60 Sekunden abgebrochen");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

