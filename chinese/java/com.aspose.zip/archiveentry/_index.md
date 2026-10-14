---
title: "ArchiveEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示存档中的单个文件。"
type: docs
weight: 27
url: /zh/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

表示存档中的单个文件。

将 [ArchiveEntry](../../com.aspose.zip/archiveentry) 实例转换为 [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted)，以确定该条目是否已加密。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getComment()](#getComment--) | 获取存档中条目的注释。 |
| [getCompressedSize()](#getCompressedSize--) | 获取压缩文件的大小。 |
| [getCompressionProgressed()](#getCompressionProgressed--) | 获取在原始流的一部分被压缩时触发的事件。 |
| [getCompressionSettings()](#getCompressionSettings--) | 获取压缩或解压缩的设置。 |
| [getDataSource()](#getDataSource--) | 如果条目是添加到存档而非提取，则为该条目的来源。 |
| [getExtractionProgressed()](#getExtractionProgressed--) | 获取在提取原始流的一部分时触发的事件。 |
| [getLength()](#getLength--) | 获取长度。 |
| [getModificationTime()](#getModificationTime--) | 获取最后修改的日期和时间。 |
| [getName()](#getName--) | 获取归档中条目的名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取原始文件的大小。 |
| [isDirectory()](#isDirectory--) | 获取指示该条目是否为目录的值。 |
| [open()](#open--) | 打开条目进行提取，并提供包含解压后条目内容的流。 |
| [open(String password)](#open-java.lang.String-) | 打开条目进行提取，并提供包含解压后条目内容的流。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 设置在原始流的一部分被压缩时触发的事件。 |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | 设置在提取原始流的一部分时触发的事件。 |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | 设置最后修改的日期和时间。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到提供的流中。

使用密码提取 zip 归档的条目。

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流。必须可写。 |
| password | java.lang.String | 可选的解密密码。 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


根据提供的路径将条目提取到文件系统中。

提取 ZIP 归档的两个条目，每个都有各自的密码

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |
| password | java.lang.String | 可选的解密密码。 |

**Returns:**
java.io.File - 已提取文件的信息
### getComment() {#getComment--}
```
public final String getComment()
```


获取存档中条目的注释。

**Returns:**
java.lang.String - 归档中条目的注释
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

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

在此示例中，事件处理程序用于在提取条目前一百兆字节后进行取消。

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
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


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

从流中读取以获取文件的原始内容。

**Returns:**
java.io.InputStream - 表示条目内容的流。
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


打开条目进行提取，并提供包含解压后条目内容的流。


用法：

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
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

事件发送者是一个 [ArchiveEntry](../../com.aspose.zip/archiveentry) 实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 当原始流的一部分被压缩时触发的事件 |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


设置在提取原始流的一部分时触发的事件。

在此示例中，事件处理程序用于计算已处理大小的百分比份额。

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

事件发送者是一个 [ArchiveEntry](../../com.aspose.zip/archiveentry) 实例。可以取消提取。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | 当原始流的一部分被提取时触发的事件 |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


设置最后修改的日期和时间。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 最后修改日期和时间 |

