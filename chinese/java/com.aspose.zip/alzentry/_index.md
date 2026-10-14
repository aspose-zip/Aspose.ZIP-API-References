---
title: "AlzEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 ALZ 存档中的文件条目以及其元数据。"
type: docs
weight: 13
url: /zh/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

表示 ALZ 存档中的文件条目以及其元数据。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到可写流中。 |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | 使用可选密码将条目提取到可写流中。 |
| [extract(String path)](#extract-java.lang.String-) | 将条目提取到指定文件。 |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | 使用可选密码将条目提取到指定文件。 |
| [getCompressedSize()](#getCompressedSize--) | 获取条目数据的压缩大小（字节）。 |
| [getLength()](#getLength--) | 获取此条目的未压缩长度。 |
| [getName()](#getName--) | 获取存档中存储的条目名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取条目数据的未压缩大小（字节）。 |
| [isDirectory()](#isDirectory--) | 获取此条目是否表示目录。 |
| [open()](#open--) | 打开条目并提供包含解压缩数据的流。 |
| [open(String password)](#open-java.lang.String-) | 打开条目并提供包含解压缩数据的流。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到可写流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流 |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


使用可选密码将条目提取到可写流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流 |
| password | java.lang.String | 此条目的可选密码 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


将条目提取到指定文件。现有文件将被覆盖。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件路径 |

**Returns:**
java.io.File - 已提取的文件
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


使用可选密码将条目提取到指定文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件路径 |
| password | java.lang.String | 此条目的可选密码 |

**Returns:**
java.io.File - 已提取的文件
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


获取条目数据的压缩大小（字节）。

**Returns:**
long - 压缩后大小（字节）
### getLength() {#getLength--}
```
public final Long getLength()
```


获取此条目的未压缩长度。

**Returns:**
java.lang.Long - 未压缩长度（字节）
### getName() {#getName--}
```
public final String getName()
```


获取存档中存储的条目名称。

**Returns:**
java.lang.String - 条目名称
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


获取条目数据的未压缩大小（字节）。

**Returns:**
long - 未压缩大小（字节）
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


获取此条目是否表示目录。

**Returns:**
boolean - 对于目录条目为 `true`
### open() {#open--}
```
public final InputStream open()
```


打开条目并提供包含解压缩数据的流。

**Returns:**
java.io.InputStream - 包含解压缩条目数据的流
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


打开条目并提供包含解压缩数据的流。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| password | java.lang.String | 此条目的可选密码 |

**Returns:**
java.io.InputStream - 包含解压缩条目数据的流
