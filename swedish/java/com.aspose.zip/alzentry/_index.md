---
title: "AlzEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar en filpost i ett ALZ-arkiv tillsammans med dess metadata."
type: docs
weight: 13
url: /sv/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Representerar en filpost i ett ALZ-arkiv tillsammans med dess metadata.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar posten till en skrivbar ström. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extraherar posten till en skrivbar ström med ett valfritt lösenord. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar posten till den angivna filen. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extraherar posten till den angivna filen med ett valfritt lösenord. |
| [getCompressedSize()](#getCompressedSize--) | Hämtar den komprimerade storleken på postens data i byte. |
| [getLength()](#getLength--) | Hämtar den dekomprimerade längden på den här posten. |
| [getName()](#getName--) | Hämtar postens namn som lagras i arkivet. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar den dekomprimerade storleken på postens data i byte. |
| [isDirectory()](#isDirectory--) | Hämtar om den här posten representerar en katalog. |
| [open()](#open--) | Öppnar posten och tillhandahåller en ström som innehåller dekomprimerad data. |
| [open(String password)](#open-java.lang.String-) | Öppnar posten och tillhandahåller en ström som innehåller dekomprimerad data. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar posten till en skrivbar ström.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | målström |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extraherar posten till en skrivbar ström med ett valfritt lösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | målström |
| lösenord | java.lang.String | valfritt lösenord för den här posten |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar posten till den angivna filen. En befintlig fil skrivs över.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | destinationsfilens sökväg |

**Returns:**
java.io.File - extraherad fil
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extraherar posten till den angivna filen med ett valfritt lösenord.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | destinationsfilens sökväg |
| lösenord | java.lang.String | valfritt lösenord för den här posten |

**Returns:**
java.io.File - extraherad fil
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Hämtar den komprimerade storleken på postens data i byte.

**Returns:**
long - komprimerad storlek i byte
### getLength() {#getLength--}
```
public final Long getLength()
```


Hämtar den dekomprimerade längden på den här posten.

**Returns:**
java.lang.Long - okomprimerad längd i byte
### getName() {#getName--}
```
public final String getName()
```


Hämtar postens namn som lagras i arkivet.

**Returns:**
java.lang.String - postnamn
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Hämtar den dekomprimerade storleken på postens data i byte.

**Returns:**
long - okomprimerad storlek i byte
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Hämtar om den här posten representerar en katalog.

**Returns:**
boolean - `true` för ett kataloginlägg
### open() {#open--}
```
public final InputStream open()
```


Öppnar posten och tillhandahåller en ström som innehåller dekomprimerad data.

**Returns:**
java.io.InputStream - ström som innehåller dekomprimerad postdata
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Öppnar posten och tillhandahåller en ström som innehåller dekomprimerad data.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| lösenord | java.lang.String | valfritt lösenord för den här posten |

**Returns:**
java.io.InputStream - ström som innehåller dekomprimerad postdata
