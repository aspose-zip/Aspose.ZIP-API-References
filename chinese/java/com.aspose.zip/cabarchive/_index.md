---
title: "CabArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 CAB 存档文件。"
type: docs
weight: 44
url: /zh/java/com.aspose.zip/cabarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.zip.ICompressionArchive, java.lang.AutoCloseable
```
public class CabArchive implements ICompressionArchive, AutoCloseable
```

此类表示 CAB 存档文件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CabArchive(CabEntrySettings settings)](#CabArchive-com.aspose.zip.CabEntrySettings-) | 初始化一个准备用于压缩的 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例。 |
| [CabArchive(InputStream sourceStream)](#CabArchive-java.io.InputStream-) | 初始化一个 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
| [CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)](#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-) | 初始化一个 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
| [CabArchive(String path)](#CabArchive-java.lang.String-) | 初始化一个 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
| [CabArchive(String path, CabLoadOptions loadOptions)](#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-) | 初始化一个 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例，并构建可从归档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 将指定目录中的所有文件（递归）添加到归档中。 |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 将指定目录中的所有文件（递归）添加到归档中。 |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | 将指定目录路径中的所有文件递归添加到归档中。 |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | 将指定目录路径中的所有文件递归添加到归档中。 |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | 在存档中创建单个条目。 |
| [createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-) | 在归档中创建单个条目并使用特定设置。 |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | 在存档中创建单个条目。 |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-) | 在存档中创建单个条目。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [getEntries()](#getEntries--) | 获取构成归档的 [CabEntry](../../com.aspose.zip/cabentry) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 cab 归档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 将存档保存到提供的流中。 |
| [save(OutputStream outputStream, CabSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-) | 使用特定选项将归档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件中。 |
| [save(String destinationFileName, CabSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.CabSaveOptions-) | 将存档保存到提供的目标文件中。 |
### CabArchive(CabEntrySettings settings) {#CabArchive-com.aspose.zip.CabEntrySettings-}
```
public CabArchive(CabEntrySettings settings)
```


初始化一个准备用于压缩的 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例。

使用特定的压缩设置压缩文件。

```

``````

CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings()));
try (CabArchive archive = new CabArchive(settings))
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | the source of the archive |

### CabArchive(InputStream sourceStream) {#CabArchive-java.io.InputStream-}
```
public CabArchive(InputStream sourceStream)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

此构造函数不会解压任何条目。请参阅 [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |

### CabArchive(InputStream sourceStream, CabLoadOptions loadOptions) {#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)
```


初始化一个 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例，并构建可从归档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### CabArchive(String path) {#CabArchive-java.lang.String-}
```
public CabArchive(String path)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

此构造函数不会解压任何条目。请参阅 [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径 |

### CabArchive(String path, CabLoadOptions loadOptions) {#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(String path, CabLoadOptions loadOptions)
```


初始化一个 [CabArchive](../../com.aspose.zip/cabarchive) 类的新实例，并构建可从归档中提取的条目列表。

以下示例展示了如何将所有条目提取到目录中。

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CabArchive createEntries(File directory)
```


Adds to the archive all files, recursively, from the specified directory.

```

``````

 try (var archive = new CabArchive())
 {
     File directory = new File("C:/Logs");
     archive.createEntries(directory);
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.io.File | 要压缩的目录。 |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CabArchive createEntries(File directory, boolean includeRootDirectory)
```


将指定目录中的所有文件（递归）添加到归档中。

```

``````

try (var archive = new CabArchive())
{
File directory = new File("C:/Logs");
archive.createEntries(directory, false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CabArchive createEntries(String sourceDirectory)
```


Adds to the archive all files recursively from the specified directory path.

```

``````

 try (var archive = new CabArchive())
 {
     archive.createEntries("C:/Logs");
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 要压缩的目录路径。 |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CabArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


将指定目录路径中的所有文件递归添加到归档中。

```

``````

try (var archive = new CabArchive())
{
archive.createEntries("C:/Logs", false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory path to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final CabEntry createEntry(String name, File fileInfo)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     var sourceFile = new java.io.File("logs\\log.txt");
     archive.createEntry("log.txt", sourceFile);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
|  | fileInfo | java.io.File | 要压缩的文件的元数据。 |

条目名称仅在 `name` 参数中设置。`fileInfo` 参数提供的文件名不会影响条目名称。 |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)
```


在存档中创建单个条目。

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
File sourceFile = new File("logs\\log.txt");
archive.createEntry("log.txt", sourceFile, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| fileInfo | java.io.File | The metadata of file to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `fileInfo` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CabEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
 {
     archive.createEntry("stream-entry.bin", stream);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| source | java.io.InputStream | 条目的输入流。 |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, InputStream source, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)
```


在归档中创建单个条目并使用特定设置。

```

``````

try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
{
CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings());
archive.createEntry("stream-entry.bin", stream, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final CabEntry createEntry(String name, String path)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("entry.bin", "data.bin");
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
|  | path | java.lang.String | 新文件的完全限定名称，或要压缩的相对文件名。 |

条目名称仅在 `name` 参数中设置。`path` 参数提供的文件名不会影响条目名称。 |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, String path, CabEntrySettings newEntrySettings)
```


在存档中创建单个条目。

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry(\"entry.bin\", \"data.bin\", settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("log.txt", () -> new FileInputStream("log.txt"));
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | 为该条目提供输入流的方法。 |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider, CabEntrySettings newEntrySettings)
```


在存档中创建单个条目。

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry(\"log.txt\", () -> new FileInputStream(\"log.txt\"), settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | 用于放置解压文件的目录路径。 |

如果目录不存在，将会创建 |

### getEntries() {#getEntries--}
```
public final List<CabEntry> getEntries()
```


获取构成归档的 [CabEntry](../../com.aspose.zip/cabentry) 类型的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.CabEntry&gt; - 构成存档的 [CabEntry](../../com.aspose.zip/cabentry) 类型的条目
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成 cab 归档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成 cab 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


将存档保存到提供的流中。

```

``````

try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream(\"archive.cab\"))
{
archive.createEntry("entry.bin", "data.bin");
archive.save(cabFile);
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream.

`outputStream` must be writable. |

### save(OutputStream outputStream, CabSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-}
```
public final void save(OutputStream outputStream, CabSaveOptions saveOptions)
```


Saves archive to the stream provided with specific options.

```

``````

  try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream("archive.cab"))
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save(cabFile, options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outputStream | java.io.OutputStream | 目标流。 |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | 存档保存的选项。 |

`outputStream` 必须是可写的。 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


将存档保存到提供的目标文件中。

```

``````

try (CabArchive archive = new CabArchive())
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### save(String destinationFileName, CabSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.CabSaveOptions-}
```
public final void save(String destinationFileName, CabSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

  try (CabArchive archive = new CabArchive())
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save("archive.cab", options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，将会被覆盖。 |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | 存档保存的选项。 |

可以将归档保存到加载时相同的路径。但不推荐这样做，因为此方法会复制到临时文件。 |

