---
title: "ZArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 Z 压缩归档文件。"
type: docs
weight: 153
url: /zh/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

此类表示 Z（压缩）归档文件。可用于创建或提取 Z 归档。

参见 [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ZArchive()](#ZArchive--) | 初始化一个用于压缩的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。 |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | 初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。 |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | 初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。 |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | 初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。 |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | 初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | 将 Z 归档提取到文件。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将 Z 归档提取到流。 |
| [extract(String path)](#extract-java.lang.String-) | 通过路径将 Z 归档提取到文件。 |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档内容提取到提供的目录。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 Z 归档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getName()](#getName--) | 获取存档中条目的名称。 |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 将 Z 归档保存到提供的流中。 |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | 将 Z 归档保存到提供的流中。 |
| [save(String destinationFileName)](#save-java.lang.String-) | 将 Z 存档保存到提供的目标文件。 |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | 将 Z 存档保存到提供的目标文件。 |
| [setSource(File file)](#setSource-java.io.File-) | 设置要在存档中压缩的内容。 |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 设置要在存档中压缩的内容。 |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | 设置要在存档中压缩的内容。 |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


初始化一个用于压缩的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。

此构造函数不进行解压缩。请参阅 [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) 方法以进行解压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | java.io.InputStream | 存档的来源 |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。

此构造函数不进行解压缩。请参阅 [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) 方法以进行解压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | java.io.InputStream | 存档的来源 |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | 用于加载存档的选项。 |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。

此构造函数不进行解压缩。请参阅 [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) 方法以进行解压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档源的路径 |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


初始化一个用于解压的 [ZArchive](../../com.aspose.zip/zarchive) 类的新实例。

此构造函数不进行解压缩。请参阅 [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) 方法以进行解压缩。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档源的路径 |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | 用于加载存档的选项。 |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


将 Z 归档提取到文件。

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
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


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


通过路径将 Z 归档提取到文件。

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract(\"extracted.bin\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

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
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 输出 | java.io.OutputStream | 目标流 |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


将 Z 归档保存到提供的流中。

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 要创建的存档的路径。如果指定的文件名指向已存在的文件，它将被覆盖 |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


将 Z 存档保存到提供的目标文件。

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| file | java.io.File | 将作为输入流打开的文件信息 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


设置要在存档中压缩的内容。

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourcePath | java.lang.String | 将作为输入流打开的文件路径 |

