---
title: "SevenZipArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 7z 存档文件。"
type: docs
weight: 104
url: /zh/java/com.aspose.zip/sevenziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class SevenZipArchive implements IArchive, AutoCloseable
```

此类表示 7z 存档文件。可用于创建和提取 7z 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SevenZipArchive()](#SevenZipArchive--) | 使用可选的条目设置初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例。 |
| [SevenZipArchive(SevenZipEntrySettings newEntrySettings)](#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-) | 使用可选的条目设置初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例。 |
| [SevenZipArchive(InputStream sourceStream)](#SevenZipArchive-java.io.InputStream-) | 初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [SevenZipArchive(InputStream sourceStream, String password)](#SevenZipArchive-java.io.InputStream-java.lang.String-) | 初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [SevenZipArchive(String path)](#SevenZipArchive-java.lang.String-) | 初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [SevenZipArchive(String path, String password)](#SevenZipArchive-java.lang.String-java.lang.String-) | 初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)](#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-) | 初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [SevenZipArchive(String path, SevenZipLoadOptions options)](#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-) | 初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [SevenZipArchive(String[] parts)](#SevenZipArchive-java.lang.String---) | 从多卷 7z 存档初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [SevenZipArchive(String[] parts, String password)](#SevenZipArchive-java.lang.String---java.lang.String-) | 从多卷 7z 存档初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。 |
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
| [createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | 在存档中创建单个条目。 |
| [createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-) | 在存档中创建单个条目。 |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | 在存档中创建单个条目。 |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-) | 在存档中创建单个条目。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [extractToDirectory(String destinationDirectory, String password)](#extractToDirectory-java.lang.String-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [getEntries()](#getEntries--) | 获取构成存档的 [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 7z 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getNewEntrySettings()](#getNewEntrySettings--) | 用于新添加的 [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) 项目的压缩和加密设置。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 将 7z 存档保存到提供的流中。 |
| [save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-) | 将 7z 存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件。 |
| [save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-) | 将存档保存到提供的目标文件。 |
| [saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-) | 将多卷存档保存到提供的目标目录。 |
### SevenZipArchive() {#SevenZipArchive--}
```
public SevenZipArchive()
```


使用可选的条目设置初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例。

以下示例展示了如何使用默认设置压缩单个文件：LZMA 压缩且不加密。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

LZMA compression without encryption would be used.

### SevenZipArchive(SevenZipEntrySettings newEntrySettings) {#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-}
```
public SevenZipArchive(SevenZipEntrySettings newEntrySettings)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class with optional settings for its entries.

The following example shows how to compress a single file with default settings: LZMA compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | 用于新添加的 [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) 项目的压缩和加密设置。如果未指定，将使用不加密的 LZMA 压缩。 |

### SevenZipArchive(InputStream sourceStream) {#SevenZipArchive-java.io.InputStream-}
```
public SevenZipArchive(InputStream sourceStream)
```


初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### SevenZipArchive(InputStream sourceStream, String password) {#SevenZipArchive-java.io.InputStream-java.lang.String-}
```
public SevenZipArchive(InputStream sourceStream, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

此构造函数不会解压任何条目。请参阅 [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) 方法进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |
| password | java.lang.String | 可选的解密密码。如果文件名已加密，则必须提供。 |

### SevenZipArchive(String path) {#SevenZipArchive-java.lang.String-}
```
public SevenZipArchive(String path)
```


初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### SevenZipArchive(String path, String password) {#SevenZipArchive-java.lang.String-java.lang.String-}
```
public SevenZipArchive(String path, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

此构造函数不会解压任何条目。请参阅 [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) 方法进行解压。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 归档文件的完全限定路径或相对路径 |
| password | java.lang.String | 可选的解密密码。如果文件名已加密，则必须提供。 |

### SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options) {#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)
```


初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。

解压加密的归档。允许最多 60 秒的处理时间，超过后将取消。

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("Top$ecr3t");
options.setCancellationFlag(cf);
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
a.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Options to load existing archive with.

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing. |

### SevenZipArchive(String path, SevenZipLoadOptions options) {#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(String path, SevenZipLoadOptions options)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

Extract an encrypted archive. Allow up to 60 seconds to proceed, cancel after that period.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setDecryptionPassword("Top$ecr3t");
         options.setCancellationFlag(cf);
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
             a.extractToDirectory("C:\\extracted");
         } catch (IOException ex) {
         }
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的完全限定路径或相对路径。 |
|  | options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | 用于加载现有存档的选项。 |

此构造函数不会解压任何条目。请参阅 [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) 方法进行解压。 |

### SevenZipArchive(String[] parts) {#SevenZipArchive-java.lang.String---}
```
public SevenZipArchive(String[] parts)
```


从多卷 7z 存档初始化 [SevenZipArchive](../../com.aspose.zip/sevenziparchive) 类的新实例，并构建可从存档中提取的条目列表。

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parts | java.lang.String[] | paths to each segment of multi-volume 7z archive respecting order |

### SevenZipArchive(String[] parts, String password) {#SevenZipArchive-java.lang.String---java.lang.String-}
```
public SevenZipArchive(String[] parts, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class from multi-volume 7z archive and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| parts | java.lang.String[] | 多卷 7z 归档每个段的路径，按顺序排列 |
| password | java.lang.String | 可选的解密密码。如果文件名已加密，则必须提供。 |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SevenZipArchive createEntries(File directory)
```


将给定目录中的所有文件和子目录递归添加到存档中。

```

``````

try (SevenZipArchive archive = new SevenZipArchive()) {
File folder = new File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SevenZipArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         File folder = new File("C:\\folder");
         archive.createEntries(folder);
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目录 | java.io.File | 要压缩的目录 |
| includeRootDirectory | 布尔 | 指示是否包含根目录本身 |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SevenZipArchive createEntries(String sourceDirectory)
```


将给定目录中的所有文件和子目录递归添加到存档中。

使用 LZMA 压缩创建 7z 归档。

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntries("C:\\folder");
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SevenZipArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

Compose 7z archive with LZMA compression.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
         archive.createEntries("C:\\folder");
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 要压缩的目录 |
| includeRootDirectory | 布尔 | 指示是否包含根目录本身 |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, File file)
```


在存档中创建单个条目。

将归档与每个条目使用不同密码加密的方式组合。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different passwords each.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         File fi1 = new File("data1.bin");
         File fi2 = new File("data2.bin");
         File fi3 = new File("data3.bin");

         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
             archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
             archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

条目名称仅在 `name` 参数中设置。`file` 参数提供的文件名不会影响条目名称。

如果使用 `openImmediately` 参数立即打开文件，则该文件会被阻塞，直到归档保存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| file | java.io.File | 要压缩的文件的元数据 |
| openImmediately | 布尔 | true，表示立即打开文件；否则在归档保存时打开文件 |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


在存档中创建单个条目。

将归档与每个条目使用不同密码加密的方式组合。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

Compose 7z archive with LZMA compression and encryption of all entries.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.7z");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| source | java.io.InputStream | 条目的输入流 |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)
```


在存档中创建单个条目。

使用 LZMA 压缩和对所有条目进行加密来创建 7z 归档。

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
archive.save("archive.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with LZMA compressed encrypted entry.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF}), new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new File("data1.bin"));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

条目名称仅在 `name` 参数中设置。`file` 参数提供的文件名不会影响条目名称。

`file` 可以指向目录。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| source | java.io.InputStream | 条目的输入流 |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | 用于添加的 [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) 项目的压缩和加密设置。对于固实压缩，单独的压缩设置将被忽略，请参阅 `SevenZipEntrySettings.Solid`（[SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)）。 |
| file | java.io.File | 要压缩的文件或文件夹的元数据 |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final SevenZipArchiveEntry createEntry(String name, String path)
```


在存档中创建单个条目。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

条目名称仅在 `name` 参数中设置。`path` 参数提供的文件名不会影响条目名称。

如果使用 `openImmediately` 参数立即打开文件，则该文件会被阻塞，直到归档保存。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称 |
| path | java.lang.String | 新文件的完全限定名称，或要压缩的相对文件名 |
| openImmediately | 布尔 | true，表示立即打开文件；否则在归档保存时打开文件 |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


在存档中创建单个条目。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

Compose archive with LZMA2 compressed encrypted entry.

```

``````

 System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
 using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
 {
     using (var archive = new SevenZipArchive())
     {
         archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
         archive.Save(sevenZipFile);
     }
 }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 条目的名称。 |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | 为该条目提供输入流的方法。 |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, SevenZipEntrySettings newEntrySettings)
```


在存档中创建单个条目。

使用 LZMA2 压缩并加密的条目来创建归档。

```

``````

System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
using (var archive = new SevenZipArchive())
{
archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.Save(sevenZipFile);
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | Compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | 用于放置解压文件的目录路径。 |

如果目录不存在，将会创建 |

### extractToDirectory(String destinationDirectory, String password) {#extractToDirectory-java.lang.String-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory, String password)
```


将存档中的所有文件提取到提供的目录。

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |
| password | java.lang.String | optional password for content decryption.

`password` is used for content decryption only. If file names are encrypted provide password in [SevenZipArchive(String, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-String--String-) or [SevenZipArchive(java.io.InputStream, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-java.io.InputStream--String-) constructor. |

### getEntries() {#getEntries--}
```
public final List<SevenZipArchiveEntry> getEntries()
```


Gets entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.SevenZipArchiveEntry&gt; - entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final SevenZipEntrySettings getNewEntrySettings()
```


Compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items.

**Returns:**
[SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) - compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves 7z archive to the stream provided.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (SevenZipArchive archive = new SevenZipArchive()) {
                 archive.createEntry("data", source);
                 archive.save(sevenZipFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | java.io.OutputStream | 目标流 |

### save(OutputStream output, SevenZipArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)
```


将 7z 存档保存到提供的流中。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("data", source);
archive.save(sevenZipFile);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to a destination file provided.

```

``````

  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
     using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
     {
        archive.CreateEntry("data", source);
        archive.Save("archive.7z");
     }
  }
  
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，将会被覆盖。 |

可以将归档保存到加载时相同的路径。但不推荐这样做，因为此方法会复制到临时文件。 |

### save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)
```


将存档保存到提供的目标文件。

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data", source);
archive.save("archive.7z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```


Saves multi-volume archive to destination directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         archive.createEntry("entry.bin", "data.bin");
         archive.saveSplit("C:\\Folder", new SplitSevenZipArchiveSaveOptions("volume", 65536));
     }
 
```

此方法会组合多个 `(n)` 文件，例如 filename.7z.001、filename.7z.002、...、filename.7z.(n)。

无法将现有归档设为多卷。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 用于创建归档段的目录路径 |
| options | [SplitSevenZipArchiveSaveOptions](../../com.aspose.zip/splitsevenziparchivesaveoptions) | 归档保存的选项，包括文件名 |

