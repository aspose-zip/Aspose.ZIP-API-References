---
title: "CabEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 cab 存档中的单个文件。"
type: docs
weight: 46
url: /zh/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

表示 cab 存档中的单个文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getModificationTime()](#getModificationTime--) | 获取最后修改的日期和时间。 |
| [getName()](#getName--) | 获取存档中条目的名称。 |
| [open()](#open--) | 打开条目进行提取，并提供包含条目内容的流。 |
| [toString()](#toString--) | 返回 [CabEntry](../../com.aspose.zip/cabentry) 类实例的字符串表示形式。 |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


将条目提取到提供的流中。

提取 CAB 存档的一个条目。

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
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

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |

**Returns:**
java.io.File - 复合文件的文件信息
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


获取最后修改的日期和时间。

**Returns:**
java.util.Date - 最后修改的日期和时间。
### getName() {#getName--}
```
public final String getName()
```


获取存档中条目的名称。

**Returns:**
java.lang.String - 存档中条目的名称
### open() {#open--}
```
public final InputStream open()
```


打开条目进行提取，并提供包含条目内容的流。

用法：

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
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


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
