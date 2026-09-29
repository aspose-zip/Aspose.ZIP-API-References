---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP for Java API 参考"
description: "检测存档格式并提供其他相关信息。"
type: docs
weight: 32
url: /zh/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

检测存档格式并提供其他相关信息。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | 初始化一个新的 [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) 类实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | 获取格式信息。 |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | 获取格式信息。 |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


初始化一个新的 [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) 类实例。

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


获取格式信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 归档文件的流。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


获取格式信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 归档文件的文件名。 |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
