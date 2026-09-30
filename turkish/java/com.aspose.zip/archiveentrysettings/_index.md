---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Girişleri sıkıştırmak veya açmak için kullanılan ayarlar."
type: docs
weight: 30
url: /tr/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Girişleri sıkıştırmak veya açmak için kullanılan ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Yeni bir [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) sınıfı örneği başlatır. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Yeni bir [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) sınıfı örneği başlatır. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Yeni bir [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getComment()](#getComment--) | ZIP arşivindeki giriş için yorumu alır. |
| [getCompressionSettings()](#getCompressionSettings--) | Sıkıştırma veya açma rutinine ait ayarları alır. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Şifreleme veya şifre çözme ayarlarını alır. |
| [setComment(String value)](#setComment-java.lang.String-) | ZIP arşivindeki giriş için yorum. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Yeni bir [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) sınıfı örneği başlatır.

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Yeni bir [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Sıkıştırma ayarları. Varsayılan deflate ayarları için null geçin. |

Bunlardan biri olabilir:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Yeni bir [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Sıkıştırma ayarları. Varsayılan deflate ayarları için null geçin. |

Bunlardan biri olabilir:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Şifreleme ayarları. Şifreleme veya şifre çözme ihtiyacınız yoksa null geçin. |

Bunlardan biri olabilir:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


ZIP arşivindeki giriş için yorumu alır.

**Returns:**
java.lang.String - ZIP arşivindeki giriş için yorum.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Sıkıştırma veya açma rutinine ait ayarları alır.

Bunlardan biri olabilir:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Şifreleme veya şifre çözme ayarlarını alır. Belirli bir girdinin ayarları değişebilir.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


ZIP arşivindeki giriş için yorum.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

