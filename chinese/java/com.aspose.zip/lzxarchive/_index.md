---
title: "LzxArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示一个 LZX .lzx 存档文件。"
type: docs
weight: 89
url: /zh/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

此类表示 LZX（.lzx）存档文件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | 初始化 [LzxArchive](../../com.aspose.zip/lzxarchive) 类的新实例，并构造一个可以从存档中提取的条目列表。 |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | 初始化 [LzxArchive](../../com.aspose.zip/lzxarchive) 类的新实例，并构造一个可以从存档中提取的条目列表。 |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | 初始化 [LzxArchive](../../com.aspose.zip/lzxarchive) 类的新实例，并构造一个可以从存档中提取的条目列表。 |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | 初始化 [LzxArchive](../../com.aspose.zip/lzxarchive) 类的新实例，并构造一个可以从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件和目录提取到提供的目录中。 |
| [getEntries()](#getEntries--) | 获取构成存档的 [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) 类型的文件条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


初始化 [LzxArchive](../../com.aspose.zip/lzxarchive) 类的新实例，并构造一个可以从存档中提取的条目列表。

此构造函数不解压任何条目。请参阅 [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 存档的来源。 |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


初始化 [LzxArchive](../../com.aspose.zip/lzxarchive) 类的新实例，并构造一个可以从存档中提取的条目列表。

此构造函数不解压任何条目。请参阅 [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 存档的来源。 |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | 用于加载现有存档的选项。 |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


初始化 [LzxArchive](../../com.aspose.zip/lzxarchive) 类的新实例，并构造一个可以从存档中提取的条目列表。

以下示例提取存档，然后将第一个条目解压到 `MemoryStream`。

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

此构造函数不解压任何条目。请参阅 [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的完全限定路径或相对路径。 |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | 用于加载现有存档的选项。 |

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

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
