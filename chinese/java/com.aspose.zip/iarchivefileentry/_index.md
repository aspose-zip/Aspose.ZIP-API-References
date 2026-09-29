---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "此接口表示一个存档文件条目。"
type: docs
weight: 162
url: /zh/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

此接口表示一个存档文件条目。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getName()](#getName--) | 获取条目的名称。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


将条目提取到提供的流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流。必须可写。 |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


根据提供的路径将条目提取到文件系统中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |

**Returns:**
java.io.File - 包含提取数据的 java.io.File 实例
### getLength() {#getLength--}
```
public abstract Long getLength()
```


获取条目的字节长度。

**Returns:**
java.lang.Long - 条目的字节长度
### getName() {#getName--}
```
public abstract String getName()
```


获取条目的名称。

仅用于压缩的归档，例如 gzip、bzip2、lzip、lzma、xz、z，如果在头部找不到其他名称，则名称为 \"File.bin\"。

**Returns:**
java.lang.String - 条目的名称
