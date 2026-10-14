---
title: "Lz4Archive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 LZ4 存档文件。"
type: docs
weight: 80
url: /zh/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

此类表示 LZ4 存档文件。可用于提取或组合 LZ4 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | 初始化一个用于解压的 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。 |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | 初始化一个用于解压的 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。 |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | 初始化一个 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。 |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | 初始化一个 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。 |
| [Lz4Archive()](#Lz4Archive--) | 初始化一个用于压缩的 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。 |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | 初始化一个用于压缩的 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将存档提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 将存档提取到指定路径的文件中。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档内容提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getLength()](#getLength--) | 获取长度。 |
| [getName()](#getName--) | 获取原始名称。 |
| [open()](#open--) | 打开存档进行提取，并提供包含存档内容的流。 |
| [save(File destination)](#save-java.io.File-) | 将 lz4 存档保存到提供的目标文件。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 将 lz4 存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件中。 |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | 设置要在存档中压缩的内容。 |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | 设置要在存档中压缩的内容。 |
| [setSource(File fileInfo)](#setSource-java.io.File-) | 设置要在存档中压缩的内容。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 设置要在存档中压缩的内容。 |
| [setSource(String path)](#setSource-java.lang.String-) | 设置要在存档中压缩的内容。 |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


初始化一个用于解压的 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。

从流中打开存档并将其提取到 `MemoryStream`。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream(\"archive.lz4\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

此构造函数不执行解压。请参阅用于解压的 [open()](../../com.aspose.zip/lz4archive\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | 加载存档时的选项。 |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


初始化一个 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。

通过路径打开文件中的存档并将其提取到 `MemoryStream`。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

此构造函数不执行解压。请参阅用于解压的 [open()](../../com.aspose.zip/lz4archive\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径 |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | 加载存档时的选项。 |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


初始化一个用于压缩的 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


初始化一个用于压缩的 [Lz4Archive](../../com.aspose.zip/lz4archive) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | 已组合存档的设置。 |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将存档提取到提供的流中。

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
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


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

从流中读取以获取文件的原始内容。请参阅示例部分。

**Returns:**
java.io.InputStream - 表示存档内容的流
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


将 lz4 存档保存到提供的目标文件。

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lz4\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | java.io.OutputStream | 目标流。 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


将存档保存到提供的目标文件中。

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource("data.bin");
archive.save(\"archive.lz4\");
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
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

使用此方法组合联合的 tar.lz4 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | 待压缩的 Tar 存档。 |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


设置要在存档中压缩的内容。

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileInfo | java.io.File | 要压缩的文件的引用。 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


设置要在存档中压缩的内容。

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.lz4\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 要压缩的文件的路径。 |

