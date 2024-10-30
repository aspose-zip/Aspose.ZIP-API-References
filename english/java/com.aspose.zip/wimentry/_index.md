---
title: WimEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents single file or directory within wim image.
type: docs
weight: 90
url: /java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Represents single file or directory within wim image.
## Methods

| Method | Description |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Gets the names of the alternate data streams for the file or directory. |
| [getArchive()](#getArchive--) | Gets the archive the entry belongs to. |
| [getChangeTime()](#getChangeTime--) | Gets the last time the file or directory was changed. |
| [getCreationTime()](#getCreationTime--) | Gets the creation time of the file or directory. |
| [getFileAttributes()](#getFileAttributes--) | Gets the file or directory attributes. |
| [getFullPath()](#getFullPath--) | Gets the full path of the entry within the image. |
| [getHardLink()](#getHardLink--) | Gets the hardlink id of the file or directory. |
| [getImage()](#getImage--) | Gets the image the entry belongs to. |
| [getLastAccessTime()](#getLastAccessTime--) | Gets the last access time of the file or directory. |
| [getLastWriteTime()](#getLastWriteTime--) | Gets the modification time of the file or directory. |
| [getName()](#getName--) | Gets the name of the entry within the image. |
| [getParent()](#getParent--) | Gets the parent directory the entry belongs to. |
| [getShortName()](#getShortName--) | Gets the short name of the entry within the image. |
| [hasHardLinks()](#hasHardLinks--) | Gets whether the file or directory is known by other names. |
| [isDirectory()](#isDirectory--) | Gets a value indicating whether the entry represents a directory. |
| [toString()](#toString--) | Returns string representation of the instance of the [WimEntry](../../com.aspose.zip/wimentry) class. |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Gets the names of the alternate data streams for the file or directory.

**Returns:**
java.lang.String[] - the names of the alternate data streams for the file or directory
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Gets the archive the entry belongs to.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Gets the last time the file or directory was changed.

**Returns:**
java.util.Date - the last time the file or directory was changed
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Gets the creation time of the file or directory.

**Returns:**
java.util.Date - the creation time of the file or directory
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Gets the file or directory attributes.

**Returns:**
int - the file or directory attributes
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Gets the full path of the entry within the image.

**Returns:**
java.lang.String - the full path of the entry within the image
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Gets the hardlink id of the file or directory.

**Returns:**
long - the hardlink id of the file or directory
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Gets the image the entry belongs to.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
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
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the image.

**Returns:**
java.lang.String - the name of the entry within the image
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Gets the parent directory the entry belongs to.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Gets the short name of the entry within the image.

**Returns:**
java.lang.String - the short name of the entry within the image
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Gets whether the file or directory is known by other names.

**Returns:**
boolean - whether the file or directory is known by other names
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


Returns string representation of the instance of the [WimEntry](../../com.aspose.zip/wimentry) class.

**Returns:**
java.lang.String - string representation of this object
