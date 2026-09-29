---
title: "LzxArchiveEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 LZX 存档中的单个文件。"
type: docs
weight: 90
url: /zh/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

表示 LZX 存档中的单个文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 将 Lzx 存档条目提取到文件系统的指定路径。 |
| [getCommentary()](#getCommentary--) | 获取注释。 |
| [getCompressedSize()](#getCompressedSize--) | 获取压缩文件的大小。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getModificationTime()](#getModificationTime--) | 获取条目的最后修改时间。 |
| [getName()](#getName--) | 获取条目的名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取原始文件的大小。 |
| [isDirectory()](#isDirectory--) | 获取指示此条目是否为目录的值。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到提供的流中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 目标 | java.io.OutputStream | 目标流。必须可写。 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


将 Lzx 存档条目提取到文件系统的指定路径。

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
