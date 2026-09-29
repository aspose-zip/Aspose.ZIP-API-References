---
title: "AppleLz4CompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para la compresión LZ4 dentro de un archivo Apple Archive .aar."
type: docs
weight: 21
url: /es/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Configuraciones para la compresión LZ4 dentro de un archivo Apple Archive (.aar).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Inicializa una nueva instancia de la clase [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Inicializa una nueva instancia de la clase [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) con parámetros predeterminados. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Obtiene el tamaño de cada bloque comprimido `pbz4`/`bv41`. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Inicializa una nueva instancia de la clase [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| blockSize | int | El tamaño de cada bloque comprimido `pbz4`/`bv41`. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Inicializa una nueva instancia de la clase [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) con parámetros predeterminados.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Obtiene el tamaño de cada bloque comprimido `pbz4`/`bv41`.

Valor: El valor predeterminado es 4 MiB.

**Returns:**
int - el tamaño de cada bloque comprimido `pbz4`/`bv41`.
