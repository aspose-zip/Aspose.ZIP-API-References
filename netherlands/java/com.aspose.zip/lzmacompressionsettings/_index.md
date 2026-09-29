---
title: "LzmaCompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor de LZMA-compressiemethode."
type: docs
weight: 88
url: /nl/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Instellingen voor de LZMA-compressiemethode.

Het Lempel\u2013Ziv\u2013Markov chain-algoritme (LZMA) is een algoritme dat wordt gebruikt om verliesloze gegevenscompressie uit te voeren. Dit algoritme gebruikt een woordenboekcompressieschema dat enigszins vergelijkbaar is met het LZ77-algoritme en biedt een hoge compressieverhouding en een variabele compressiewoordenboekgrootte.

Zie meer: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Initialiseert een nieuw exemplaar van de [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) klasse met standaardparameters. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | Initialiseert een nieuw exemplaar van de [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) klasse met opgegeven dictionary-grootte, aantal snelle bytes en aantal letterlijke contextbits. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | Initialiseert een nieuw exemplaar van de [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) klasse met opgegeven dictionary-grootte, standaard aantal snelle bytes gelijk aan 32 en aantal letterlijke contextbits gelijk aan 3. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | De grootte van het woordenboek (geschiedenisbuffer) geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Haalt het aantal letterlijke contextbits op. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Haalt het aantal bytes op dat wordt gebruikt voor snelle overeenkomstzoekopdrachten in het LZMA-algoritme. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Initialiseert een nieuw exemplaar van de [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) klasse met standaardparameters.

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
