---
title: IsoEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents an entry file or directory within an ISO archive.
type: docs
weight: 46
url: /java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Represents an entry (file or directory) within an ISO archive.
## Methods

| Method | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts the entry to the filesystem by the path provided. |
| [getLength()](#getLength--) | Gets the length of the entry. |
| [getName()](#getName--) | Gets the name of the entry. |
| [isDirectory()](#isDirectory--) | Gets a value indicating whether the entry is a directory. |
| [toString()](#toString--) | Returns a string that represents the current entry. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### getLength() {#getLength--}
```
public Long getLength()
```


Gets the length of the entry.

**Returns:**
java.lang.Long - the length of the entry
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

**Returns:**
java.lang.String - the name of the entry
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry is a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### toString() {#toString--}
```
public String toString()
```


Returns a string that represents the current entry.

**Returns:**
java.lang.String - a string that represents the current entry
