---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于压缩或解压 7z 条目的设置。"
type: docs
weight: 113
url: /zh/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

用于压缩或解压 7z 条目的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | 初始化 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 类的新实例。 |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | 初始化 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 类的新实例。 |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | 初始化 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | 获取指示是否压缩存档头的值。 |
| [getCompressionSettings()](#getCompressionSettings--) | 获取压缩或解压例程的设置。 |
| [getEncryptionSettings()](#getEncryptionSettings--) | 获取加密或解密的设置。 |
| [getSolid()](#getSolid--) | 获取指示是否连接条目并将其视为单个数据块的值。 |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | 设置指示是否压缩存档头的值。 |
| [setSolid(boolean value)](#setSolid-boolean-) | 设置指示是否连接条目并将其视为单个数据块的值。 |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


初始化 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 类的新实例。

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


初始化 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | 压缩设置。若使用默认 LZMA 设置，请传入 null。 |

可以是以下之一：

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


初始化 [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | 压缩设置。若使用默认 LZMA 设置，请传入 null。 |

可以是以下之一：

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | 加密设置。如果不需要加密或解密，请传入 null。 |

只能是以下之一：

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


获取指示是否压缩存档头的值。

此设置等同于 7-Zip 工具的 `-mhc=on` 开关。目前，它与头部加密不兼容。

**Returns:**
布尔型 - 指示是否压缩存档头的值
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


获取压缩或解压例程的设置。

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


获取加密或解密的设置。特定条目的设置可能会有所不同。

该 [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) 是 7z 存档的唯一选项。

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


获取指示是否连接条目并将其视为单个数据块的值。

以下示例展示了如何将目录压缩为使用 LZMA2 压缩且不加密的固实 7z 存档。

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
settings.setSolid(true);
try (SevenZipArchive archive = new SevenZipArchive(settings)) {
archive.createEntries("C:\\Documents");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

**Returns:**
boolean - value indicating whether to concatenate entries and treat them as a single data block.
### setCompressHeader(boolean value) {#setCompressHeader-boolean-}
```
public final void setCompressHeader(boolean value)
```


Sets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to compress archive header |

### setSolid(boolean value) {#setSolid-boolean-}
```
public final void setSolid(boolean value)
```


Sets value indicating whether to concatenate entries and treat them as a single data block.

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
         settings.setSolid(true);
         try (SevenZipArchive archive = new SevenZipArchive(settings)) {
             archive.createEntries("C:\\Documents");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

在实例化存档时提供用于固实 7z 存档的 `SevenZipEntrySettings`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 指示是否连接条目并将其视为单个数据块的值。 |

