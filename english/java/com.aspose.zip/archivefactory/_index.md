---
title: ArchiveFactory
second_title: Aspose.ZIP for Java API Reference
description: Detects the archive format and creates the appropriate  object according to the type of archive.
type: docs
weight: 16
url: /java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive.
## Methods

| Method | Description |
| --- | --- |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given stream. |
| [getArchive(String path)](#getArchive-java.lang.String-) | Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given path. |
### getArchive(InputStream stream) {#getArchive-java.io.InputStream-}
```
public static IArchive getArchive(InputStream stream)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream containing the archive data. It must bee seekable. |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - An [IArchive](../../com.aspose.zip/iarchive) object representing the archive.
### getArchive(String path) {#getArchive-java.lang.String-}
```
public static IArchive getArchive(String path)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive to be analyzed. |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - An [IArchive](../../com.aspose.zip/iarchive) object representing the archive.
