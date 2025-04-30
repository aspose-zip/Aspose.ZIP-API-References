---
title: XarEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents a single entry within xar archive.
type: docs
weight: 104
url: /java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

Represents a single entry within xar archive.
## Methods

| Method | Description |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | Gets the creation time of the file or directory. |
| [getFullPath()](#getFullPath--) | Gets the full path of the entry within the archive. |
| [getLastAccessTime()](#getLastAccessTime--) | Gets the last access time of the file or directory. |
| [getLastWriteTime()](#getLastWriteTime--) | Gets the modification time of the file or directory. |
| [getModificationTime()](#getModificationTime--) | Gets the modification time of the file or directory. |
| [getName()](#getName--) | Gets the name of the entry within the archive. |
| [getParent()](#getParent--) | Gets the parent directory the entry belongs to. |
| [isDirectory()](#isDirectory--) | Gets a value indicating whether the entry represents a directory. |
| [toString()](#toString--) | Returns string representation of the instance of the [XarEntry](../../com.aspose.zip/xarentry) class. |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Gets the creation time of the file or directory.

**Returns:**
java.util.Date - the creation time of the file or directory
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Gets the full path of the entry within the archive.

**Returns:**
java.lang.String - the full path of the entry within the archive
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets the last access time of the file or directory.

**Returns:**
java.util.Date - the last access time of the file or directory
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Gets the modification time of the file or directory.

**Returns:**
java.util.Date - the modification time of the file or directory
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the modification time of the file or directory.

**Returns:**
java.util.Date - the modification time of the file or directory
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


Gets the parent directory the entry belongs to.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [XarEntry](../../com.aspose.zip/xarentry) class.

**Returns:**
java.lang.String - string representation of this object
