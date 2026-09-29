---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Detta gränssnitt representerar en arkivfilspost."
type: docs
weight: 162
url: /sv/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Detta gränssnitt representerar en arkivfilspost.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getName()](#getName--) | Hämtar postens namn. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Extraherar posten till den angivna strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | destinationsström. Måste vara skrivbar |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Extraherar posten till filsystemet enligt den angivna sökvägen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

**Returns:**
java.io.File - java.io.File-instans som innehåller extraherade data
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Hämtar längden på posten i byte.

**Returns:**
java.lang.Long - längden på posten i byte
### getName() {#getName--}
```
public abstract String getName()
```


Hämtar postens namn.

Arkiv endast för komprimering, såsom gzip, bzip2, lzip, lzma, xz, z har namnet "File.bin" om inte ett annat namn kan hittas i rubrikerna.

**Returns:**
java.lang.String - postens namn
