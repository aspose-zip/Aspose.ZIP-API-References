---
title: AppleArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents an Apple Archive .aar file.
type: docs
weight: 16
url: /java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

This class represents an Apple Archive (.aar) file. Use it to compose Apple Archive files.

Apple and Apple Archive are trademarks of Apple Inc.
## Constructors

| Constructor | Description |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class with settings used for composed entries. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class with settings used for composed entries. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Adds to the archive all files and directories recursively in the directory given. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Adds to the archive all files and directories recursively in the directory given. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Creates a single entry within the archive. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Creates a single entry within the archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Creates a single entry within the archive. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Creates a single entry within the archive. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Creates a single entry within the archive. |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts all the files in the archive to the directory provided. |
| [getEntries()](#getEntries--) | Gets entries constituting the archive. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive. |
| [getFormat()](#getFormat--) | Gets the archive format. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Gets settings used for newly composed entries. |
| [isSolid()](#isSolid--) | Gets a value indicating whether the archive uses solid compression. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Saves archive to the stream provided. |
| [save(String destinationFileName)](#save-java.lang.String-) | Saves archive to a destination file provided. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class with settings used for composed entries.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class with settings used for composed entries.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Settings used when composing a new Apple Archive. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive.

This constructor does not decompress any entry. See [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) and [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) methods for decompressing. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Options to load existing archive with.

This constructor does not decompress any entry. See [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) and [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) methods for decompressing. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file.

This constructor does not decompress any entry. See [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) and [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) methods for decompressing. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [AppleArchive](../../com.aspose.zip/applearchive) class and composes an entry list can be extracted from the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Options to load existing archive with.

This constructor does not decompress any entry. See [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) and [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) methods for decompressing. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Adds to the archive all files and directories recursively in the directory given.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory itself or not. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Creates a single entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| fileInfo | java.io.File | The metadata of file to be compressed. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Creates a single entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| fileInfo | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The path to the file to compress. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The path to the file to compress. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Gets entries constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - entries constituting the archive.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Gets settings used for newly composed entries.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Gets a value indicating whether the archive uses solid compression. In solid mode, all entry data is compressed as a single stream and individual entry extraction is not available. Use [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) instead.

**Returns:**
boolean - a value indicating whether the archive uses solid compression.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves archive to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream.

`output` must be writable. Some compression settings, such as LZ4, also require a seekable stream. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to a destination file provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. |

