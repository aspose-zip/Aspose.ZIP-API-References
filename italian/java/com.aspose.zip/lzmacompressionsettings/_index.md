---
title: "LzmaCompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per il metodo di compressione LZMA."
type: docs
weight: 88
url: /it/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Impostazioni per il metodo di compressione LZMA.

L'algoritmo Lempel–Ziv–Markov chain (LZMA) è un algoritmo utilizzato per eseguire la compressione dati senza perdita. Questo algoritmo utilizza uno schema di compressione a dizionario leggermente simile all'algoritmo LZ77 e presenta un alto rapporto di compressione e una dimensione del dizionario di compressione variabile.

Vedi di più: [Lempel–Ziv–Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Inizializza una nuova istanza della classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con parametri predefiniti. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | Inizializza una nuova istanza della classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con dimensione del dizionario specificata, numero di byte veloci e numero di bit di contesto letterale. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | Inizializza una nuova istanza della classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con dimensione del dizionario specificata, numero predefinito di byte veloci pari a 32 e numero di bit di contesto letterale pari a 3. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | La dimensione del dizionario (buffer di cronologia) indica quanti byte dei dati non compressi elaborati di recente sono conservati in memoria. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Restituisce il numero di bit di contesto letterale. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Restituisce il numero di byte utilizzati per la ricerca rapida di corrispondenze nell'algoritmo LZMA. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Inizializza una nuova istanza della classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) con parametri predefiniti.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
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
