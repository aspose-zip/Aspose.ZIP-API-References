---
title: IArchiveFileEntry
second_title: Aspose.ZIP for Java API Reference
description: This interface represents an archive file entry.
type: docs
weight: 42
url: /java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

This interface represents an archive file entry.
## Methods

| Method | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts the entry to the filesystem by the path provided. |
| [getLength()](#getLength--) | Gets the length of the entry in bytes. |
| [getName()](#getName--) | Gets name of the entry. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - FileInfo instance containing extracted data.
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes.
### getName() {#getName--}
```
public abstract String getName()
```


Gets name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - name of the entry.
