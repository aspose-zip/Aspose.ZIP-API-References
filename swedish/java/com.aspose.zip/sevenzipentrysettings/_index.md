---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar som används för att komprimera eller dekomprimera 7z-poster."
type: docs
weight: 113
url: /sv/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Inställningar som används för att komprimera eller dekomprimera 7z-poster.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Initierar en ny instans av klassen [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Initierar en ny instans av klassen [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Initierar en ny instans av klassen [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Hämtar värde som indikerar om arkivhuvudet ska komprimeras. |
| [getCompressionSettings()](#getCompressionSettings--) | Hämtar inställningar för komprimerings- eller dekomprimeringsrutin. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Hämtar inställningar för kryptering eller dekryptering. |
| [getSolid()](#getSolid--) | Hämtar värde som indikerar om poster ska sammanfogas och behandlas som ett enda datablock. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Ställer in värde som indikerar om arkivhuvudet ska komprimeras. |
| [setSolid(boolean value)](#setSolid-boolean-) | Ställer in värde som indikerar om poster ska sammanfogas och behandlas som ett enda datablock. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Initierar en ny instans av klassen [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Initierar en ny instans av klassen [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | inställningar för komprimering. Skicka null för standard LZMA-inställningar. |

Kan vara en av dessa:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Initierar en ny instans av klassen [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | inställningar för komprimering. Skicka null för standard LZMA-inställningar. |

Kan vara en av dessa:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | inställningar för kryptering. Skicka null om ingen kryptering eller dekryptering behövs. |

Kan bara vara en:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Hämtar värde som indikerar om arkivhuvudet ska komprimeras.

Denna inställning motsvarar `-mhc=on`-växeln i 7-Zip-verktyget. För närvarande är den inkompatibel med huvudkryptering.

**Returns:**
boolesk - värde som indikerar om arkivhuvudet ska komprimeras
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Hämtar inställningar för komprimerings- eller dekomprimeringsrutin.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Hämtar inställningar för kryptering eller dekryptering. Inställningarna för en specifik post kan variera.

Den [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) är det enda alternativet för 7z-arkiv.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Hämtar värde som indikerar om poster ska sammanfogas och behandlas som ett enda datablock.

Följande exempel visar hur man komprimerar en katalog till ett solid 7z-arkiv med LZMA2-komprimering utan kryptering.

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

Tillhandahåll `SevenZipEntrySettings` för solid 7z-arkiv vid arkivinstansiering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | värde som indikerar om poster ska sammanfogas och behandlas som ett enda datablock. |

