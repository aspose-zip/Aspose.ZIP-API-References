---
title: "ArchiveEntrySettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuraciones usadas para comprimir o descomprimir entradas."
type: docs
weight: 30
url: /es/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Configuraciones usadas para comprimir o descomprimir entradas.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Inicializa una nueva instancia de la clase [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Inicializa una nueva instancia de la clase [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Inicializa una nueva instancia de la clase [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getComment()](#getComment--) | Obtiene el comentario de la entrada dentro del archivo ZIP. |
| [getCompressionSettings()](#getCompressionSettings--) | Obtiene la configuración para la rutina de compresión o descompresión. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Obtiene la configuración para el cifrado o descifrado. |
| [setComment(String value)](#setComment-java.lang.String-) | Comentario de la entrada dentro del archivo ZIP. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Inicializa una nueva instancia de la clase [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Inicializa una nueva instancia de la clase [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Configuración para compresión. Pase null para la configuración predeterminada de deflate. |

Puede ser uno de estos:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Inicializa una nueva instancia de la clase [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Configuración para compresión. Pase null para la configuración predeterminada de deflate. |

Puede ser uno de estos:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Configuración para cifrado. Pase null si no es necesario cifrar o descifrar. |

Puede ser uno de estos:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Obtiene el comentario de la entrada dentro del archivo ZIP.

**Returns:**
java.lang.String - comentario de la entrada dentro del archivo ZIP.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Obtiene la configuración para la rutina de compresión o descompresión.

Puede ser uno de estos:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Obtiene la configuración para el cifrado o descifrado. La configuración de una entrada particular puede variar.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Comentario de la entrada dentro del archivo ZIP.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

