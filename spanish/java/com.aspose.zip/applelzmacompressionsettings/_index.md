---
title: "AppleLzmaCompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para la compresión LZMA dentro de un archivo Apple Archive .aar."
type: docs
weight: 23
url: /es/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Configuraciones para la compresión LZMA dentro de un archivo Apple Archive (.aar).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) con parámetros predeterminados. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Obtiene el tamaño de cada bloque de datos antes de la compresión. |
| [getDictionarySize()](#getDictionarySize--) | Obtiene el tamaño del diccionario usado para la compresión. |
| [getFastBytes()](#getFastBytes--) | Obtiene el número de bytes rápidos usados para la compresión. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| blockSize | int | El tamaño de cada bloque de datos antes de la compresión. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| blockSize | int | El tamaño de cada bloque de datos antes de la compresión. |
| dictionarySize | int | El tamaño del diccionario usado para la compresión. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| blockSize | int | El tamaño de cada bloque de datos antes de la compresión. |
| dictionarySize | int | El tamaño del diccionario usado para la compresión. |
| fastBytes | int | El número de bytes rápidos usados para la compresión. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Inicializa una nueva instancia de la clase [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) con parámetros predeterminados.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Obtiene el tamaño de cada bloque de datos antes de la compresión.

Valor: El valor predeterminado es 4 MiB.

**Returns:**
int - el tamaño de cada bloque de datos antes de la compresión.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Obtiene el tamaño del diccionario usado para la compresión.

Valor: El valor predeterminado es 8 MiB.

**Returns:**
int - el tamaño del diccionario usado para la compresión.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Obtiene el número de bytes rápidos usados para la compresión.

Valor: El valor predeterminado es 32.

**Returns:**
int - el número de bytes rápidos usados para la compresión.
