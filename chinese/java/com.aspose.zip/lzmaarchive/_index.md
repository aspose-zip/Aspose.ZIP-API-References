---
title: "LzmaArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 LZMA 存档文件。"
type: docs
weight: 86
url: /zh/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

此类表示 LZMA 存档文件。可用于创建或提取 LZMA 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | 初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，并以 lzma 格式创建存档。 |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | 初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，并以 lzma 格式创建存档。 |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | 初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，以进行解压缩。 |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | 初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，以进行解压缩。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | 将 lzma 存档提取到文件。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将 lzma 存档提取到流。 |
| [extract(String path)](#extract-java.lang.String-) | 通过路径将 lzma 存档提取到文件。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档内容提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 lzma 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getLength()](#getLength--) | 获取长度。 |
| [getName()](#getName--) | 原始文件的名称。 |
| [save(File destination)](#save-java.io.File-) | 将 lzma 存档保存到提供的目标文件。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 将 lzma 存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将 lzma 存档保存到提供的目标文件。 |
| [setSource(File file)](#setSource-java.io.File-) | 设置要在存档中压缩的内容。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 设置要在存档中压缩的内容。 |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | 设置要在存档中压缩的内容。 |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，并以 lzma 格式创建存档。

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，并以 lzma 格式创建存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | 特定 lzma 存档的设置集合 |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，以进行解压缩。

此构造函数不进行解压缩。请参阅 [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\\#extract-OutputStream-) 方法以进行解压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | java.io.InputStream | 存档的来源 |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


初始化 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 类的新实例，以进行解压缩。

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| file | java.io.File | 用于存储解压后数据的文件 |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将 lzma 存档提取到流。

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 用于存放解压后数据的文件路径 |

**Returns:**
java.io.File - 已提取文件的信息
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将存档内容提取到提供的目录。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | 用于放置解压文件的目录路径。 |

如果目录不存在，将会创建 |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成 lzma 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成 lzma 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


获取存档格式。

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


获取长度。

**Returns:**
java.lang.Long - 长度
### getName() {#getName--}
```
public final String getName()
```


原始文件的名称。

**Returns:**
java.lang.String - 原始文件的名称
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


将 lzma 存档保存到提供的目标文件。

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lzma\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | java.io.OutputStream | 目标流 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


将 lzma 存档保存到提供的目标文件。

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| file | java.io.File | 将作为输入流打开的文件 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


设置要在存档中压缩的内容。

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save(\"archive.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourcePath | java.lang.String | 文件路径，将作为输入流打开 |

