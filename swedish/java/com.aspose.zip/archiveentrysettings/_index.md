---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar som används för att komprimera eller dekomprimera poster."
type: docs
weight: 30
url: /sv/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Inställningar som används för att komprimera eller dekomprimera poster.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Initierar en ny instans av klassen [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Initierar en ny instans av klassen [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Initierar en ny instans av klassen [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getComment()](#getComment--) | Hämtar kommentar för posten i ZIP-arkivet. |
| [getCompressionSettings()](#getCompressionSettings--) | Hämtar inställningar för komprimerings- eller dekomprimeringsrutin. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Hämtar inställningar för kryptering eller dekryptering. |
| [setComment(String value)](#setComment-java.lang.String-) | Kommentar för posten i ZIP-arkivet. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Initierar en ny instans av klassen [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Initierar en ny instans av klassen [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Inställningar för komprimering. Skicka null för standard deflate-inställningar. |

Kan vara en av dessa:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Initierar en ny instans av klassen [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Inställningar för komprimering. Skicka null för standard deflate-inställningar. |

Kan vara en av dessa:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Inställningar för kryptering. Skicka null om det inte behövs att kryptera eller dekryptera. |

Kan vara en av dessa:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Hämtar kommentar för posten i ZIP-arkivet.

**Returns:**
java.lang.String - kommentar för posten i ZIP-arkivet.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Hämtar inställningar för komprimerings- eller dekomprimeringsrutin.

Kan vara en av dessa:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Hämtar inställningar för kryptering eller dekryptering. Inställningarna för en specifik post kan variera.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Kommentar för posten i ZIP-arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

