---
title: "AlzArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示一个 ALZ 存档文件。"
type: docs
weight: 11
url: /zh/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

表示一个 ALZ 存档文件。使用此类来检查和提取 ALZ 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | 从流初始化 ALZ 存档。 |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | 使用提供的加载选项从流初始化 ALZ 存档。 |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | 从文件路径初始化 ALZ 存档。 |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | 使用提供的加载选项从文件路径初始化 ALZ 存档。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | 释放此存档占用的资源。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将所有文件和目录提取到提供的目录。 |
| [getEntries()](#getEntries--) | 获取构成此存档的条目。 |
| [getFileEntries()](#getFileEntries--) | 通过通用存档接口获取条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


从流初始化 ALZ 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | ALZ 存档流；它必须支持读取和定位 |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


使用提供的加载选项从流初始化 ALZ 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | ALZ 存档流；它必须支持读取和定位 |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | 用于加载存档的选项 |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


从文件路径初始化 ALZ 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 指向 ALZ 存档的路径 |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


使用提供的加载选项从文件路径初始化 ALZ 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | java.lang.String | 指向 ALZ 存档的路径 |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | 用于加载存档的选项 |

### close() {#close--}
```
public void close()
```


释放此存档占用的资源。

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将所有文件和目录提取到提供的目录。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 目标目录；在必要时会创建 |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


获取构成此存档的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - 不可变的 ALZ 条目列表
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


通过通用存档接口获取条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 存档条目
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
