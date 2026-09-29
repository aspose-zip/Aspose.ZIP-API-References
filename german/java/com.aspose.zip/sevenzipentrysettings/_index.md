---
title: "SevenZipEntrySettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen zum Komprimieren oder Dekomprimieren von 7z-Einträgen."
type: docs
weight: 113
url: /de/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Einstellungen zum Komprimieren oder Dekomprimieren von 7z-Einträgen.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Initialisiert eine neue Instanz der [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings)-Klasse. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Initialisiert eine neue Instanz der [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings)-Klasse. |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Initialisiert eine neue Instanz der [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Liefert den Wert, der angibt, ob der Archivkopf komprimiert werden soll. |
| [getCompressionSettings()](#getCompressionSettings--) | Liefert die Einstellungen für die Komprimierungs- oder Dekomprimierungsroutine. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Liefert die Einstellungen für die Verschlüsselung oder Entschlüsselung. |
| [getSolid()](#getSolid--) | Liefert den Wert, der angibt, ob Einträge zusammengeführt und als ein einziger Datenblock behandelt werden sollen. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Setzt den Wert, der angibt, ob der Archivkopf komprimiert werden soll. |
| [setSolid(boolean value)](#setSolid-boolean-) | Setzt den Wert, der angibt, ob Einträge zusammengeführt und als ein einziger Datenblock behandelt werden sollen. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Initialisiert eine neue Instanz der [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings)-Klasse.

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Initialisiert eine neue Instanz der [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Einstellungen für die Kompression. Übergeben Sie null für die Standard‑LZMA‑Einstellungen. |

Kann einer der folgenden sein:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Initialisiert eine neue Instanz der [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings)-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Einstellungen für die Kompression. Übergeben Sie null für die Standard‑LZMA‑Einstellungen. |

Kann einer der folgenden sein:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | Einstellungen für die Verschlüsselung. Übergeben Sie null, wenn keine Verschlüsselung oder Entschlüsselung erforderlich ist. |

Es kann nur einer sein:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Liefert den Wert, der angibt, ob der Archivkopf komprimiert werden soll.

Diese Einstellung entspricht dem Schalter `-mhc=on` des 7‑Zip‑Tools. Derzeit ist sie mit der Kopfverschlüsselung nicht kompatibel.

**Returns:**
boolesch – Wert, der angibt, ob der Archivkopf komprimiert werden soll
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Liefert die Einstellungen für die Komprimierungs- oder Dekomprimierungsroutine.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Liefert die Einstellungen für die Verschlüsselung oder Entschlüsselung. Die Einstellungen eines bestimmten Eintrags können variieren.

Die [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionssettings) ist die einzige Option für 7z‑Archive.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Liefert den Wert, der angibt, ob Einträge zusammengeführt und als ein einziger Datenblock behandelt werden sollen.

Das folgende Beispiel zeigt, wie ein Verzeichnis zu einem soliden 7z‑Archiv mit LZMA2‑Kompression ohne Verschlüsselung komprimiert wird.

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

Stellen Sie `SevenZipEntrySettings` für ein solides 7z‑Archiv bei der Instanziierung des Archivs bereit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Wert, der angibt, ob Einträge zusammengeführt und als ein einziger Datenblock behandelt werden sollen. |

