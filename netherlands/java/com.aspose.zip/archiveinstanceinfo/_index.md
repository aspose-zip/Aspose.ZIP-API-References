---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt informatie over de archiefinstantie voor."
type: docs
weight: 34
url: /nl/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Stelt informatie over de archiefinstantie voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Haalt een waarde op die aangeeft of de namen van items (bestanden) in het archief versleuteld zijn. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Haalt informatie over het archiefformaat op. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Haalt informatie over het archiefformaat op. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Haalt informatie over de archiefinstantie op. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Haalt informatie over de archiefinstantie op. |
| [getFormatInfo()](#getFormatInfo--) | Haalt de informatie over het archiefformaat op. |
| [isContentEncrypted()](#isContentEncrypted--) | Haalt een waarde op die aangeeft of de inhoud van het archief versleuteld is. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Haalt een waarde op die aangeeft of de namen van items (bestanden) in het archief versleuteld zijn.

**Returns:**
boolean - een waarde die aangeeft of de namen van de items (bestanden) van het archief versleuteld zijn.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Haalt informatie over het archiefformaat op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | De stroom van het archiefbestand. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Haalt informatie over het archiefformaat op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De bestandsnaam van het archiefbestand. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Haalt informatie over de archiefinstantie op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | De stroom van het archiefbestand. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Haalt informatie over de archiefinstantie op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De bestandsnaam van het archiefbestand. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Haalt de informatie over het archiefformaat op.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Haalt een waarde op die aangeeft of de inhoud van het archief versleuteld is.

**Returns:**
boolean - een waarde die aangeeft of de inhoud van het archief versleuteld is.
