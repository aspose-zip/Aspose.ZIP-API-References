---
title: "LzmaArchiveSettings"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Configuraciones para el archivo lzma."
type: docs
weight: 87
url: /es/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Configuraciones para el archivo lzma.

El algoritmo Lempel\\u2013Ziv\\u2013Markov chain (LZMA) es un algoritmo utilizado para realizar compresión de datos sin pérdida. Este algoritmo usa un esquema de compresión por diccionario algo similar al algoritmo LZ77 y presenta una alta relación de compresión y un tamaño de diccionario de compresión variable.

Ver más: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Inicializa una nueva instancia de la clase [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) con un tamaño de diccionario predeterminado, igual a 16 megabytes, número de bytes rápidos igual a 32 y bits de contexto literal igual a 3. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtiene un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [getDictionarySize()](#getDictionarySize--) | El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Obtiene el número de bits de contexto literal. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Obtiene el número de bytes utilizados para la búsqueda rápida de coincidencias en el algoritmo LZMA. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Establece un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Establece el número de bits de contexto literal. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Establece el número de bytes utilizados para la búsqueda rápida de coincidencias en el algoritmo LZMA. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Inicializa una nueva instancia de la clase [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) con un tamaño de diccionario predeterminado, igual a 16 megabytes, número de bytes rápidos igual a 32 y bits de contexto literal igual a 3.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


El tamaño del diccionario (búfer de historial) indica cuántos bytes de los datos descomprimidos procesados recientemente se mantienen en memoria. Si no se establece, se elegirá de acuerdo al tamaño de la entrada.

Cuanto mayor sea el diccionario, generalmente mejor será la relación de compresión, pero los diccionarios más grandes que los datos descomprimidos son un desperdicio de RAM. El tamaño del diccionario del archivo LZMA debe ser una potencia de dos (2^n) o tres veces una potencia de dos (3\\*2^n).

**Returns:**
int - Tamaño del diccionario (búfer de historial).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Obtiene el número de bits de contexto literal.

Los bits de contexto literal definen cuántos de los bits más significativos del byte descomprimido anterior se utilizan para predecir los bits del siguiente byte literal. Deben estar entre 0 y 8.

**Returns:**
int - el número de bits de contexto literal.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Obtiene el número de bytes utilizados para la búsqueda rápida de coincidencias en el algoritmo LZMA.

Un valor más alto permite al compresor buscar coincidencias más largas, lo que puede mejorar ligeramente la relación de compresión pero ralentiza la compresión.

**Returns:**
int - el número de bytes utilizados para la búsqueda de coincidencias rápidas en el algoritmo LZMA.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Establece un evento que se dispara cuando se comprime una parte del flujo sin procesar.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

