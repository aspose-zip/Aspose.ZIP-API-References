---
title: AlzEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents a file entry in an ALZ archive together with its metadata.
type: docs
weight: 13
url: /java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Represents a file entry in an ALZ archive together with its metadata.
## Methods

| Method | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to a writable stream. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extracts the entry to a writable stream using an optional password. |
| [extract(String path)](#extract-java.lang.String-) | Extracts the entry to the specified file. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extracts the entry to the specified file using an optional password. |
| [getCompressedSize()](#getCompressedSize--) | Gets the compressed size of the entry data in bytes. |
| [getLength()](#getLength--) | Gets the uncompressed length of this entry. |
| [getName()](#getName--) | Gets the entry name stored in the archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Gets the uncompressed size of the entry data in bytes. |
| [isDirectory()](#isDirectory--) | Gets whether this entry represents a directory. |
| [open()](#open--) | Opens the entry and provides a stream containing decompressed data. |
| [open(String password)](#open-java.lang.String-) | Opens the entry and provides a stream containing decompressed data. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to a writable stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to a writable stream using an optional password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |
| password | java.lang.String | optional password for this entry |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the specified file. An existing file is overwritten.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | destination file path |

**Returns:**
java.io.File - extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the specified file using an optional password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | destination file path |
| password | java.lang.String | optional password for this entry |

**Returns:**
java.io.File - extracted file
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets the compressed size of the entry data in bytes.

**Returns:**
long - compressed size in bytes
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of this entry.

**Returns:**
java.lang.Long - uncompressed length in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the entry name stored in the archive.

**Returns:**
java.lang.String - entry name
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the entry data in bytes.

**Returns:**
long - uncompressed size in bytes
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets whether this entry represents a directory.

**Returns:**
boolean - `true` for a directory entry
### open() {#open--}
```
public final InputStream open()
```


Opens the entry and provides a stream containing decompressed data.

**Returns:**
java.io.InputStream - stream containing decompressed entry data
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Opens the entry and provides a stream containing decompressed data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for this entry |

**Returns:**
java.io.InputStream - stream containing decompressed entry data
