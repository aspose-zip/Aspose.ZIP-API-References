---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于压缩或解压条目的设置。"
type: docs
weight: 30
url: /zh/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

用于压缩或解压条目的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | 初始化 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 类的新实例。 |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | 初始化 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 类的新实例。 |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | 初始化 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getComment()](#getComment--) | 获取 ZIP 存档中条目的注释。 |
| [getCompressionSettings()](#getCompressionSettings--) | 获取压缩或解压例程的设置。 |
| [getEncryptionSettings()](#getEncryptionSettings--) | 获取加密或解密的设置。 |
| [setComment(String value)](#setComment-java.lang.String-) | ZIP 存档中条目的注释。 |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


初始化 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 类的新实例。

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


初始化 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | 压缩设置。若使用默认 deflate 设置，请传入 null。 |

可以是以下之一：

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


初始化 [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | 压缩设置。若使用默认 deflate 设置，请传入 null。 |

可以是以下之一：

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | 加密设置。如果不需要加密或解密，请传入 null。 |

可以是以下之一：

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


获取 ZIP 存档中条目的注释。

**Returns:**
java.lang.String - ZIP 存档中条目的注释。
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


获取压缩或解压例程的设置。

可以是以下之一：

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


获取加密或解密的设置。特定条目的设置可能会有所不同。

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


ZIP 存档中条目的注释。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

