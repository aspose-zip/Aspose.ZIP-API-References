---
title: "WimEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 wim 镜像中的单个文件或目录。"
type: docs
weight: 132
url: /zh/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

表示 wim 镜像中的单个文件或目录。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | 获取文件或目录的备用数据流的名称。 |
| [getArchive()](#getArchive--) | 获取条目所属的存档。 |
| [getChangeTime()](#getChangeTime--) | 获取文件或目录上次更改的时间。 |
| [getCreationTime()](#getCreationTime--) | 获取文件或目录的创建时间。 |
| [getFileAttributes()](#getFileAttributes--) | 获取文件或目录的属性。 |
| [getFullPath()](#getFullPath--) | 获取条目在映像中的完整路径。 |
| [getHardLink()](#getHardLink--) | 获取文件或目录的硬链接 ID。 |
| [getImage()](#getImage--) | 获取条目所属的映像。 |
| [getLastAccessTime()](#getLastAccessTime--) | 获取文件或目录的最近访问时间。 |
| [getLastWriteTime()](#getLastWriteTime--) | 获取文件或目录的修改时间。 |
| [getModificationTime()](#getModificationTime--) | 获取文件或目录的修改时间。 |
| [getName()](#getName--) | 获取条目在映像中的名称。 |
| [getParent()](#getParent--) | 获取条目所属的父目录。 |
| [getShortName()](#getShortName--) | 获取条目在映像中的短名称。 |
| [hasHardLinks()](#hasHardLinks--) | 获取文件或目录是否有其他别名。 |
| [isDirectory()](#isDirectory--) | 获取指示该条目是否为目录的值。 |
| [toString()](#toString--) | 返回 [WimEntry](../../com.aspose.zip/wimentry) 类实例的字符串表示形式。 |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


获取文件或目录的备用数据流的名称。

**Returns:**
java.lang.String[] - 文件或目录的备用数据流的名称
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


获取条目所属的存档。

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


获取文件或目录上次更改的时间。

**Returns:**
java.util.Date - 文件或目录最后一次更改的时间
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


获取文件或目录的创建时间。

**Returns:**
java.util.Date - 文件或目录的创建时间
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


获取文件或目录的属性。

**Returns:**
int - 文件或目录的属性
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


获取条目在映像中的完整路径。

**Returns:**
java.lang.String - 镜像内条目的完整路径
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


获取文件或目录的硬链接 ID。

**Returns:**
long - 文件或目录的硬链接 ID
### getImage() {#getImage--}
```
public final WimImage getImage()
```


获取条目所属的映像。

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


获取文件或目录的最近访问时间。

**Returns:**
java.util.Date - 文件或目录的最后访问时间
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


获取文件或目录的修改时间。

**Returns:**
java.util.Date - 文件或目录的修改时间
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


获取文件或目录的修改时间。

**Returns:**
java.util.Date - 文件或目录的修改时间
### getName() {#getName--}
```
public final String getName()
```


获取条目在映像中的名称。

**Returns:**
java.lang.String - 镜像内条目的名称
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


获取条目所属的父目录。

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


获取条目在映像中的短名称。

**Returns:**
java.lang.String - 镜像内条目的短名称
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


获取文件或目录是否有其他别名。

**Returns:**
boolean - 文件或目录是否有其他别名
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


获取指示该条目是否为目录的值。

**Returns:**
boolean - 表示该条目是否为目录的值
### toString() {#toString--}
```
public String toString()
```


返回 [WimEntry](../../com.aspose.zip/wimentry) 类实例的字符串表示形式。

**Returns:**
java.lang.String - 此对象的字符串表示
