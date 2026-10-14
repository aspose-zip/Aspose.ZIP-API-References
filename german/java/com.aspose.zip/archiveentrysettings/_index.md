---
title: "ArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen, die zum Komprimieren oder Dekomprimieren von Einträgen verwendet werden."
type: docs
weight: 30
url: /de/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Einstellungen, die zum Komprimieren oder Dekomprimieren von Einträgen verwendet werden.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Initialisiert eine neue Instanz der Klasse [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Initialisiert eine neue Instanz der Klasse [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Initialisiert eine neue Instanz der Klasse [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getComment()](#getComment--) | Liest den Kommentar für den Eintrag im ZIP-Archiv. |
| [getCompressionSettings()](#getCompressionSettings--) | Liefert die Einstellungen für die Komprimierungs- oder Dekomprimierungsroutine. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Liefert die Einstellungen für die Verschlüsselung oder Entschlüsselung. |
| [setComment(String value)](#setComment-java.lang.String-) | Kommentar für den Eintrag im ZIP-Archiv. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Initialisiert eine neue Instanz der Klasse [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Initialisiert eine neue Instanz der Klasse [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Einstellungen für die Kompression. Übergeben Sie null für die standardmäßigen Deflate-Einstellungen. |

Kann einer der folgenden sein:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Initialisiert eine neue Instanz der Klasse [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Einstellungen für die Kompression. Übergeben Sie null für die standardmäßigen Deflate-Einstellungen. |

Kann einer der folgenden sein:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Einstellungen für die Verschlüsselung. Übergeben Sie null, wenn keine Verschlüsselung oder Entschlüsselung erforderlich ist. |

Kann einer der folgenden sein:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Liest den Kommentar für den Eintrag im ZIP-Archiv.

**Returns:**
java.lang.String - Kommentar für den Eintrag im ZIP-Archiv.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Liefert die Einstellungen für die Komprimierungs- oder Dekomprimierungsroutine.

Kann einer der folgenden sein:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Liefert die Einstellungen für die Verschlüsselung oder Entschlüsselung. Die Einstellungen eines bestimmten Eintrags können variieren.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Kommentar für den Eintrag im ZIP-Archiv.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

