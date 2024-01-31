---
title: ArchiveEntrySettings
second_title: Aspose.ZIP for Java API Reference
description: Settings used to compress or decompress entries.
type: docs
weight: 15
url: /java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Settings used to compress or decompress entries.
## Constructors

| Constructor | Description |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Initializes a new instance of the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) class. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Initializes a new instance of the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) class. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Initializes a new instance of the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Gets settings for compression or decompression routine. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Gets settings for encryption or decryption. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Initializes a new instance of the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) class.

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Initializes a new instance of the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Settings for compression. Pass null for default deflate settings.

Can be one of these:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Initializes a new instance of the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Settings for compression. Pass null for default deflate settings.

Can be one of these:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
| encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Settings for encryption. Pass null if no need to encrypt or decrypt.

Can be one of these:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression routine.

Can be one of these:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Gets settings for encryption or decryption. Settings of particular entry may vary.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
