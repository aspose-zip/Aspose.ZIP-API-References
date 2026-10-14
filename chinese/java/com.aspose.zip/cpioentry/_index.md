---
title: "CpioEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 cpio 存档中的单个文件。"
type: docs
weight: 58
url: /zh/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

表示 cpio 存档中的单个文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | 获取最后写入时间。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getName()](#getName--) | 获取存档中条目的名称。 |
| [getParent()](#getParent--) | 获取条目所属的存档。 |
| [isDirectory()](#isDirectory--) | 获取指示该条目是否为目录的值。 |
| [open()](#open--) | 打开条目进行提取，并提供包含条目内容的流。 |
| [toString()](#toString--) | 返回 [CpioEntry](../../com.aspose.zip/cpioentry) 类实例的字符串表示形式。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到提供的流中。

提取 cpio 存档的条目。

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
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

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |

**Returns:**
java.io.File - 已提取文件的信息
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


获取最后写入时间。

**Returns:**
java.util.Date - 最后写入时间
### getLength() {#getLength--}
```
public final Long getLength()
```


获取条目的字节长度。

**Returns:**
java.lang.Long - 条目的字节长度
### getName() {#getName--}
```
public final String getName()
```


获取存档中条目的名称。

**Returns:**
java.lang.String - 存档中条目的名称
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


获取条目所属的存档。

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


获取指示该条目是否为目录的值。

**Returns:**
boolean - 指示条目是否表示目录的值。
### open() {#open--}
```
public final InputStream open()
```


打开条目进行提取，并提供包含条目内容的流。

用法：

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
