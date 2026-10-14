---
title: "XarFileEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 xar 存档中的文件条目。"
type: docs
weight: 141
url: /zh/java/com.aspose.zip/xarfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class XarFileEntry extends XarEntry implements IArchiveFileEntry
```

表示 xar 存档中的文件条目。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getCompressionProgressed()](#getCompressionProgressed--) | 获取在原始流的一部分被压缩时触发的事件。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [open()](#open--) | 打开条目进行提取，并提供包含条目内容的流。 |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 设置在原始流的一部分被压缩时触发的事件。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到提供的流中。

提取 wim 归档的条目。

```

``````

try (FileOutputStream output = new FileOutputStream("file")){
try (XarArchive archive = new XarArchive("archive.xar")) {
((XarFileEntry)archive.getEntries().get(0)).extract(output);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         ((XarFileEntry)archive.getEntries().get(0)).extract("data.bin");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |

**Returns:**
java.io.File - 已提取文件的信息
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

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

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
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


设置在原始流的一部分被压缩时触发的事件。

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

