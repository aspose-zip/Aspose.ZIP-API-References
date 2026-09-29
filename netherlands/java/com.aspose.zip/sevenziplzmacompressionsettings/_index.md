---
title: "SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor LZMA-compressiemethode binnen een 7z-archief."
type: docs
weight: 115
url: /nl/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

Instellingen voor LZMA-compressiemethode binnen een 7z-archief.

Het Lempel\u2013Ziv\u2013Markov chain-algoritme (LZMA) is een algoritme dat wordt gebruikt om verliesloze gegevenscompressie uit te voeren. Dit algoritme gebruikt een woordenboekcompressieschema dat enigszins vergelijkbaar is met het LZ77-algoritme en biedt een hoge compressieverhouding en een variabele compressiewoordenboekgrootte.

Zie meer: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | Initialiseert een nieuw exemplaar van de [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) klasse met standaardparameters. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | Initialiseert een nieuw exemplaar van de [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) klasse met opgegeven dictionary-grootte, aantal snelle bytes en aantal literal context bits. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | Initialiseert een nieuw exemplaar van de [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) klasse met opgegeven dictionary-grootte, aantal snelle bytes gelijk aan 32, aantal literal context bits gelijk aan 3. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Dictionary (geschiedenisbuffer) grootte geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Haalt het aantal letterlijke contextbits op. |
| [getMethod()](#getMethod--) | Haalt compressie- of decompressiemethode op. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Haalt het aantal bytes op dat wordt gebruikt voor snelle overeenkomstzoekopdrachten in het LZMA-algoritme. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Dictionary (geschiedenisbuffer) grootte geeft aan hoeveel bytes van de recent verwerkte ongecomprimeerde gegevens in het geheugen worden bewaard. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


Initialiseert een nieuw exemplaar van de [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) klasse met standaardparameters.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
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

