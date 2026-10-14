---
title: "LzxLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird."
type: docs
weight: 91
url: /de/java/com.aspose.zip/lzxloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzxLoadOptions
```

Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LzxLoadOptions()](#LzxLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
### LzxLoadOptions() {#LzxLoadOptions--}
```
public LzxLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen.

ISO-Archivextraktion nach einer bestimmten Zeit abbrechen.

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

