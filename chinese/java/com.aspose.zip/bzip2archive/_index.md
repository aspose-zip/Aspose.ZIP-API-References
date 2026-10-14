---
title: "Bzip2Archive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 bzip2 存档文件。"
type: docs
weight: 40
url: /zh/java/com.aspose.zip/bzip2archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Bzip2Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

此类表示 bzip2 存档文件。可用于创建或提取 bzip2 存档。

bzip2 使用 Burrows-Wheeler 块排序文本压缩算法和哈夫曼编码来压缩文件。查看更多: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Bzip2Archive()](#Bzip2Archive--) | 初始化用于压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。 |
| [Bzip2Archive(InputStream sourceStream)](#Bzip2Archive-java.io.InputStream-) | 初始化用于解压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。 |
| [Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-) | 初始化用于解压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。 |
| [Bzip2Archive(String path)](#Bzip2Archive-java.lang.String-) | 初始化用于解压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。 |
| [Bzip2Archive(String path, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-) | 初始化用于解压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将存档提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 将存档提取到指定路径的文件中。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档内容提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 bzip2 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getLength()](#getLength--) | 获取长度。 |
| [getName()](#getName--) | 原始文件的名称。 |
| [open()](#open--) | 打开存档进行提取，并提供包含存档内容的流。 |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 将存档保存到提供的流中。 |
| [save(OutputStream outputStream, Bzip2SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-) | 将存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将存档保存到提供的目标文件中。 |
| [save(String destinationFileName, Bzip2SaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-) | 将存档保存到提供的目标文件中。 |
| [setSource(CpioArchive cpioArchive)](#setSource-com.aspose.zip.CpioArchive-) | 设置要在存档中压缩的内容。 |
| [setSource(CpioArchive cpioArchive, CpioFormat format)](#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-) | 设置要在存档中压缩的内容。 |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | 设置要在存档中压缩的内容。 |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | 设置要在存档中压缩的内容。 |
| [setSource(File file)](#setSource-java.io.File-) | 设置要在存档中压缩的内容。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 设置要在存档中压缩的内容。 |
| [setSource(String path)](#setSource-java.lang.String-) | 设置要在存档中压缩的内容。 |
### Bzip2Archive() {#Bzip2Archive--}
```
public Bzip2Archive()
```


初始化用于压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。

以下示例展示了如何压缩文件。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save("archive.bz2");
}
 
```



### Bzip2Archive(InputStream sourceStream) {#Bzip2Archive-java.io.InputStream-}
```
public Bzip2Archive(InputStream sourceStream)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

此构造函数不进行解压缩。请参阅用于解压缩的 [open()](../../com.aspose.zip/bzip2archive\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源 |

### Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)
```


初始化用于解压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。

从流打开归档并将其提取到 `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

### Bzip2Archive(String path) {#Bzip2Archive-java.lang.String-}
```
public Bzip2Archive(String path)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

此构造函数不进行解压缩。请参阅用于解压缩的 [open()](../../com.aspose.zip/bzip2archive\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的路径 |

### Bzip2Archive(String path, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(String path, Bzip2LoadOptions loadOptions)
```


初始化用于解压缩的 [Bzip2Archive](../../com.aspose.zip/bzip2archive) 类的新实例。

通过路径打开文件中的存档并将其提取到 `MemoryStream`。

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

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

     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
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


获取构成 bzip2 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 构成 bzip2 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目
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
### open() {#open--}
```
public final InputStream open()
```


打开存档进行提取，并提供包含存档内容的流。


用法：

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to an output stream.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| outputStream | java.io.OutputStream | 目标流。 |

### save(OutputStream outputStream, Bzip2SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(OutputStream outputStream, Bzip2SaveOptions saveOptions)
```


将存档保存到提供的流中。

将压缩数据写入输出流。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream. |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

Writes compressed data to file.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bz2");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，它将被覆盖 |

### save(String destinationFileName, Bzip2SaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(String destinationFileName, Bzip2SaveOptions saveOptions)
```


将存档保存到提供的目标文件中。

将压缩数据写入文件。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### setSource(CpioArchive cpioArchive) {#setSource-com.aspose.zip.CpioArchive-}
```
public final void setSource(CpioArchive cpioArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (CpioArchive cpioArchive = new CpioArchive()) {
         cpioArchive.createEntry("first.bin", "data1.bin");
         cpioArchive.createEntry("second.bin", "data2.bin");
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(cpioArchive);
             bzippedArchive.save("archive.cpio.bz2");
         }
     }
 
```

使用此方法组合联合 cpio.bz2 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | 待压缩的 cpio 存档 |

### setSource(CpioArchive cpioArchive, CpioFormat format) {#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-}
```
public final void setSource(CpioArchive cpioArchive, CpioFormat format)
```


设置要在存档中压缩的内容。

```

``````

try (CpioArchive cpioArchive = new CpioArchive()) {
cpioArchive.createEntry("first.bin", "data1.bin");
cpioArchive.createEntry("second.bin", "data2.bin");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(cpioArchive);
bzippedArchive.save("archive.cpio.bz2");
}
}
 
```

Use this method to compose joint cpio.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | cpio archive to be compressed |
| format | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

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
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(tarArchive);
             bzippedArchive.save("archive.tar.bz2");
         }
     }
 
```

使用此方法组合联合 tar.bz2 存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | 待压缩的 tar 存档 |

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
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(tarArchive);
bzippedArchive.save("archive.tar.bz2");
}
}
 
```

Use this method to compose joint tar.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | tar archive to be compressed |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| file | java.io.File | 待压缩文件的引用 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


设置要在存档中压缩的内容。

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 要压缩的文件路径 |

