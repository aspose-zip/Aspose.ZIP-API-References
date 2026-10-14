---
title: "LzipArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 Lzip 存档文件。"
type: docs
weight: 83
url: /zh/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

此类表示一个 Lzip 存档文件。可用于创建或提取 Lzip 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | 初始化一个新的 [LzipArchive](../../com.aspose.zip/lziparchive) 实例。 |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | 初始化一个新的 [LzipArchive](../../com.aspose.zip/lziparchive) 实例。 |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | 初始化一个准备解压的 [LzipArchive](../../com.aspose.zip/lziparchive) 类的新实例。 |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | 初始化一个准备解压的 [LzipArchive](../../com.aspose.zip/lziparchive) 类的新实例。 |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | 初始化一个准备解压的 [LzipArchive](../../com.aspose.zip/lziparchive) 类的新实例。 |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | 初始化一个准备解压的 [LzipArchive](../../com.aspose.zip/lziparchive) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | 将 lzip 存档提取到文件。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将 lzip 存档提取到流。 |
| [extract(String path)](#extract-java.lang.String-) | 按路径将 lzip 存档提取到文件。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档内容提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 lzip 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getLength()](#getLength--) | 获取长度。 |
| [getName()](#getName--) | 原始文件的名称。 |
| [getSettings()](#getSettings--) | 获取特定 lzip 存档的设置。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取文件数据的未压缩大小（字节）。 |
| [save(File destination)](#save-java.io.File-) | 将 lzip 存档保存到提供的目标文件。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 将 lzip 存档保存到提供的流。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将 lzip 存档保存到提供的目标文件。 |
| [setSource(File file)](#setSource-java.io.File-) | 设置要在存档中压缩的内容。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 设置要在存档中压缩的内容。 |
| [setSource(String path)](#setSource-java.lang.String-) | 设置要在存档中压缩的内容。 |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


初始化一个新的 [LzipArchive](../../com.aspose.zip/lziparchive) 实例。

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


初始化一个新的 [LzipArchive](../../com.aspose.zip/lziparchive) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | 特定 lzip 存档的设置，包含字典大小的定义 |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


初始化一个准备解压的 [LzipArchive](../../com.aspose.zip/lziparchive) 类的新实例。

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

此构造函数不进行解压。请参阅用于解压的 [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | 加载存档的选项。 |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


初始化一个准备解压的 [LzipArchive](../../com.aspose.zip/lziparchive) 类的新实例。

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

此构造函数不进行解压。请参阅用于解压的 [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档源的路径 |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | 加载存档的选项。 |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


将 lzip 存档提取到文件。

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 用于存储解压后数据的流 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


按路径将 lzip 存档提取到文件。

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(\"extracted.bin\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.File | 将作为目标流打开的文件 |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


将 lzip 存档保存到提供的流。

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，它将被覆盖 |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


设置要在存档中压缩的内容。

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | java.io.InputStream | 存档的输入流 |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


设置要在存档中压缩的内容。

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

