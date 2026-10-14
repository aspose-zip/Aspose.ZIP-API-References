---
title: "ArjArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 ARJ 存档文件。"
type: docs
weight: 37
url: /zh/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

此类表示 ARJ 存档文件。

仅支持以下压缩方法：

| ------ | ------------------------------------------------------------ |
| 方法 | 说明 |
| 0      | 未压缩                                                 |
| 1      | LZ77 与自适应哈夫曼编码的组合。最佳比率。 |
| 2      | LZ77 与自适应哈夫曼编码的组合。             |
| 3      | LZ77 与自适应哈夫曼编码的组合。最佳速度。 |
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | 初始化 [ArjArchive](../../com.aspose.zip/arjarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | 初始化 [ArjArchive](../../com.aspose.zip/arjarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | 初始化 [ArjArchive](../../com.aspose.zip/arjarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | 初始化 [ArjArchive](../../com.aspose.zip/arjarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将所有条目提取到指定目录。 |
| [getCommentary()](#getCommentary--) | 获取注释。 |
| [getEntries()](#getEntries--) | 获取构成 ARJ 归档的 [ArjEntryPlain](../../com.aspose.zip/arjentryplain) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getName()](#getName--) | 获取原始名称。 |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


初始化 [ArjArchive](../../com.aspose.zip/arjarchive) 类的新实例，并构建可从归档中提取的条目列表。

此构造函数不会解压任何条目。请参阅用于解压的 [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 存档的来源 |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


初始化 [ArjArchive](../../com.aspose.zip/arjarchive) 类的新实例，并构建可从归档中提取的条目列表。

此构造函数不会解压任何条目。请参阅用于解压的 [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 存档的来源 |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | 用于加载现有存档的选项。 |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


初始化 [ArjArchive](../../com.aspose.zip/arjarchive) 类的新实例，并构建可从归档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (ArjArchive archive = new ArjArchive(\"archive.arj\")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

此构造函数不会解包任何条目。请参阅用于解压的 [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\\#extract-java.io.OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径 |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | 用于加载现有存档的选项。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将所有条目提取到指定目录。

以下示例展示了如何将所有条目提取到目录中：

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream(\"archive.arj\"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
