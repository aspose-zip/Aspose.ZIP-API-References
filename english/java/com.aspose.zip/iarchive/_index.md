---
title: IArchive
second_title: Aspose.ZIP for Java API Reference
description: This interface represents an archive.
type: docs
weight: 74
url: /java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
com.aspose.ms.System.IDisposable
```
public interface IArchive extends System.IDisposable
```

This interface represents an archive.
## Methods

| Method | Description |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts all the files in the archive to the directory provided. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z consist of the single record - the archive itself.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.
