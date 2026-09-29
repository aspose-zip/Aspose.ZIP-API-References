---
title: "GzipLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het laden."
type: docs
weight: 70
url: /nl/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

Opties voor het laden van [GzipArchive](../../com.aspose.zip/gziparchive).

In het .NET Framework 4.0 en hoger kan dit worden gebruikt om extractie te annuleren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | Haalt de waarde op die aangeeft of de streamheader moet worden geparseerd om eigenschappen te bepalen, inclusief naam. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | Stelt de waarde in die aangeeft of de streamheader moet worden geparseerd om eigenschappen te bepalen, inclusief naam. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


Haalt de waarde op die aangeeft of de streamheader moet worden geparseerd om eigenschappen te bepalen, inclusief naam. Heeft alleen zin voor een seekbare stream.

**Returns:**
boolean - de waarde die aangeeft of de streamheader moet worden geparseerd om eigenschappen te bepalen, inclusief naam.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Stelt een annuleringsvlag in die wordt gebruikt om de extractie‑bewerking te annuleren.

Annuleer het uitpakken van een gzip‑archief na een bepaalde tijd.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive(\"big.gz\", options)) {
try {
a.extract(\"data.bin\");
} catch (OperationCanceledException e) {
System.out.println(\"Extractie werd geannuleerd na 60 seconden\");
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

