---
title: "SevenZipEntrySettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración utilizada para comprimir o descomprimir entradas 7z."
type: docs
weight: 113
url: /es/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Configuración utilizada para comprimir o descomprimir entradas 7z.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Inicializa una nueva instancia de la clase [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Inicializa una nueva instancia de la clase [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Inicializa una nueva instancia de la clase [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Obtiene el valor que indica si comprimir el encabezado del archivo. |
| [getCompressionSettings()](#getCompressionSettings--) | Obtiene la configuración para la rutina de compresión o descompresión. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Obtiene la configuración para el cifrado o descifrado. |
| [getSolid()](#getSolid--) | Obtiene el valor que indica si concatenar entradas y tratarlas como un único bloque de datos. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Establece el valor que indica si comprimir el encabezado del archivo. |
| [setSolid(boolean value)](#setSolid-boolean-) | Establece el valor que indica si concatenar entradas y tratarlas como un único bloque de datos. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Inicializa una nueva instancia de la clase [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Inicializa una nueva instancia de la clase [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Configuración para compresión. Pase null para la configuración predeterminada de LZMA. |

Puede ser uno de estos:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Inicializa una nueva instancia de la clase [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | Configuración para compresión. Pase null para la configuración predeterminada de LZMA. |

Puede ser uno de estos:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | Configuración para cifrado. Pase null si no es necesario cifrar o descifrar. |

Solo puede haber uno:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Obtiene el valor que indica si comprimir el encabezado del archivo.

Esta configuración es equivalente al interruptor `-mhc=on` de la herramienta 7-Zip. Actualmente, es incompatible con el cifrado del encabezado.

**Returns:**
boolean - valor que indica si comprimir el encabezado del archivo
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Obtiene la configuración para la rutina de compresión o descompresión.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Obtiene la configuración para el cifrado o descifrado. La configuración de una entrada particular puede variar.

El [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) es la única opción para archivos 7z.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Obtiene el valor que indica si concatenar entradas y tratarlas como un único bloque de datos.

El siguiente ejemplo muestra cómo comprimir un directorio a un archivo 7z sólido con compresión LZMA2 sin cifrado.

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

Proporcione `SevenZipEntrySettings` para un archivo 7z sólido al instanciar el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | valor que indica si concatenar entradas y tratarlas como un único bloque de datos. |

