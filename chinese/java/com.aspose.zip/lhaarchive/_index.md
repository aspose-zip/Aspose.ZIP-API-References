---
title: "LhaArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示一个 LHA .lzh 存档文件。"
type: docs
weight: 75
url: /zh/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

此类表示 LHA（.lzh）存档文件。

仅支持以下压缩方法：

| ------ | --------------------------------------------- |
| 方法 | 说明                                   |
| lh0    | 未压缩                                  |
| lh4    | 8 KiB 滑动字典和静态 Huffman   |
| lh5    | 16 KiB 滑动字典和静态 Huffman  |
| lh6    | 64 KiB 滑动字典和静态 Huffman  |
| lh7    | 128 KiB 滑动字典和静态 Huffman |
| lhx    | 1 Mib 滑动字典和静态 Huffman   |
| lhd    | 目录                                     |
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | 初始化一个新的 [LhaArchive](../../com.aspose.zip/lhaarchive) 类的实例，并构建可从存档中提取的条目列表。 |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | 初始化一个新的 [LhaArchive](../../com.aspose.zip/lhaarchive) 类的实例，并构建可从存档中提取的条目列表。 |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | 初始化一个新的 [LhaArchive](../../com.aspose.zip/lhaarchive) 类的实例，并构建可从存档中提取的条目列表。 |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | 初始化一个新的 [LhaArchive](../../com.aspose.zip/lhaarchive) 类的实例，并构建可从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件和目录提取到提供的目录中。 |
| [getEntries()](#getEntries--) | 获取构成存档的 [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) 类型的文件条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


初始化一个新的 [LhaArchive](../../com.aspose.zip/lhaarchive) 类的实例，并构建可从存档中提取的条目列表。

此构造函数不会解压任何条目。请参阅用于解压的 [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


初始化一个新的 [LhaArchive](../../com.aspose.zip/lhaarchive) 类的实例，并构建可从存档中提取的条目列表。

此构造函数不会解压任何条目。请参阅用于解压的 [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | 用于加载现有存档的选项。 |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


初始化一个新的 [LhaArchive](../../com.aspose.zip/lhaarchive) 类的实例，并构建可从存档中提取的条目列表。

以下示例提取存档，然后将第一个条目解压到 `MemoryStream`。

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

此构造函数不会解压任何条目。请参阅 [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 归档文件的完全限定路径或相对路径 |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | 用于加载现有存档的选项。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将存档中的所有文件和目录提取到提供的目录中。

```

``````

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
