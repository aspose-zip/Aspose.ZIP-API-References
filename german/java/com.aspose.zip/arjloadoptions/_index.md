---
title: "ArjLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird."
type: docs
weight: 39
url: /de/java/com.aspose.zip/arjloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArjLoadOptions
```

Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird.

Im .NET Framework 4.0 und höher kann es verwendet werden, um die Extraktion abzubrechen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ArjLoadOptions()](#ArjLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
### ArjLoadOptions() {#ArjLoadOptions--}
```
public ArjLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen.

ARJ-Archivextraktion nach einer bestimmten Zeit abbrechen.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
ArjLoadOptions options = new ArjLoadOptions();
options.setCancellationFlag(cf);
try (ArjArchive a = new ArjArchive("big.arj", options)) {
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

