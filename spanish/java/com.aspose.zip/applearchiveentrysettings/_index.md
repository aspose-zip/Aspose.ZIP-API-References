---
title: "AppleArchiveEntrySettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración utilizada para componer entradas dentro de ."
type: docs
weight: 18
url: /es/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Configuración utilizada para componer entradas dentro de [AppleArchive](../../com.aspose.zip/applearchive).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Inicializa una nueva instancia de la clase [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Obtiene la configuración de compresión aplicada a la carga útil del Apple Archive compuesto. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Obtiene un valor que indica si los campos de suma de verificación CRC32 están incluidos para las entradas de archivo compuestas. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Establece un valor que indica si los campos de suma de verificación CRC32 están incluidos para las entradas de archivo compuestas. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Inicializa una nueva instancia de la clase [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Configuración de compresión aplicada a la carga útil del Apple Archive compuesto. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Obtiene la configuración de compresión aplicada a la carga útil del Apple Archive compuesto.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Obtiene un valor que indica si los campos de suma de verificación CRC32 están incluidos para las entradas de archivo compuestas.

**Returns:**
boolean - un valor que indica si los campos de suma de verificación CRC32 están incluidos para las entradas de archivo compuestas.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Establece un valor que indica si los campos de suma de verificación CRC32 están incluidos para las entradas de archivo compuestas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si los campos de suma de verificación CRC32 están incluidos para las entradas de archivo compuestas. |

