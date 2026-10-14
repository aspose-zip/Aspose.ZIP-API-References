---
title: "ArchiveEntrySettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres utilisés pour compresser ou décompresser les entrées."
type: docs
weight: 30
url: /fr/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Paramètres utilisés pour compresser ou décompresser les entrées.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Initialise une nouvelle instance de la classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Initialise une nouvelle instance de la classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Initialise une nouvelle instance de la classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getComment()](#getComment--) | Obtient le commentaire de l'entrée dans l'archive ZIP. |
| [getCompressionSettings()](#getCompressionSettings--) | Obtient les paramètres pour la routine de compression ou de décompression. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Obtient les paramètres pour le chiffrement ou le déchiffrement. |
| [setComment(String value)](#setComment-java.lang.String-) | Commentaire de l'entrée dans l'archive ZIP. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Initialise une nouvelle instance de la classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Initialise une nouvelle instance de la classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Paramètres pour la compression. Passez null pour les paramètres de déflation par défaut. |

Peut être l'un de ceux-ci :

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Initialise une nouvelle instance de la classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Paramètres pour la compression. Passez null pour les paramètres de déflation par défaut. |

Peut être l'un de ceux-ci :

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Paramètres pour le chiffrement. Passez null s'il n'est pas nécessaire de chiffrer ou déchiffrer. |

Peut être l'un de ceux-ci :

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Obtient le commentaire de l'entrée dans l'archive ZIP.

**Returns:**
java.lang.String - commentaire de l'entrée dans l'archive ZIP.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Obtient les paramètres pour la routine de compression ou de décompression.

Peut être l'un de ceux-ci :

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Obtient les paramètres pour le chiffrement ou le déchiffrement. Les paramètres d'une entrée particulière peuvent varier.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Commentaire de l'entrée dans l'archive ZIP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

