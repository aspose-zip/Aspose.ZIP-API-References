---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示有关存档实例的信息。"
type: docs
weight: 34
url: /zh/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

表示有关存档实例的信息。
## 方法

| 方法 | 描述 |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | 获取一个值，指示归档中条目（文件）的名称是否已加密。 |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | 获取归档格式信息。 |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | 获取归档格式信息。 |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | 获取归档实例信息。 |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | 获取归档实例信息。 |
| [getFormatInfo()](#getFormatInfo--) | 获取归档格式信息。 |
| [isContentEncrypted()](#isContentEncrypted--) | 获取一个值，指示存档的内容是否已加密。 |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


获取一个值，指示归档中条目（文件）的名称是否已加密。

**Returns:**
boolean - 一个值，指示存档中条目（文件）的名称是否已加密。
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


获取归档格式信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 归档文件的流。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


获取归档格式信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 归档文件的文件名。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


获取归档实例信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 归档文件的流。 |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


获取归档实例信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 归档文件的文件名。 |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


获取归档格式信息。

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


获取一个值，指示存档的内容是否已加密。

**Returns:**
boolean - 一个值，指示存档的内容是否已加密。
