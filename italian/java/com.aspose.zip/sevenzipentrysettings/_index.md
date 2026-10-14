---
title: "SevenZipEntrySettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni utilizzate per comprimere o decomprimere le voci 7z."
type: docs
weight: 113
url: /it/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Impostazioni utilizzate per comprimere o decomprimere le voci 7z.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Inizializza una nuova istanza della classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Inizializza una nuova istanza della classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Inizializza una nuova istanza della classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Ottiene il valore che indica se comprimere l'intestazione dell'archivio. |
| [getCompressionSettings()](#getCompressionSettings--) | Ottiene le impostazioni per la routine di compressione o decompressione. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Ottiene le impostazioni per la crittografia o la decrittazione. |
| [getSolid()](#getSolid--) | Ottiene il valore che indica se concatenare le voci e trattarle come un unico blocco di dati. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Imposta il valore che indica se comprimere l'intestazione dell'archivio. |
| [setSolid(boolean value)](#setSolid-boolean-) | Imposta il valore che indica se concatenare le voci e trattarle come un unico blocco di dati. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Inizializza una nuova istanza della classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Inizializza una nuova istanza della classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | impostazioni per la compressione. Passare null per le impostazioni predefinite LZMA. |

Può essere uno di questi:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Inizializza una nuova istanza della classe [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | impostazioni per la compressione. Passare null per le impostazioni predefinite LZMA. |

Può essere uno di questi:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | impostazioni per la crittografia. Passare null se non è necessario crittografare o decrittare. |

Può esserci solo una:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Ottiene il valore che indica se comprimere l'intestazione dell'archivio.

Questa impostazione è equivalente all'opzione `-mhc=on` dello strumento 7-Zip. Attualmente, è incompatibile con la crittografia dell'intestazione.

**Returns:**
boolean - valore che indica se comprimere l'intestazione dell'archivio
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Ottiene le impostazioni per la routine di compressione o decompressione.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Ottiene le impostazioni per la crittografia o la decrittazione. Le impostazioni di una voce particolare possono variare.

Il [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) è l'unica opzione per gli archivi 7z.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Ottiene il valore che indica se concatenare le voci e trattarle come un unico blocco di dati.

Il seguente esempio mostra come comprimere una directory in un archivio 7z solido con compressione LZMA2 senza crittografia.

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

Fornire `SevenZipEntrySettings` per un archivio 7z solido durante l'istanziazione dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | valore che indica se concatenare le voci e trattarle come un unico blocco di dati. |

