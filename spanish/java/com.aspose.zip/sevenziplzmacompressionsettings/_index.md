---
title: "SevenZipLZMACompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuración para el método de compresión LZMA dentro de un archivo 7z."
type: docs
weight: 115
url: /es/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

Configuración para el método de compresión LZMA dentro de un archivo 7z.

El algoritmo Lempel\\u2013Ziv\\u2013Markov chain (LZMA) es un algoritmo utilizado para realizar compresión de datos sin pérdida. Este algoritmo usa un esquema de compresión por diccionario algo similar al algoritmo LZ77 y presenta una alta relación de compresión y un tamaño de diccionario de compresión variable.

Ver más: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | Inicializa una nueva instancia de la clase [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) con parámetros predeterminados. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | Inicializa una nueva instancia de la clase [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) con el tamaño de diccionario especificado, el número de bytes rápidos y el número de bits de contexto literal. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | Inicializa una nueva instancia de la clase [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) con el tamaño de diccionario especificado, el número de bytes rápidos igual a 32 y el número de bits de contexto literal igual a 3. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Obtiene el número de bits de contexto literal. |
| [getMethod()](#getMethod--) | Obtiene el método de compresión o descompresión. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Obtiene el número de bytes utilizados para la búsqueda rápida de coincidencias en el algoritmo LZMA. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


Inicializa una nueva instancia de la clase [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) con parámetros predeterminados.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("result.7z");
}
 
```



### SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#SevenZipLZMACompressionSettings-int-int-int-}
```
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### SevenZipLZMACompressionSettings(int dictionarySize) {#SevenZipLZMACompressionSettings-int-}
```
public SevenZipLZMACompressionSettings(int dictionarySize)
```


Initializes a new instance of the [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) class with specified dictionary size, number of fast bytes equal to 32, number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - dictionary (history buffer) size
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Gets compression or decompression method.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | dictionary (history buffer) size |

