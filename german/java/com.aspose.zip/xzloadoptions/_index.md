---
title: "XzLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Laden ."
type: docs
weight: 152
url: /de/java/com.aspose.zip/xzloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XzLoadOptions
```

Optionen zum Laden von [XzArchive](../../com.aspose.zip/xzarchive).

Im .NET Framework 4.0 und höher kann es verwendet werden, um die Extraktion abzubrechen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [XzLoadOptions()](#XzLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
### XzLoadOptions() {#XzLoadOptions--}
```
public XzLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen.

Lzip-Archivextraktion nach einer bestimmten Zeit abbrechen.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
XzLoadOptions options = new XzLoadOptions();
options.setCancellationFlag(cf);
try (XzArchive a = new XzArchive("big.xz", options)) {
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

