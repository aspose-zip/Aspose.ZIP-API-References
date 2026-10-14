---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze interface vertegenwoordigt een archiefbestandvermelding."
type: docs
weight: 162
url: /nl/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Deze interface vertegenwoordigt een archiefbestandvermelding.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het item naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het item naar het bestandssysteem via het opgegeven pad. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [getName()](#getName--) | Haalt de naam van het item op. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Extraheert het item naar de opgegeven stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | doelstream. Moet beschrijfbaar zijn. |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Extraheert het item naar het bestandssysteem via het opgegeven pad.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |

**Returns:**
java.io.File - java.io.File‑instantie die geëxtraheerde gegevens bevat
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Haalt de lengte van het item op in bytes.

**Returns:**
java.lang.Long - de lengte van het item in bytes
### getName() {#getName--}
```
public abstract String getName()
```


Haalt de naam van het item op.

Archieven alleen voor compressie, zoals gzip, bzip2, lzip, lzma, xz, z, hebben de naam "File.bin" tenzij een andere naam in de headers kan worden gevonden.

**Returns:**
java.lang.String - de naam van de entry
