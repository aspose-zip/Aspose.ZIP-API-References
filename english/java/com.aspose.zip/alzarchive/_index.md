---
title: AlzArchive
second_title: Aspose.ZIP for Java API Reference
description: Represents an ALZ archive file.
type: docs
weight: 11
url: /java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Represents an ALZ archive file. Use this class to inspect and extract ALZ archives.
## Constructors

| Constructor | Description |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Initializes an ALZ archive from a stream. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Initializes an ALZ archive from a stream using the supplied load options. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Initializes an ALZ archive from a file path. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Initializes an ALZ archive from a file path using the supplied load options. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | Releases resources held by this archive. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts all files and directories to the supplied directory. |
| [getEntries()](#getEntries--) | Gets the entries constituting this archive. |
| [getFileEntries()](#getFileEntries--) | Gets entries through the common archive interface. |
| [getFormat()](#getFormat--) | Gets the archive format. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Initializes an ALZ archive from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | ALZ archive stream; it must support reading and seeking |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Initializes an ALZ archive from a stream using the supplied load options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | ALZ archive stream; it must support reading and seeking |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | options used to load the archive |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Initializes an ALZ archive from a file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | path to an ALZ archive |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Initializes an ALZ archive from a file path using the supplied load options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | path to an ALZ archive |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | options used to load the archive |

### close() {#close--}
```
public void close()
```


Releases resources held by this archive.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all files and directories to the supplied directory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | destination directory; it is created when necessary |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Gets the entries constituting this archive.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - immutable list of ALZ entries
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries through the common archive interface.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - archive entries
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
