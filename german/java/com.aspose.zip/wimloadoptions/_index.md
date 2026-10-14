---
title: "WimLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird."
type: docs
weight: 135
url: /de/java/com.aspose.zip/wimloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class WimLoadOptions
```

Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WimLoadOptions()](#WimLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
### WimLoadOptions() {#WimLoadOptions--}
```
public WimLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen.

WIM-Archivextraktion nach einer bestimmten Zeit abbrechen.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
WimLoadOptions options = new WimLoadOptions();
options.setCancellationFlag(cf);
try (WimArchive a = new WimArchive("big.wim", options)) {
try {
StreamSupport.stream(a.getImages().get(0).getAllEntries().spliterator(), false)
.filter(entry -> entry instanceof WimFileEntry)
.map(entry -> (WimFileEntry) entry)
.findFirst().ifPresent(entry -> entry.extract("data.bin"));
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

