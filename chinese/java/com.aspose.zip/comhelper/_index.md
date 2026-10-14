---
title: "ComHelper"
second_title: "Aspose.ZIP for Java API 参考"
description: "为 COM 客户端提供将存档加载到 Aspose.Zip 的方法。"
type: docs
weight: 55
url: /zh/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

为 COM 客户端提供将存档加载到 Aspose.Zip 的方法。

使用 ComHelper 类从文件或流加载归档。特定类提供默认构造函数来创建新归档，并提供重载构造函数以从文件或流加载归档。如果在 .NET 应用程序中使用 Aspose.Zip，您可以直接使用所有归档构造函数；但在 COM 应用程序中使用 Aspose.Zip 时，仅提供默认的归档构造函数。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ComHelper()](#ComHelper--) | 初始化此类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | 允许 COM 应用程序从流加载 bzip2 归档。 |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | 允许 COM 应用程序从文件加载 bzip2 归档。 |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | 允许 COM 应用程序从流加载 gzip 归档。 |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | 允许 COM 应用程序从文件加载 gzip 归档。 |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | 允许 COM 应用程序从流加载 rar 归档。 |
| [openRar(String fileName)](#openRar-java.lang.String-) | 允许 COM 应用程序从文件加载 rar 归档。 |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | 允许 COM 应用程序从流加载 ZIP 归档。 |
| [openZip(String fileName)](#openZip-java.lang.String-) | 允许 COM 应用程序从文件加载 ZIP 归档。 |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


初始化此类的新实例。

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


允许 COM 应用程序从流加载 bzip2 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | .NET 流对象，包含要加载的归档。 |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


允许 COM 应用程序从文件加载 bzip2 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 要加载的存档的文件名。 |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


允许 COM 应用程序从流加载 gzip 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | .NET 流对象，包含要加载的归档。 |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


允许 COM 应用程序从文件加载 gzip 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 要加载的存档的文件名。 |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


允许 COM 应用程序从流加载 rar 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | .NET 流对象，包含要加载的归档。 |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


允许 COM 应用程序从文件加载 rar 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 要加载的存档的文件名。 |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


允许 COM 应用程序从流加载 ZIP 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | .NET 流对象，包含要加载的归档。 |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


允许 COM 应用程序从文件加载 ZIP 归档。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | 要加载的存档的文件名。 |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
