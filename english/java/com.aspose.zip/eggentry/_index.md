---
title: EggEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents a file entry in an EGG archive with all its metadata.
type: docs
weight: 61
url: /java/com.aspose.zip/eggentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class EggEntry implements IArchiveFileEntry
```

Represents a file entry in an EGG archive with all its metadata.
## Methods

| Method | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts the entry to a file. |
| [getCompressedSize()](#getCompressedSize--) | Gets the compressed size of the entry. |
| [getLength()](#getLength--) | Gets the uncompressed length of the entry. |
| [getModificationTime()](#getModificationTime--) | Gets the last modified date and time. |
| [getName()](#getName--) | Gets the name of the entry within the archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Gets the uncompressed size of the entry. |
| [isDirectory()](#isDirectory--) | Gets a value indicating whether this entry represents a directory. |
| [open()](#open--) | Opens the entry for extraction and provides a stream with decompressed entry content. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to a file. An existing file is overwritten.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | destination file path. |

**Returns:**
java.io.File - extracted file.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets the compressed size of the entry.

**Returns:**
long - the compressed size of the entry.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry.

**Returns:**
java.lang.Long - the uncompressed length of the entry.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified date and time.

**Returns:**
java.util.Date - the last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive.
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the entry.

**Returns:**
long - the uncompressed size of the entry.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry represents a directory.

**Returns:**
boolean - `true` if this entry represents a directory; otherwise, `false`.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.

**Returns:**
java.io.InputStream - stream representing the contents of the entry.
