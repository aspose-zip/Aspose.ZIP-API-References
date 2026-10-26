---
title: EggArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents an EGG archive file.
type: docs
weight: 59
url: /java/com.aspose.zip/eggarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class EggArchive implements IArchive, AutoCloseable
```

This class represents an EGG archive file. Use it to extract EGG archives.
## Constructors

| Constructor | Description |
| --- | --- |
| [EggArchive(InputStream stream)](#EggArchive-java.io.InputStream-) | Initializes an EGG archive from a stream. |
| [EggArchive(InputStream stream, EggArchiveLoadOptions loadOptions)](#EggArchive-java.io.InputStream-com.aspose.zip.EggArchiveLoadOptions-) | Initializes an EGG archive from a stream. |
| [EggArchive(String path)](#EggArchive-java.lang.String-) | Initializes an EGG archive from a file path. |
| [EggArchive(String path, EggArchiveLoadOptions loadOptions)](#EggArchive-java.lang.String-com.aspose.zip.EggArchiveLoadOptions-) | Initializes an EGG archive from a file path. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | Releases all resources used by this archive. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts archived files to the provided directory. |
| [getComment()](#getComment--) | Gets the comment for the whole archive. |
| [getEntries()](#getEntries--) | Gets the list of files in the archive. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive. |
| [getFormat()](#getFormat--) | Gets the archive format. |
### EggArchive(InputStream stream) {#EggArchive-java.io.InputStream-}
```
public EggArchive(InputStream stream)
```


Initializes an EGG archive from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | EGG archive stream; it must support reading and seeking. |

### EggArchive(InputStream stream, EggArchiveLoadOptions loadOptions) {#EggArchive-java.io.InputStream-com.aspose.zip.EggArchiveLoadOptions-}
```
public EggArchive(InputStream stream, EggArchiveLoadOptions loadOptions)
```


Initializes an EGG archive from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | EGG archive stream; it must support reading and seeking. |
| loadOptions | [EggArchiveLoadOptions](../../com.aspose.zip/eggarchiveloadoptions) | options to load the archive with. |

### EggArchive(String path) {#EggArchive-java.lang.String-}
```
public EggArchive(String path)
```


Initializes an EGG archive from a file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to the EGG archive file. |

### EggArchive(String path, EggArchiveLoadOptions loadOptions) {#EggArchive-java.lang.String-com.aspose.zip.EggArchiveLoadOptions-}
```
public EggArchive(String path, EggArchiveLoadOptions loadOptions)
```


Initializes an EGG archive from a file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to the EGG archive file. |
| loadOptions | [EggArchiveLoadOptions](../../com.aspose.zip/eggarchiveloadoptions) | options to load the archive with. |

### close() {#close--}
```
public final void close()
```


Releases all resources used by this archive.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts archived files to the provided directory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | path to the directory in which to place the extracted files. |

### getComment() {#getComment--}
```
public final String getComment()
```


Gets the comment for the whole archive.

**Returns:**
java.lang.String - comment for the whole archive.
### getEntries() {#getEntries--}
```
public final List<EggEntry> getEntries()
```


Gets the list of files in the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.EggEntry&gt; - immutable list of files in the archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Egg](../../com.aspose.zip/archiveformat\#Egg).
