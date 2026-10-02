---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar information om arkivinstansen."
type: docs
weight: 34
url: /sv/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Representerar information om arkivinstansen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Hämtar ett värde som indikerar om namnen på poster (filer) i arkivet är krypterade. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Hämtar information om arkivformatet. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Hämtar information om arkivformatet. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Hämtar information om arkivinstansen. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Hämtar information om arkivinstansen. |
| [getFormatInfo()](#getFormatInfo--) | Hämtar information om arkivformatet. |
| [isContentEncrypted()](#isContentEncrypted--) | Hämtar ett värde som indikerar om arkivets innehåll är krypterat. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Hämtar ett värde som indikerar om namnen på poster (filer) i arkivet är krypterade.

**Returns:**
boolean - ett värde som indikerar om namnen på poster (filer) i arkivet är krypterade.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Hämtar information om arkivformatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen för arkivfilen. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Hämtar information om arkivformatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamnet för arkivfilen. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Hämtar information om arkivinstansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen för arkivfilen. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Hämtar information om arkivinstansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamnet för arkivfilen. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Hämtar information om arkivformatet.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Hämtar ett värde som indikerar om arkivets innehåll är krypterat.

**Returns:**
boolean - ett värde som indikerar om arkivets innehåll är krypterat.
