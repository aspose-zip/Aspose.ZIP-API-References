---
title: "IsoEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en postfil eller katalog i ett ISO-arkiv."
type: docs
weight: 72
url: /sv/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Representerar en post (fil eller katalog) i ett ISO-arkiv.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getLength()](#getLength--) | Hämtar postens längd. |
| [getModificationTime()](#getModificationTime--) | Hämtar senaste ändringsdatum och -tid. |
| [getName()](#getName--) | Hämtar postens namn. |
| [isDirectory()](#isDirectory--) | Hämtar ett värde som indikerar om posten är en katalog. |
| [toString()](#toString--) | Returnerar en sträng som representerar den aktuella posten. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | målström |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Extraherar posten till filsystemet enligt den angivna sökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till målfilen. Om filen redan finns kommer den att skrivas över |

**Returns:**
java.io.File - java.io.File-instans som innehåller extraherade data
### getLength() {#getLength--}
```
public Long getLength()
```


Hämtar postens längd.

**Returns:**
java.lang.Long - postens längd
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Hämtar senaste ändringsdatum och -tid.

**Returns:**
java.util.Date - senaste ändringsdatum och tid
### getName() {#getName--}
```
public final String getName()
```


Hämtar postens namn.

**Returns:**
java.lang.String - postens namn
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Hämtar ett värde som indikerar om posten är en katalog.

**Returns:**
boolean - ett värde som indikerar om posten representerar en katalog
### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar den aktuella posten.

**Returns:**
java.lang.String - postens namn
