---
title: "LzmaCompressionSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuraciones para el método de compresión LZMA."
type: docs
weight: 88
url: /es/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Configuraciones para el método de compresión LZMA.

El algoritmo Lempel\\u2013Ziv\\u2013Markov chain (LZMA) es un algoritmo utilizado para realizar compresión de datos sin pérdida. Este algoritmo usa un esquema de compresión por diccionario algo similar al algoritmo LZ77 y presenta una alta relación de compresión y un tamaño de diccionario de compresión variable.

Ver más: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Inicializa una nueva instancia de la clase [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con parámetros predeterminados. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | Inicializa una nueva instancia de la clase [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con el tamaño de diccionario especificado, el número de bytes rápidos y el número de bits de contexto literal. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | Inicializa una nueva instancia de la clase [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con el tamaño de diccionario especificado, número predeterminado de bytes rápidos igual a 32 y número de bits de contexto literal igual a 3. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Obtiene el número de bits de contexto literal. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Obtiene el número de bytes utilizados para la búsqueda rápida de coincidencias en el algoritmo LZMA. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Inicializa una nueva instancia de la clase [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con parámetros predeterminados.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



### LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#LzmaCompressionSettings-int-int-int-}
```
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### LzmaCompressionSettings(int dictionarySize) {#LzmaCompressionSettings-int-}
```
public LzmaCompressionSettings(int dictionarySize)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - how many bytes of the recently processed uncompressed data are kept in memory.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
