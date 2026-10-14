---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Laden ."
type: docs
weight: 70
url: /de/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Optionen zum Laden [GzipArchive](../../com.aspose.zip/gziparchive).

Im .NET Framework 4.0 und höher kann es verwendet werden, um die Extraktion abzubrechen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Liefert den Wert, der angibt, ob der Stream-Header geparst werden soll, um Eigenschaften, einschließlich des Namens, zu ermitteln. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Setzt den Wert, der angibt, ob der Stream-Header geparst werden soll, um Eigenschaften, einschließlich des Namens, zu ermitteln. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Liefert den Wert, der angibt, ob der Stream-Header geparst werden soll, um Eigenschaften, einschließlich des Namens, zu ermitteln. Sinnvoll nur für einen seekbaren Stream.

**Returns:**
boolean - der Wert, der angibt, ob der Stream-Header geparst werden soll, um Eigenschaften, einschließlich des Namens, zu ermitteln.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das verwendet wird, um den Extraktionsvorgang abzubrechen.

Brechen Sie die Extraktion des Gzip-Archivs nach einer bestimmten Zeit ab.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
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

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

