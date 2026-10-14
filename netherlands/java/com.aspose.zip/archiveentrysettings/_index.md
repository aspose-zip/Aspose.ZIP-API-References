---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen die worden gebruikt om vermeldingen te comprimeren of te decomprimeren."
type: docs
weight: 30
url: /nl/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Instellingen die worden gebruikt om vermeldingen te comprimeren of te decomprimeren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Initialiseert een nieuw exemplaar van de [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) klasse. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Initialiseert een nieuw exemplaar van de [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) klasse. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Initialiseert een nieuw exemplaar van de [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getComment()](#getComment--) | Haalt de opmerking op voor het item binnen het ZIP-archief. |
| [getCompressionSettings()](#getCompressionSettings--) | Haalt de instellingen op voor compressie- of decompressieroutine. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Haalt de instellingen op voor versleuteling of ontsleuteling. |
| [setComment(String value)](#setComment-java.lang.String-) | Opmerking voor het item binnen het ZIP-archief. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Initialiseert een nieuw exemplaar van de [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) klasse.

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Initialiseert een nieuw exemplaar van de [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Instellingen voor compressie. Geef null door voor standaard deflate-instellingen. |

Kan een van deze zijn:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Initialiseert een nieuw exemplaar van de [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) klasse.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Instellingen voor compressie. Geef null door voor standaard deflate-instellingen. |

Kan een van deze zijn:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Instellingen voor encryptie. Geef null door als er geen encryptie of decryptie nodig is. |

Kan een van deze zijn:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Haalt de opmerking op voor het item binnen het ZIP-archief.

**Returns:**
java.lang.String - opmerking voor het item binnen het ZIP-archief.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Haalt de instellingen op voor compressie- of decompressieroutine.

Kan een van deze zijn:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Haalt de instellingen op voor versleuteling of ontsleuteling. De instellingen van een specifiek item kunnen variëren.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Opmerking voor het item binnen het ZIP-archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String |  |

