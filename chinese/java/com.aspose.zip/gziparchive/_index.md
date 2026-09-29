---
title: "GzipArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 gzip 存档文件。"
type: docs
weight: 69
url: /zh/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

此类表示 gzip 归档文件。可用于创建或提取 gzip 归档。

Gzip 压缩算法基于 DEFLATE 算法，它是 LZ77 与 Huffman 编码的组合。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | 初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于压缩。 |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | 初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于解压缩。 |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | 初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于解压缩。 |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | 初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于解压缩。 |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | 初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于解压缩。 |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | 初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例。 |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | 初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将存档提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 将存档提取到指定路径的文件中。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档内容提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 gzip 归档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getLength()](#getLength--) | 获取原始文件的大小。 |
| [getName()](#getName--) | 原始文件的名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取原始文件的大小。 |
| [open()](#open--) | 打开存档进行提取，并提供包含存档内容的流。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 将存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件中。 |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | 设置要在存档中压缩的内容。 |
| [setSource(File file)](#setSource-java.io.File-) | 设置要在存档中压缩的内容。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 设置要在存档中压缩的内容。 |
| [setSource(String path)](#setSource-java.lang.String-) | 设置要在存档中压缩的内容。 |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于压缩。

以下示例展示了如何压缩文件。

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save(\"archive.gz\");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

此构造函数不进行解压缩。请参阅用于解压缩的 [open()](../../com.aspose.zip/gziparchive\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源。 |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于解压缩。

从流打开归档并将其提取到 `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get(\"archive.gz\")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

此构造函数不进行解压缩。请参阅用于解压缩的 [open()](../../com.aspose.zip/gziparchive\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源。 |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | 加载存档的选项。 |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例，用于解压缩。

通过路径打开文件中的存档并将其提取到 `MemoryStream`。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

此构造函数不进行解压缩。请参阅用于解压缩的 [open()](../../com.aspose.zip/gziparchive\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径。 |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


初始化一个新的 [GzipArchive](../../com.aspose.zip/gziparchive) 类实例。

通过路径打开文件中的存档并将其提取到 `MemoryStream`。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流。必须可写。 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


将存档提取到指定路径的文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |

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

如果目录不存在，它将被创建。 |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


获取构成 gzip 归档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成 gzip 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。
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


获取原始文件的大小。

在解压缩过程中，此属性可能包含不正确的大小。如果未压缩文件大小超过 4GB，由于标头中的 32 位限制，此属性将给出错误的值。

**Returns:**
java.lang.Long - 原始文件的大小
### getName() {#getName--}
```
public final String getName()
```


原始文件的名称。

**Returns:**
java.lang.String - 原始文件的名称
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


获取原始文件的大小。

在解压缩过程中，此属性可能包含不正确的大小。如果未压缩文件大小超过 4GB，由于标头中的 32 位限制，此属性将给出错误的值。

**Returns:**
long - 原始文件的大小。
### open() {#open--}
```
public final InputStream open()
```


打开存档进行提取，并提供包含存档内容的流。

提取归档并将提取的内容复制到文件流。

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | 目标流。 |

`outputStream` 必须是可写的。 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


将存档保存到提供的目标文件中。

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save(\"archive.gz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

使用此方法组合联合 tar.gz 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | 待压缩的 Tar 存档。 |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


设置要在存档中压缩的内容。

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"archive.gz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | java.io.InputStream | 存档的输入流。 |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


设置要在存档中压缩的内容。

通过路径打开文件中的存档并将其提取到 `MemoryStream`。

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save(\"archive.gz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

