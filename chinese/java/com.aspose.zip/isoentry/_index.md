---
title: "IsoEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 ISO 存档中的条目文件或目录。"
type: docs
weight: 72
url: /zh/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

表示 ISO 存档中的条目（文件或目录）。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getLength()](#getLength--) | 获取条目的长度。 |
| [getModificationTime()](#getModificationTime--) | 获取最后修改的日期和时间。 |
| [getName()](#getName--) | 获取条目的名称。 |
| [isDirectory()](#isDirectory--) | 获取一个值，指示条目是否为目录。 |
| [toString()](#toString--) | 返回一个表示当前条目的字符串。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


将条目提取到提供的流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流 |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


根据提供的路径将条目提取到文件系统中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖 |

**Returns:**
java.io.File - 包含提取数据的 java.io.File 实例
### getLength() {#getLength--}
```
public Long getLength()
```


获取条目的长度。

**Returns:**
java.lang.Long - 条目的长度
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


获取最后修改的日期和时间。

**Returns:**
java.util.Date - 最后修改的日期和时间
### getName() {#getName--}
```
public final String getName()
```


获取条目的名称。

**Returns:**
java.lang.String - 条目的名称
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


获取一个值，指示条目是否为目录。

**Returns:**
boolean - 表示该条目是否为目录的值
### toString() {#toString--}
```
public String toString()
```


返回一个表示当前条目的字符串。

**Returns:**
java.lang.String - 条目的名称
