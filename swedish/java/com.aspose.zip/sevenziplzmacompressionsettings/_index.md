---
title: "SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för LZMA-komprimeringsmetod i ett 7z-arkiv."
type: docs
weight: 115
url: /sv/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

Inställningar för LZMA-komprimeringsmetod i ett 7z-arkiv.

Lempel–Ziv–Markov-kedjealgoritmen (LZMA) är en algoritm som används för att utföra förlustfri datakomprimering. Denna algoritm använder ett ordboksbaserat komprimeringsschema som är något likt LZ77-algoritmen och har en hög komprimeringsgrad samt en variabel komprimeringsordboksstorlek.

Se mer: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | Initierar en ny instans av klassen [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) med standardparametrar. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | Initierar en ny instans av klassen [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) med angiven ordboksstorlek, antal snabba byte och antal bokstavliga kontextbitar. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | Initierar en ny instans av klassen [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) med angiven ordboksstorlek, antal snabba byte lika med 32 och antal bokstavliga kontextbitar lika med 3. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Storleken på ordboken (historikbufferten) anger hur många byte av den nyligen bearbetade okomprimerade datan som hålls i minnet. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Hämtar antalet literal kontextbitar. |
| [getMethod()](#getMethod--) | Hämtar komprimerings- eller dekomprimeringsmetod. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Hämtar antalet byte som används för snabb matchningssökning i LZMA-algoritmen. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Storleken på ordboken (historikbufferten) anger hur många byte av den nyligen bearbetade okomprimerade datan som hålls i minnet. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


Initierar en ny instans av klassen [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) med standardparametrar.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings))) {
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

