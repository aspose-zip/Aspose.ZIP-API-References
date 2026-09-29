---
title: "ArchiveEntrySettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni utilizzate per comprimere o decomprimere le voci."
type: docs
weight: 30
url: /it/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Impostazioni utilizzate per comprimere o decomprimere le voci.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Inizializza una nuova istanza della classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Inizializza una nuova istanza della classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Inizializza una nuova istanza della classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getComment()](#getComment--) | Ottiene il commento per la voce all'interno dell'archivio ZIP. |
| [getCompressionSettings()](#getCompressionSettings--) | Ottiene le impostazioni per la routine di compressione o decompressione. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Ottiene le impostazioni per la crittografia o la decrittazione. |
| [setComment(String value)](#setComment-java.lang.String-) | Commento per la voce all'interno dell'archivio ZIP. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Inizializza una nuova istanza della classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Inizializza una nuova istanza della classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Impostazioni per la compressione. Passare null per le impostazioni predefinite di deflate. |

Può essere uno di questi:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Inizializza una nuova istanza della classe [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Impostazioni per la compressione. Passare null per le impostazioni predefinite di deflate. |

Può essere uno di questi:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Impostazioni per la crittografia. Passare null se non è necessario crittografare o decrittografare. |

Può essere uno di questi:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Ottiene il commento per la voce all'interno dell'archivio ZIP.

**Returns:**
java.lang.String - commento per la voce all'interno dell'archivio ZIP.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Ottiene le impostazioni per la routine di compressione o decompressione.

Può essere uno di questi:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Ottiene le impostazioni per la crittografia o la decrittazione. Le impostazioni di una voce particolare possono variare.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Commento per la voce all'interno dell'archivio ZIP.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

