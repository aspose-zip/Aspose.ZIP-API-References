---
title: "XarArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示一个 xar 存档文件。"
type: docs
weight: 136
url: /zh/java/com.aspose.zip/xararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XarArchive implements IArchive, AutoCloseable
```

此类表示一个 xar 存档文件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XarArchive()](#XarArchive--) | 初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例。 |
| [XarArchive(XarCompressionSettings defaultCompressionSettings)](#XarArchive-com.aspose.zip.XarCompressionSettings-) | 初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例。 |
| [XarArchive(InputStream sourceStream)](#XarArchive-java.io.InputStream-) | 初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例，并组成可从存档中提取的条目列表。 |
| [XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)](#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-) | 初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例，并组成可从存档中提取的条目列表。 |
| [XarArchive(String path)](#XarArchive-java.lang.String-) | 初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例，并组成可从存档中提取的条目列表。 |
| [XarArchive(String path, XarLoadOptions loadOptions)](#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-) | 初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例，并组成可从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| [createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| [createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | 将给定目录中的所有文件和子目录递归地添加到存档中。 |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | 在存档中创建单个条目。 |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | 在存档中创建单个条目。 |
| [createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | 在存档中创建单个条目。 |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | 在存档中创建单个条目。 |
| [createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | 在存档中创建单个条目。 |
| [deleteEntry(XarEntry entry)](#deleteEntry-com.aspose.zip.XarEntry-) | 从条目列表中移除特定条目的第一次出现。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [getEntries()](#getEntries--) | 获取构成存档的 [XarEntry](../../com.aspose.zip/xarentry) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 xar 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 将存档保存到提供的流中。 |
| [save(OutputStream output, XarSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-) | 将存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件中。 |
| [save(String destinationFileName, XarSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.XarSaveOptions-) | 将存档保存到提供的目标文件中。 |
### XarArchive() {#XarArchive--}
```
public XarArchive()
```


初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例。

以下示例展示了如何压缩文件。

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```



### XarArchive(XarCompressionSettings defaultCompressionSettings) {#XarArchive-com.aspose.zip.XarCompressionSettings-}
```
public XarArchive(XarCompressionSettings defaultCompressionSettings)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class.

The following example shows how to compress a file.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultCompressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | 默认压缩设置，适用于存档的所有条目。 |

### XarArchive(InputStream sourceStream) {#XarArchive-java.io.InputStream-}
```
public XarArchive(InputStream sourceStream)
```


初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例，并组成可从存档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### XarArchive(InputStream sourceStream, XarLoadOptions loadOptions) {#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

此构造函数不会解压任何条目。请参阅用于解压的 [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | 用于加载存档的选项。 |

### XarArchive(String path) {#XarArchive-java.lang.String-}
```
public XarArchive(String path)
```


初始化 [XarArchive](../../com.aspose.zip/xararchive) 类的新实例，并组成可从存档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### XarArchive(String path, XarLoadOptions loadOptions) {#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(String path, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

此构造函数不会解压任何条目。请参阅用于解压的 [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径 |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | 用于加载存档的选项。 |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final XarArchive createEntries(File directory)
```


将给定目录中的所有文件和子目录递归地添加到存档中。

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.io.File | 要压缩的目录 |
| includeRootDirectory | 布尔 | 指示是否包含根目录本身 |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


将给定目录中的所有文件和子目录递归地添加到存档中。

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final XarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 要压缩的目录 |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


将给定目录中的所有文件和子目录递归地添加到存档中。

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 要压缩的目录 |
| includeRootDirectory | 布尔 | 指示是否包含根目录本身 |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | 用于添加的 [XarEntry](../../com.aspose.zip/xarentry) 项目的压缩设置 |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final XarEntry createEntry(String name, File file)
```


在存档中创建单个条目。

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.xar");
     }
 
```

如果使用 `openImmediately` 参数立即打开文件，则该文件会被阻塞，直到归档被释放

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| file | java.io.File | 要压缩的文件或文件夹的元数据 |
| openImmediately | 布尔 | 如果立即打开文件则为 true，否则在归档保存时打开文件。 |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)
```


在存档中创建单个条目。

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final XarEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.xar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| source | java.io.InputStream | 条目的输入流 |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)
```


在存档中创建单个条目。

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", new FileInputStream("data.bin"));
archive.save("archive.xar");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final XarEntry createEntry(String name, String sourcePath)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

条目名称仅在 `name` 参数中设置。`sourcePath` 参数提供的文件名不会影响条目名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| sourcePath | java.lang.String | 要压缩的文件路径 |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


在存档中创建单个条目。

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

条目名称仅在 `name` 参数中设置。`sourcePath` 参数提供的文件名不会影响条目名称。

如果使用 `openImmediately` 参数立即打开文件，则该文件会被锁定，直到归档被释放。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| sourcePath | java.lang.String | 要压缩的文件路径 |
| openImmediately | 布尔 | true，表示立即打开文件；否则在归档保存时打开文件 |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | 用于添加的 [XarEntry](../../com.aspose.zip/xarentry) 项目的压缩设置 |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### deleteEntry(XarEntry entry) {#deleteEntry-com.aspose.zip.XarEntry-}
```
public final XarArchive deleteEntry(XarEntry entry)
```


从条目列表中移除特定条目的第一次出现。

以下是如何删除除最后一个之外的所有条目：

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputXarFile.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | the entry to remove from the entries list |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | 用于放置解压文件的目录路径。 |

如果目录不存在，将会创建 |

### getEntries() {#getEntries--}
```
public final List<XarEntry> getEntries()
```


获取构成存档的 [XarEntry](../../com.aspose.zip/xarentry) 类型的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.XarEntry&gt; - 构成归档的 [XarEntry](../../com.aspose.zip/xarentry) 类型的条目
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成 xar 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成 xar 归档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


将存档保存到提供的流中。

对于大型归档，请使用 [save(String)](../../com.aspose.zip/xararchive\#save-String-) 而不是保存到 java.io.FileOutputStream。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | java.io.OutputStream | 目标流 |

### save(OutputStream output, XarSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-}
```
public final void save(OutputStream output, XarSaveOptions saveOptions)
```


将存档保存到提供的流中。

对于大型归档，请使用 [save(String)](../../com.aspose.zip/xararchive\#save-String-) 而不是保存到 java.io.FileOutputStream。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | java.io.OutputStream | 目标流 |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | 用于保存 xar 归档的选项 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


将存档保存到提供的目标文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，它将被覆盖 |

### save(String destinationFileName, XarSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.XarSaveOptions-}
```
public final void save(String destinationFileName, XarSaveOptions saveOptions)
```


将存档保存到提供的目标文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，它将被覆盖 |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | 用于保存 xar 归档的选项 |

