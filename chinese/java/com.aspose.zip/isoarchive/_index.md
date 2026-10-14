---
title: "IsoArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 ISO 9660 标准的 ISO 存档。"
type: docs
weight: 71
url: /zh/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

表示 ISO 存档（ISO 9660）。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | 初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并创建一个用于添加新文件和目录的空 ISO 存档。 |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | 初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并构建一个可从存档中提取的条目列表。 |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | 初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并构建一个可从存档中提取的条目列表。 |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | 初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并构建一个可从存档中提取的条目列表。 |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | 初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并构建一个可从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | 向 ISO 镜像添加目录。 |
| [createEntry(String name)](#createEntry-java.lang.String-) | 向 ISO 镜像添加文件。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 向 ISO 镜像添加文件。 |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | 向 ISO 镜像添加文件。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将所有条目提取到指定目录。 |
| [getEntries()](#getEntries--) | 获取构成存档的 [IsoEntry](../../com.aspose.zip/isoentry) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | 将 ISO 镜像保存到指定的流。 |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | 将 ISO 镜像保存到指定的流。 |
| [save(String path)](#save-java.lang.String-) | 将 ISO 镜像保存到指定的路径。 |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | 将 ISO 镜像保存到指定的路径。 |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并创建一个用于添加新文件和目录的空 ISO 存档。

以下示例展示了如何创建一个新的空 ISO 存档并向其中添加文件：

```

``````

// 创建一个新的空 ISO 存档
try (IsoArchive isoArchive = new IsoArchive()) {
// 向 ISO 存档添加文件
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// 将 ISO 存档保存到文件
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

此构造函数不会解压任何条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并构建一个可从存档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

此构造函数不会解压任何条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径 |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


初始化 [IsoArchive](../../com.aspose.zip/isoarchive) 类的新实例，并构建一个可从存档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (IsoArchive archive = new IsoArchive(\"archive.iso\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 提取条目的目标目录 |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


获取构成存档的 [IsoEntry](../../com.aspose.zip/isoentry) 类型的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - 构成 ISO 存档的 [IsoEntry](../../com.aspose.zip/isoentry) 类型的条目
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成 ISO 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


将 ISO 镜像保存到指定的流。

以下示例展示了如何将 ISO 存档保存到内存流：

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// 创建一个新的空 ISO 存档
try (IsoArchive isoArchive = new IsoArchive()) {
// 向 ISO 存档添加文件
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// 将 ISO 存档保存到内存流
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.OutputStream | ISO 镜像将被保存的流 |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | 用于保存 ISO 存档的选项 |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


将 ISO 镜像保存到指定的路径。

以下示例展示了如何将 ISO 存档保存到文件：

```

``````

// 创建一个新的空 ISO 存档
try (IsoArchive isoArchive = new IsoArchive()) {
// 向 ISO 存档添加文件
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// 将 ISO 存档保存到文件
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | ISO 镜像将被保存的路径 |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | 用于保存 ISO 存档的选项 |

