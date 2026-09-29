---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen die worden gebruikt om 7z-items te comprimeren of te decomprimeren."
type: docs
weight: 113
url: /nl/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Instellingen die worden gebruikt om 7z-items te comprimeren of te decomprimeren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Initialiseert een nieuw exemplaar van de klasse [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Initialiseert een nieuw exemplaar van de klasse [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Initialiseert een nieuw exemplaar van de klasse [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Haalt de waarde op die aangeeft of de archiefkop moet worden gecomprimeerd. |
| [getCompressionSettings()](#getCompressionSettings--) | Haalt de instellingen op voor compressie- of decompressieroutine. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Haalt de instellingen op voor versleuteling of ontsleuteling. |
| [getSolid()](#getSolid--) | Haalt de waarde op die aangeeft of items moeten worden samengevoegd en als één gegevensblok moeten worden behandeld. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Stelt de waarde in die aangeeft of de archiefkop moet worden gecomprimeerd. |
| [setSolid(boolean value)](#setSolid-boolean-) | Stelt de waarde in die aangeeft of items moeten worden samengevoegd en als één gegevensblok moeten worden behandeld. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Initialiseert een nieuw exemplaar van de klasse [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Initialiseert een nieuw exemplaar van de klasse [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Instellingen voor compressie. Geef null door voor de standaard LZMA-instellingen. |

Kan een van deze zijn:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Initialiseert een nieuw exemplaar van de klasse [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Instellingen voor compressie. Geef null door voor de standaard LZMA-instellingen. |

Kan een van deze zijn:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | Instellingen voor versleuteling. Geef null door als er geen versleuteling of ontsleuteling nodig is. |

Kan slechts één zijn:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Haalt de waarde op die aangeeft of de archiefkop moet worden gecomprimeerd.

Deze instelling is equivalent aan de `-mhc=on`-schakelaar van het 7-Zip-hulpmiddel. Momenteel is deze niet compatibel met kopversleuteling.

**Returns:**
boolean - waarde die aangeeft of de archiefkop moet worden gecomprimeerd
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Haalt de instellingen op voor compressie- of decompressieroutine.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Haalt de instellingen op voor versleuteling of ontsleuteling. De instellingen van een specifiek item kunnen variëren.

De [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) is de enige optie voor 7z-archieven.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Haalt de waarde op die aangeeft of items moeten worden samengevoegd en als één gegevensblok moeten worden behandeld.

Het volgende voorbeeld toont hoe een map te comprimeren naar een solide 7z-archief met LZMA2-compressie zonder versleuteling.

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

Voorzie `SevenZipEntrySettings` voor een solide 7z-archief bij het instantieren van het archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | waarde die aangeeft of items moeten worden samengevoegd en als één gegevensblok moeten worden behandeld. |

