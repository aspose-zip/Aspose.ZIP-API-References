---
title: "XzArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 xz 存档文件。"
type: docs
weight: 146
url: /zh/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

此类表示 xz 存档文件。可用于创建和提取 xz 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XzArchive()](#XzArchive--) | 初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，并以 xz 格式创建存档。 |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | 初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，并以 xz 格式创建存档。 |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | 初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。 |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | 初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。 |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | 初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。 |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | 初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | 将 xz 存档提取到文件。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将 xz 存档提取到流。 |
| [extract(String path)](#extract-java.lang.String-) | 按路径将 xz 存档提取到文件。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档内容提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 xz 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getName()](#getName--) | 获取存档中条目的名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取文件数据的未压缩大小（字节）。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 将 xz 存档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将 xz 存档保存到提供的目标文件中。 |
| [setSource(File file)](#setSource-java.io.File-) | 设置要在存档中压缩的内容。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 设置要在存档中压缩的内容。 |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | 设置要在存档中压缩的内容。 |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，并以 xz 格式创建存档。

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，并以 xz 格式创建存档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | 特定 xz 归档的设置集合：字典大小、块大小、校验类型 |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。

此构造函数不进行解压。请参阅用于解压的 [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | java.io.InputStream | 存档的来源 |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。

此构造函数不进行解压。请参阅用于解压的 [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | java.io.InputStream | 存档的来源 |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | 加载存档的选项。 |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。

此构造函数不进行解压。请参阅用于解压的 [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档源的路径 |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


初始化 [XzArchive](../../com.aspose.zip/xzarchive) 类的新实例，以便进行解压缩。

此构造函数不进行解压。请参阅用于解压的 [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档源的路径 |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


将 xz 存档提取到文件。

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
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


按路径将 xz 存档提取到文件。

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(\"extracted.bin\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
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


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


将 xz 存档保存到提供的目标文件中。

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("result.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| file | java.io.File | 文件，将作为输入流打开 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


设置要在存档中压缩的内容。

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourcePath | java.lang.String | 将作为输入流打开的文件的路径 |

