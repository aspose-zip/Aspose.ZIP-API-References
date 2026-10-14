---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 ARJ 存档中的单个文件。"
type: docs
weight: 38
url: /zh/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

表示 ARJ 存档中的单个文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | 将 ARJ 存档条目提取到文件中。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 根据提供的路径将条目提取到文件系统中。 |
| [getCompressedSize()](#getCompressedSize--) | 获取压缩文件的大小。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getName()](#getName--) | 获取归档中条目的名称。 |
| [getUncompressedSize()](#getUncompressedSize--) | 获取原始文件的大小。 |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


将 ARJ 存档条目提取到文件中。

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 目标文件的路径。如果文件已存在，将被覆盖。 |

**Returns:**
java.io.File - 组合文件的文件信息
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


获取压缩文件的大小。

**Returns:**
long - 压缩文件的大小
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


获取归档中条目的名称。

**Returns:**
java.lang.String - 存档中条目的名称
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


获取原始文件的大小。

**Returns:**
long - 原始文件的大小
