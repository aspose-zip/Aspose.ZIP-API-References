---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 Lha 存档中的单个文件。"
type: docs
weight: 76
url: /zh/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

表示 Lha 存档中的单个文件。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | 将 Lha 归档条目提取到文件。 |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 将条目提取到提供的流中。 |
| [extract(String path)](#extract-java.lang.String-) | 按路径将 Lha 归档条目提取到文件系统。 |
| [getLastModified()](#getLastModified--) | 获取条目的最后修改时间。 |
| [getLength()](#getLength--) | 获取条目的字节长度。 |
| [getModificationTime()](#getModificationTime--) | 获取条目的最后修改时间。 |
| [getName()](#getName--) | 获取条目的名称。 |
| [getPath()](#getPath--) | 获取条目的完整路径。 |
| [isDirectory()](#isDirectory--) | 获取指示此条目是否为目录的值。 |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


将 Lha 归档条目提取到文件。

```

``````

try (FileInputStream lhaFile = new FileInputStream(\"archive.lha\")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| path | java.lang.String | 用于存放解压后数据的文件路径 |

**Returns:**
java.io.File - 包含提取数据的 java.io.File 实例
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


获取条目的最后修改时间。

**Returns:**
java.util.Date - 条目的最后修改时间
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


获取条目的最后修改时间。

**Returns:**
java.util.Date - 条目的最后修改时间
### getName() {#getName--}
```
public final String getName()
```


获取条目的名称。

仅用于压缩的归档，例如 gzip、bzip2、lzip、lzma、xz、z，如果在头部找不到其他名称，则名称为 \"File.bin\"。

**Returns:**
java.lang.String - 条目的名称
### getPath() {#getPath--}
```
public final String getPath()
```


获取条目的完整路径。

**Returns:**
java.lang.String - 条目的完整路径
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


获取指示此条目是否为目录的值。

**Returns:**
boolean - 指示此条目是否为目录的值。
