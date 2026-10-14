---
title: "TarEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 tar 存档中的单个文件。"
type: docs
weight: 126
url: /zh/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

表示 tar 存档中的单个文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getModificationTime()](#getModificationTime--) | 获取文件或目录的修改时间。 |
| [getName()](#getName--) | 获取存档中条目的名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取原始文件的大小。 |
| [isDirectory()](#isDirectory--) | 获取指示该条目是否为目录的值。 |
| [open()](#open--) | 打开条目进行提取，并提供包含条目内容的流。 |
| [setName(String value)](#setName-java.lang.String-) | 设置存档中条目的名称。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到提供的流中。

提取 tar 存档中的条目。

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |

**Returns:**
java.io.File - 已提取文件的信息
### getLength() {#getLength--}
```
public final Long getLength()
```


获取条目的字节长度。

**Returns:**
java.lang.Long - 条目的字节长度
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


获取文件或目录的修改时间。

**Returns:**
java.util.Date - 文件或目录的修改时间。
### getName() {#getName--}
```
public final String getName()
```


获取存档中条目的名称。

**Returns:**
java.lang.String - 存档中条目的名称
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


获取原始文件的大小。

具有与 `Length` 相同的值（[getLength](../../com.aspose.zip/tarentry\#getLength--)）

**Returns:**
long - 原始文件的大小。
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


获取指示该条目是否为目录的值。

**Returns:**
boolean - 表示该条目是否为目录的值
### open() {#open--}
```
public final InputStream open()
```


打开条目进行提取，并提供包含条目内容的流。


用法：

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

