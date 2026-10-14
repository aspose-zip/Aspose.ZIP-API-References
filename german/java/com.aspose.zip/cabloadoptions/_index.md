---
title: "CabLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird."
type: docs
weight: 48
url: /de/java/com.aspose.zip/cabloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class CabLoadOptions
```

Optionen, mit denen das Archiv aus einer komprimierten Datei geladen wird.

Ermöglicht das Abbrechen der Extraktion für .NET Framework 4.0 und höher.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [CabLoadOptions()](#CabLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
### CabLoadOptions() {#CabLoadOptions--}
```
public CabLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen.

CAB-Archiv-Extraktion nach einer bestimmten Zeit abbrechen.

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

