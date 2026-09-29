---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para el método de compresión LZMA2 dentro de un archivo 7z."
type: docs
weight: 114
url: /es/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Configuración para el método de compresión LZMA2 dentro de un archivo 7z.

LZMA2 admite múltiples ejecuciones de datos LZMA comprimidos y datos sin comprimir.

See more: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Obtiene el recuento de hilos de compresión. |
| [getDictionarySize()](#getDictionarySize--) | El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria. |
| [getFastBytes()](#getFastBytes--) | Obtiene el número de control de bytes rápidos usado por el compresor LZMA2. |
| [getMethod()](#getMethod--) | Obtiene el método de compresión o descompresión. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Establece el recuento de hilos de compresión. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | dictionarySize | int | el tamaño del búfer de historial, debe estar entre 4096 y 1073741824. |

Cuanto mayor sea el diccionario, generalmente mejor será la relación de compresión, pero los diccionarios más grandes que los datos sin comprimir son un desperdicio de RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Instancia la configuración para el método de compresión LZMA2 dentro del archivo 7z.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | dictionarySize | int | el tamaño del búfer de historial, debe estar entre 4096 y 1073741824. |

Cuanto mayor sea el diccionario, generalmente mejor será la relación de compresión, pero los diccionarios más grandes que los datos sin comprimir son un desperdicio de RAM. |
| fastBytes | int | controla el número de bytes rápidos usados por los compresores LZMA2. Un número mayor de bytes rápidos puede proporcionar una mejor relación de compresión a expensas de la velocidad de compresión. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Obtiene el recuento de hilos de compresión. Si el valor es mayor que 1, se utilizará compresión multihilo.

**Returns:**
int - recuento de hilos de compresión
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria.

**Returns:**
int - tamaño del diccionario (búfer de historial)
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Obtiene el número de control de bytes rápidos usado por el compresor LZMA2.

**Returns:**
int - el número de control de bytes rápidos usado por el compresor LZMA2
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Obtiene el método de compresión o descompresión.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Establece el recuento de hilos de compresión. Si el valor es mayor que 1, se utilizará compresión multihilo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | recuento de hilos de compresión. |

No establezca este número mayor que los núcleos de CPU. |

