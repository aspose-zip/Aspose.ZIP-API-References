---
title: "WimArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示一个 wim 存档文件。"
type: docs
weight: 130
url: /zh/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

此类表示一个 wim 存档文件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | 初始化一个新的 [WimArchive](../../com.aspose.zip/wimarchive) 类实例，并构建一个可以从存档中提取的条目列表。 |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | 初始化一个新的 [WimArchive](../../com.aspose.zip/wimarchive) 类实例，并构建一个可以从存档中提取的条目列表。 |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | 初始化一个新的 [WimArchive](../../com.aspose.zip/wimarchive) 类实例，并构建一个可以从存档中提取的条目列表。 |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | 初始化一个新的 [WimArchive](../../com.aspose.zip/wimarchive) 类实例，并构建一个可以从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档提取到指定路径的文件中。 |
| [getBootImageIndex()](#getBootImageIndex--) | 获取可启动映像的（从零开始的）索引。 |
| [getEntries()](#getEntries--) | 获取构成存档的 [WimEntry](../../com.aspose.zip/wimentry) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 Wim 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFileFormatVersion()](#getFileFormatVersion--) | 获取文件格式的版本。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getGuid()](#getGuid--) | 获取存档的标识 UUID。 |
| [getImages()](#getImages--) | 获取构成存档的 [WimImage](../../com.aspose.zip/wimimage) 类型的条目。 |
| [getManifest()](#getManifest--) | 获取描述文件及其包含的映像的嵌入式清单。 |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


初始化一个新的 [WimArchive](../../com.aspose.zip/wimarchive) 类实例，并构建一个可以从存档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream(\"archive.wim\"))) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

此构造函数不解压任何条目。有关解压，请参阅 [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | 用于加载现有存档的选项。 |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


初始化一个新的 [WimArchive](../../com.aspose.zip/wimarchive) 类实例，并构建一个可以从存档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

此构造函数不解压任何条目。有关解压，请参阅 [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径 |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | 用于加载现有存档的选项。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将存档提取到指定路径的文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 用于放置提取文件的目录路径 |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


获取可启动映像的（从零开始的）索引。

**Returns:**
int - 可启动映像的（从零开始的）索引
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


获取构成存档的 [WimEntry](../../com.aspose.zip/wimentry) 类型的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - 构成存档的条目
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成 Wim 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成 Wim 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


获取文件格式的版本。

**Returns:**
int - 文件格式的版本
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


获取存档的标识 UUID。

**Returns:**
java.util.UUID - 用于标识归档的 UUID
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


获取构成存档的 [WimImage](../../com.aspose.zip/wimimage) 类型的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - 构成归档的 [WimImage](../../com.aspose.zip/wimimage) 类型的条目
### getManifest() {#getManifest--}
```
public final String getManifest()
```


获取描述文件及其包含的映像的嵌入式清单。

**Returns:**
java.lang.String - 描述文件及其包含的图像的嵌入式清单
