---
title: "XarEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 xar 存档中的单个条目。"
type: docs
weight: 140
url: /zh/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

表示 xar 存档中的单个条目。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | 获取文件或目录的创建时间。 |
| [getFullPath()](#getFullPath--) | 获取存档中条目的完整路径。 |
| [getLastAccessTime()](#getLastAccessTime--) | 获取文件或目录的最近访问时间。 |
| [getLastWriteTime()](#getLastWriteTime--) | 获取文件或目录的修改时间。 |
| [getModificationTime()](#getModificationTime--) | 获取文件或目录的修改时间。 |
| [getName()](#getName--) | 获取存档中条目的名称。 |
| [getParent()](#getParent--) | 获取条目所属的父目录。 |
| [isDirectory()](#isDirectory--) | 获取指示该条目是否为目录的值。 |
| [toString()](#toString--) | 返回 [XarEntry](../../com.aspose.zip/xarentry) 类实例的字符串表示形式。 |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


获取文件或目录的创建时间。

**Returns:**
java.util.Date - 文件或目录的创建时间
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


获取存档中条目的完整路径。

**Returns:**
java.lang.String - 存档中条目的完整路径
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


获取存档中条目的名称。

**Returns:**
java.lang.String - 存档中条目的名称
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


获取条目所属的父目录。

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
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


返回 [XarEntry](../../com.aspose.zip/xarentry) 类实例的字符串表示形式。

**Returns:**
java.lang.String - 此对象的字符串表示
