---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP för Java API-referens"
description: "Detekterar ett arkivformat och tillhandahåller annan relaterad information."
type: docs
weight: 32
url: /sv/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Detekterar ett arkivformat och tillhandahåller annan relaterad information.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Initierar en ny instans av klassen [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Hämtar formatinformation. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Hämtar formatinformation. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Initierar en ny instans av klassen [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Hämtar formatinformation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.InputStream | Strömmen för arkivfilen. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Hämtar formatinformation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Filnamnet för arkivfilen. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
