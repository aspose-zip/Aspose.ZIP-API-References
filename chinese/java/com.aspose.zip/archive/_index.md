---
title: "存档"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 zip 存档文件。"
type: docs
weight: 26
url: /zh/java/com.aspose.zip/archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class Archive implements IArchive, AutoCloseable
```

此类表示一个 zip 存档文件。可用于创建、提取或更新 zip 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Archive()](#Archive--) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并可为其条目提供可选设置。 |
| [Archive(ArchiveEntrySettings newEntrySettings)](#Archive-com.aspose.zip.ArchiveEntrySettings-) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并可为其条目提供可选设置。 |
| [Archive(InputStream sourceStream)](#Archive-java.io.InputStream-) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
| [Archive(String path)](#Archive-java.lang.String-) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
| [Archive(String path, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
| [Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | 初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
| [Archive(String mainSegment, String[] segmentsInOrder)](#Archive-java.lang.String-java.lang.String---) | 从多卷 ZIP 存档初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
| [Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-) | 从多卷 ZIP 存档初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 将给定目录中的所有文件和子目录递归添加到存档中。 |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 将给定目录中的所有文件和子目录递归添加到存档中。 |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | 将给定目录中的所有文件和子目录递归添加到存档中。 |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | 将给定目录中的所有文件和子目录递归添加到存档中。 |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | 在存档中创建单个条目。 |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | 在存档中创建单个条目。 |
| [createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | 在存档中创建单个条目。 |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-) | 在存档中创建单个条目。 |
| [deleteEntry(ArchiveEntry entry)](#deleteEntry-com.aspose.zip.ArchiveEntry-) | 从条目列表中移除特定条目的第一次出现。 |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | 按索引从条目列表中移除条目。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [getComment()](#getComment--) | 获取整个存档的注释。 |
| [getEntries()](#getEntries--) | 获取构成存档的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式（Zip） |
| [getNewEntrySettings()](#getNewEntrySettings--) | 用于新添加的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 项目的压缩和加密设置。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 将存档保存到提供的流中。 |
| [save(OutputStream outputStream, ArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-) | 将存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件中。 |
| [save(String destinationFileName, ArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-) | 将存档保存到提供的目标文件中。 |
| [saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-) | 将多卷存档保存到提供的目标目录中。 |
### Archive() {#Archive--}
```
public Archive()
```


初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并可为其条目提供可选设置。


以下示例展示了如何使用默认设置压缩单个文件。

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```



### Archive(ArchiveEntrySettings newEntrySettings) {#Archive-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries.


The following example shows how to compress a single file with default settings.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | 用于新添加的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 项目的压缩和加密设置。如果未指定，将使用最常用的 Deflate 压缩且不加密。 |

### Archive(InputStream sourceStream) {#Archive-java.io.InputStream-}
```
public Archive(InputStream sourceStream)
```


初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。

下面的示例提取加密的存档，然后将第一个条目解压缩到 `ByteArrayOutputStream`。

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

此构造函数不会解压任何条目。请参阅 [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源。 |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | 用于加载现有存档的选项。 |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。

下面的示例提取加密的存档，然后将第一个条目解压缩到 `ByteArrayOutputStream`。

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, the most common Deflate compression without encryption would be used. |

### Archive(String path) {#Archive-java.lang.String-}
```
public Archive(String path)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

此构造函数不会解压任何条目。请参阅 [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的完全限定路径或相对路径。 |

### Archive(String path, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String path, ArchiveLoadOptions loadOptions)
```


初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。

下面的示例提取加密的存档，然后将第一个条目解压缩到 `ByteArrayOutputStream`。

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive("encrypted.zip", options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |

### Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

此构造函数不会解压任何条目。请参阅 [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) 方法以进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的完全限定路径或相对路径。 |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | 用于加载现有存档的选项。 |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | 用于新添加的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 项目的压缩和加密设置。如果未指定，将使用最常用的 Deflate 压缩且不加密。 |

### Archive(String mainSegment, String[] segmentsInOrder) {#Archive-java.lang.String-java.lang.String---}
```
public Archive(String mainSegment, String[] segmentsInOrder)
```


从多卷 ZIP 存档初始化 [Archive](../../com.aspose.zip/archive) 类的新实例，并生成可从存档中提取的条目列表。

```

``````

try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
a.extractToDirectory("destination");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mainSegment | java.lang.String | Path to the last segment of multi-volume archive with the central directory.

Usually this segment has \*.zip extension and smaller than others. |
| segmentsInOrder | java.lang.String[] | Paths to each segment but the last of multi-volume zip archive respecting order.

Usually they named filename.z01, filename.z02, ..., filename.z(n-1). |

### Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class from multi-volume ZIP archive and composes an entry list can be extracted from the archive.

This sample extract to a directory an archive of three segments.

```

``````

     try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
         a.extractToDirectory("destination");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | mainSegment | java.lang.String | 多卷存档中带有中心目录的最后一个段的路径。 |

通常此段的扩展名为 \\*.zip，且比其他段小。 |
|  | segmentsInOrder | java.lang.String[] | 多卷 zip 存档中除最后一个段之外的每个段的路径，按顺序排列。 |

通常它们命名为 filename.z01、filename.z02、...、filename.z(n-1)。 |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | 用于加载现有存档的选项。 |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final Archive createEntries(File directory)
```


将给定目录中的所有文件和子目录递归添加到存档中。

```

``````

try (Archive archive = new Archive()) {
java.io.File folder = new java.io.File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final Archive createEntries(File directory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        java.io.File folder = new java.io.File("C:\\folder");
        archive.createEntries(folder);
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.io.File | 要压缩的目录。 |
| includeRootDirectory | 布尔 | 指示是否包含根目录本身。 |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final Archive createEntries(String sourceDirectory)
```


将给定目录中的所有文件和子目录递归添加到存档中。

```

``````

try (Archive archive = new Archive()) {
archive.createEntries("C:\\folder");
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final Archive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntries("C:\\folder");
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 要压缩的目录。 |
| includeRootDirectory | 布尔 | 指示是否包含根目录本身。 |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final ArchiveEntry createEntry(String name, File file)
```


在存档中创建单个条目。

创建归档，其中每个条目使用不同的加密方法和密码进行加密。

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different encryption methods and passwords each.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

条目名称仅在 `name` 参数中设置。`file` 参数提供的文件名不会影响条目名称。

如果使用 `openImmediately` 参数立即打开文件，则该文件会被阻塞，直到归档保存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| file | java.io.File | 要压缩的文件的元数据。 |
| openImmediately | 布尔 | 如果立即打开文件则为 True，否则在归档保存时打开文件。 |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


在存档中创建单个条目。

创建归档，其中每个条目使用不同的加密方法和密码进行加密。

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final ArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.zip");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| source | java.io.InputStream | 条目的输入流。 |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)
```


在存档中创建单个条目。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {
                    0x00,
                    (byte) 0xFF
            }), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new java.io.File("data1.bin"));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

条目名称仅在 `name` 参数中设置。`file` 参数提供的文件名不会影响条目名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| source | java.io.InputStream | 条目的输入流。 |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | 用于添加的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 项目的压缩和加密设置。 |
| file | java.io.File | 要压缩的文件或文件夹的元数据。 |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final ArchiveEntry createEntry(String name, String path)
```


在存档中创建单个条目。

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

条目名称仅在 `name` 参数中设置。`path` 参数提供的文件名不会影响条目名称。

如果使用 `openImmediately` 参数立即打开文件，则该文件会被阻塞，直到归档保存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| path | java.lang.String | 新文件的完全限定名称，或要压缩的相对文件名。 |
| openImmediately | 布尔 | 如果立即打开文件则为 True，否则在归档保存时打开文件。 |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


在存档中创建单个条目。

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

     Supplier<InputStream> provider = new Supplier<InputStream>() {
         public InputStream get() {
             return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
         }
     };
     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
             archive.save(zipFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | 提供条目输入流的方法 |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, ArchiveEntrySettings newEntrySettings)
```


在存档中创建单个条目。

使用加密条目创建归档。

```

``````

Supplier<InputStream> provider = new Supplier<InputStream>() {
public InputStream get() {
return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
}
};
try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.save(zipFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | the method providing input stream for the entry |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### deleteEntry(ArchiveEntry entry) {#deleteEntry-com.aspose.zip.ArchiveEntry-}
```
public final Archive deleteEntry(ArchiveEntry entry)
```


Removes the first occurrence of the specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        while (archive.getEntries().size() > 1)
            archive.deleteEntry(archive.getEntries().get(0));
        archive.save("last_entry.zip");
    }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | 要从条目列表中移除的条目。 |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final Archive deleteEntry(int entryIndex)
```


按索引从条目列表中移除条目。

```

``````

try (Archive archive = new Archive("two_files.zip")) {
archive.deleteEntry(0);
archive.save("single_file.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | The zero-based index of the entry to remove. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        archive.extractToDirectory("C:\\extracted");
    }
 
```

如果目录不存在，将会被创建。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 用于放置解压文件的目录路径。 |

### getComment() {#getComment--}
```
public final String getComment()
```


获取整个存档的注释。

如果提供了 `ArchiveLoadOptions.Encoding`([ArchiveLoadOptions.getEncoding](../../com.aspose.zip/archiveloadoptions\#getEncoding)/[ArchiveLoadOptions.setEncoding](../../com.aspose.zip/archiveloadoptions\#setEncoding))，则使用它进行解码。否则，将使用 UTF-8。

**Returns:**
java.lang.String - 整个存档的注释。
### getEntries() {#getEntries--}
```
public final List<ArchiveEntry> getEntries()
```


获取构成存档的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 类型的条目。

**Returns:**
java.util.List&lt;com.aspose.zip.ArchiveEntry&gt; - 构成存档的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 类型的条目。
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


获取存档格式（Zip）

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - Zip archive format.
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final ArchiveEntrySettings getNewEntrySettings()
```


用于新添加的 [ArchiveEntry](../../com.aspose.zip/archiveentry) 项目的压缩和加密设置。

**Returns:**
[ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) - the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) instance
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


将存档保存到提供的流中。

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

`outputStream` must be writable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream. |

### save(OutputStream outputStream, ArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(OutputStream outputStream, ArchiveSaveOptions saveOptions)
```


Saves archive to the stream provided.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry.bin", "data.bin");
            archive.save(zipFile);
        }
    } catch (IOException ex) {
    }
 
```

`outputStream` 必须是可写的。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outputStream | java.io.OutputStream | 目标流。 |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | 存档保存的选项。 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


将存档保存到提供的目标文件中。

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncoding(StandardCharsets.US_ASCII);
archive.save("archive.zip", options);
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, ArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(String destinationFileName, ArchiveSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncoding(StandardCharsets.US_ASCII);
        archive.save("archive.zip", options);
    }
 
```

可以将存档保存到其加载时的相同路径。但不推荐这样做，因为此方法会复制到临时文件。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，将会被覆盖。 |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | 存档保存的选项。 |

### saveSplit(String destinationDirectory, SplitArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)
```


将多卷存档保存到提供的目标目录中。

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.saveSplit( "C:\\Folder", new SplitArchiveSaveOptions("volume", 65536));
}
 
```

This method composes several (n) files filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Cannot make existing archive multi-volume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory where archive segments to be created. |
| options | [SplitArchiveSaveOptions](../../com.aspose.zip/splitarchivesaveoptions) | Options for archive saving, including file name. |

