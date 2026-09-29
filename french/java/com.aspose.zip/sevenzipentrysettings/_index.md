---
title: "SevenZipEntrySettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres utilisés pour compresser ou décompresser des entrées 7z."
type: docs
weight: 113
url: /fr/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Paramètres utilisés pour compresser ou décompresser des entrées 7z.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Initialise une nouvelle instance de la classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Initialise une nouvelle instance de la classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Initialise une nouvelle instance de la classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Obtient la valeur indiquant si l'en-tête de l'archive doit être compressé. |
| [getCompressionSettings()](#getCompressionSettings--) | Obtient les paramètres pour la routine de compression ou de décompression. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Obtient les paramètres pour le chiffrement ou le déchiffrement. |
| [getSolid()](#getSolid--) | Obtient la valeur indiquant si les entrées doivent être concaténées et traitées comme un seul bloc de données. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Définit la valeur indiquant si l'en-tête de l'archive doit être compressé. |
| [setSolid(boolean value)](#setSolid-boolean-) | Définit la valeur indiquant si les entrées doivent être concaténées et traitées comme un seul bloc de données. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Initialise une nouvelle instance de la classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Initialise une nouvelle instance de la classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | paramètres pour la compression. Passez null pour les paramètres LZMA par défaut. |

Peut être l'un de ceux-ci :

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Initialise une nouvelle instance de la classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | paramètres pour la compression. Passez null pour les paramètres LZMA par défaut. |

Peut être l'un de ceux-ci :

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | paramètres pour le chiffrement. Passez null s'il n'est pas nécessaire de chiffrer ou de déchiffrer. |

Ne peut être qu'un seul :

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Obtient la valeur indiquant si l'en-tête de l'archive doit être compressé.

Ce paramètre est équivalent à l'option `-mhc=on` de l'outil 7-Zip. Actuellement, il est incompatible avec le chiffrement de l'en-tête.

**Returns:**
booléen - valeur indiquant si l'en-tête de l'archive doit être compressé
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Obtient les paramètres pour la routine de compression ou de décompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Obtient les paramètres pour le chiffrement ou le déchiffrement. Les paramètres d'une entrée particulière peuvent varier.

Le [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) est la seule option pour les archives 7z.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Obtient la valeur indiquant si les entrées doivent être concaténées et traitées comme un seul bloc de données.

L'exemple suivant montre comment compresser un répertoire en archive 7z solide avec compression LZMA2 sans chiffrement.

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

Fournissez `SevenZipEntrySettings` pour une archive 7z solide lors de l'instanciation de l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | valeur indiquant si les entrées doivent être concaténées et traitées comme un seul bloc de données. |

