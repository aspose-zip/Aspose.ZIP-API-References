---
title: "SevenZipArchiveEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 7z 存档中的单个文件。"
type: docs
weight: 105
url: /zh/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

表示 7z 存档中的单个文件。

将一个 [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) 实例转换为 [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted)，以确定该条目是否已加密。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getCompressedSize()](#getCompressedSize--) | 获取压缩文件的大小。 |
| [getCompressionProgressed()](#getCompressionProgressed--) | 获取在原始流的一部分被压缩时触发的事件。 |
| [getCompressionSettings()](#getCompressionSettings--) | 获取压缩或解压缩的设置。 |
| [getLength()](#getLength--) | 获取长度。 |
| [getModificationTime()](#getModificationTime--) | 获取最后修改的日期和时间。 |
| [getName()](#getName--) | 获取存档中条目的名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取原始文件的大小。 |
| [isDirectory()](#isDirectory--) | 获取指示该条目是否为目录的值。 |
| [open()](#open--) | 打开条目进行提取，并提供包含条目内容的流。 |
| [open(String password)](#open-java.lang.String-) | 打开条目进行提取，并提供包含条目内容的流。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 设置在原始流的一部分被压缩时触发的事件。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到提供的流中。

使用密码提取 zip 归档的条目。

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流。必须可写。 |
| password | java.lang.String | 用于解密的可选密码 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


根据提供的路径将条目提取到文件系统中。

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(\"data.bin\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |
| password | java.lang.String | 用于解密的可选密码 |

**Returns:**
java.io.File - 已提取文件的信息
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


获取压缩文件的大小。

**Returns:**
long - 压缩文件的大小
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


获取在原始流的一部分被压缩时触发的事件。

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

从流中读取以获取文件的原始内容。参见示例部分。

**Returns:**
java.io.InputStream - 表示条目内容的流
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


打开条目进行提取，并提供包含条目内容的流。

用法：

```

``````

SevenZipArchive archive = new SevenZipArchive(\"archive.7z\");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

事件发送者是一个 [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) 实例。

对于 LZMA2 条目，在固实模式和多线程模式下不调用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 当原始流的一部分被压缩时触发的事件 |

