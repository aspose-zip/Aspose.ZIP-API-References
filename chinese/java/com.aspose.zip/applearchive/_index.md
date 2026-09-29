---
title: "AppleArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 Apple Archive .aar 文件。"
type: docs
weight: 16
url: /zh/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

此类表示 Apple Archive (.aar) 文件。可使用它来创建 Apple Archive 文件。

Apple 和 Apple Archive 是 Apple Inc. 的商标。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | 使用用于已组成条目的设置初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例。 |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | 使用用于已组成条目的设置初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例。 |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | 初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。 |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | 初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。 |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | 初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。 |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | 初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 将给定目录中的所有文件和子目录递归添加到存档中。 |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 将给定目录中的所有文件和子目录递归添加到存档中。 |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | 在存档中创建单个条目。 |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | 在存档中创建单个条目。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [getEntries()](#getEntries--) | 获取构成存档的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getNewEntrySettings()](#getNewEntrySettings--) | 获取用于新组成条目的设置。 |
| [isSolid()](#isSolid--) | 获取指示存档是否使用固体压缩的值。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 将存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件。 |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


使用用于已组成条目的设置初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例。

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


使用用于已组成条目的设置初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | 创建新 Apple Archive 时使用的设置。 |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | 存档的来源。 |

此构造函数不会解压任何条目。请参阅用于解压的 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 和 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 方法。 |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源。 |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | 用于加载现有存档的选项。 |

此构造函数不会解压任何条目。请参阅用于解压的 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 和 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 方法。 |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | path | java.lang.String | 存档文件的完全限定路径或相对路径。 |

此构造函数不会解压任何条目。请参阅用于解压的 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 和 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 方法。 |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


初始化 [AppleArchive](../../com.aspose.zip/applearchive) 类的新实例，并组成可从存档中提取的条目列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的完全限定路径或相对路径。 |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | 用于加载现有存档的选项。 |

此构造函数不会解压任何条目。请参阅用于解压的 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 和 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 方法。 |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


将给定目录中的所有文件和子目录递归添加到存档中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.io.File | 要压缩的目录。 |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


将给定目录中的所有文件和子目录递归添加到存档中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.io.File | 要压缩的目录。 |
| includeRootDirectory | 布尔 | 指示是否包含根目录本身。 |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


在存档中创建单个条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| fileInfo | java.io.File | 要压缩的文件的元数据。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


在存档中创建单个条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| fileInfo | java.io.File | 要压缩的文件的元数据。 |
| openImmediately | 布尔 | 如果立即打开文件则为 True，否则在归档保存时打开文件。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


在存档中创建单个条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| source | java.io.InputStream | 条目的输入流。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


在存档中创建单个条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| path | java.lang.String | 要压缩的文件路径。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


在存档中创建单个条目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| path | java.lang.String | 要压缩的文件路径。 |
| openImmediately | 布尔 | 如果立即打开文件则为 True，否则在归档保存时打开文件。 |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将存档中的所有文件提取到提供的目录。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 用于放置解压文件的目录路径。 |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


获取构成存档的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - 构成存档的条目。
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


获取用于新组成条目的设置。

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


获取指示存档是否使用固体压缩的值。在固体模式下，所有条目数据作为单一流进行压缩，无法单独提取条目。请改用 [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--)。

**Returns:**
boolean - 指示存档是否使用固体压缩的值。
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


将存档保存到提供的流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 输出 | java.io.OutputStream | 目标流。 |

`output` 必须可写。某些压缩设置（如 LZ4）还需要可定位的流。 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


将存档保存到提供的目标文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档路径。 |

