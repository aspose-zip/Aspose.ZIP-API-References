---
title: "AppleArchiveEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 . 中的文件或目录条目。"
type: docs
weight: 17
url: /zh/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

表示在 [AppleArchive](../../com.aspose.zip/applearchive) 中的文件或目录条目。

此类的实例可以表示从现有 Apple Archive 解析的条目，或添加到正在构建的归档中的条目。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 通过路径将 Apple 存档条目提取到文件系统。 |
| [getLength()](#getLength--) | 获取条目以字节为单位的未压缩长度。 |
| [getName()](#getName--) | 获取归档内条目的路径。 |
| [isDirectory()](#isDirectory--) | 获取指示该条目是否为目录的值。 |
| [open()](#open--) | 打开条目进行提取，并提供包含条目内容的流。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
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


通过路径将 Apple 存档条目提取到文件系统。

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
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


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
