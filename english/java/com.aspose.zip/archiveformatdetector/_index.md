---
title: ArchiveFormatDetector
second_title: Aspose.ZIP for Java API Reference
description: Detects an archive format and provides other related information.
type: docs
weight: 17
url: /java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Detects an archive format and provides other related information.
## Constructors

| Constructor | Description |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Initializes a new instance of the [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) class. |
## Methods

| Method | Description |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Gets format info. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Gets format info. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Initializes a new instance of the [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) class.

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Gets format info.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream of the archive file. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Gets format info.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The filename of the archive file. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
