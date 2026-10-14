---
title: "RarArchive"
second_title: "Aspose.ZIP for Java API 参考"
description: "此类表示 RAR 存档文件。"
type: docs
weight: 97
url: /zh/java/com.aspose.zip/rararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class RarArchive implements IArchive, AutoCloseable
```

此类表示 RAR 存档文件。使用它来提取 RAR 存档。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [RarArchive(String path)](#RarArchive-java.lang.String-) | 初始化 [RarArchive](../../com.aspose.zip/rararchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [RarArchive(String path, RarArchiveLoadOptions loadOptions)](#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-) | 初始化 [RarArchive](../../com.aspose.zip/rararchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [RarArchive(InputStream sourceStream)](#RarArchive-java.io.InputStream-) | 初始化 [RarArchive](../../com.aspose.zip/rararchive) 类的新实例，并构建可从存档中提取的条目列表。 |
| [RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)](#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-) | 初始化 [RarArchive](../../com.aspose.zip/rararchive) 类的新实例，并构建可从存档中提取的条目列表。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将存档中的所有文件提取到提供的目录。 |
| [getEntries()](#getEntries--) | 获取构成 rar 存档的 [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) 类型的条目。 |
| [getFileEntries()](#getFileEntries--) | 获取构成 rar 存档的 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 类型的条目。 |
| [getFormat()](#getFormat--) | 获取存档格式。 |
### RarArchive(String path) {#RarArchive-java.lang.String-}
```
public RarArchive(String path)
```


初始化 [RarArchive](../../com.aspose.zip/rararchive) 类的新实例，并构建可从存档中提取的条目列表。

以下示例提取存档，然后将第一个条目解压到 `MemoryStream`。

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (RarArchive archive = new RarArchive("data.rar")) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### RarArchive(String path, RarArchiveLoadOptions loadOptions) {#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(String path, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (RarArchive archive = new RarArchive("data.rar")) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

此构造函数不会解压任何条目。有关解压，请参阅 [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 存档文件的完全限定路径或相对路径。 |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | 用于加载现有存档的选项。 |

### RarArchive(InputStream sourceStream) {#RarArchive-java.io.InputStream-}
```
public RarArchive(InputStream sourceStream)
```


初始化 [RarArchive](../../com.aspose.zip/rararchive) 类的新实例，并构建可从存档中提取的条目列表。


以下示例对第一个条目进行解密并解压到 `MemoryStream`。

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
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

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions) {#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.


The following example decipher and decompress first entry to a `MemoryStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (RarArchive archive = new RarArchive(fs, options)) {
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

此构造函数不会解压任何条目。有关解压，请参阅 [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) 方法。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 存档的来源。 |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | 用于加载现有存档的选项。 |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将存档中的所有文件提取到提供的目录。

```

``````

try (RarArchive archive = new RarArchive("archive.rar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<RarArchiveEntry> getEntries()
```


Gets entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.

**Returns:**
java.util.List&lt;com.aspose.zip.RarArchiveEntry&gt; - entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
