---
title: SevenZipEntrySettings
second_title: Aspose.ZIP for Java API Reference
description: Settings used to compress or decompress 7z entries.
type: docs
weight: 79
url: /java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Settings used to compress or decompress 7z entries.
## Constructors

| Constructor | Description |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Initializes a new instance of the [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) class. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Initializes a new instance of the [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) class. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Initializes a new instance of the [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Gets value indicating whether to compress archive header. |
| [getCompressionSettings()](#getCompressionSettings--) | Gets settings for compression or decompression routine. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Gets settings for encryption or decryption. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Sets value indicating whether to compress archive header. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Initializes a new instance of the [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) class.

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Initializes a new instance of the [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | settings for compression. Pass null for default LZMA settings.

Can be one of these:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Initializes a new instance of the [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | settings for compression. Pass null for default LZMA settings.

Can be one of these:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
| encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | settings for encryption. Pass null if no need to encrypt or decrypt.

Can be only one:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Gets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Returns:**
boolean - value indicating whether to compress archive header
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression routine.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Gets settings for encryption or decryption. Settings of particular entry may vary.

The [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) is only option of 7z archives.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
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

