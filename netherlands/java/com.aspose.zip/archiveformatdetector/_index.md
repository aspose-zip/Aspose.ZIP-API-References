---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Detecteert een archiefformaat en biedt andere gerelateerde informatie."
type: docs
weight: 32
url: /nl/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Detecteert een archiefformaat en biedt andere gerelateerde informatie.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Initialiseert een nieuw exemplaar van de [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Haalt formatinformatie op. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Haalt formatinformatie op. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Initialiseert een nieuw exemplaar van de [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) klasse.

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Haalt formatinformatie op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.InputStream | De stroom van het archiefbestand. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Haalt formatinformatie op.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | De bestandsnaam van het archiefbestand. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
