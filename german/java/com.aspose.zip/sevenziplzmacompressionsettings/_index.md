---
title: "SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die LZMA-Kompressionsmethode innerhalb eines 7z-Archivs."
type: docs
weight: 115
url: /de/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

Einstellungen für die LZMA-Kompressionsmethode innerhalb eines 7z-Archivs.

Der Lempel\u2013Ziv\u2013Markov‑Ketten‑Algorithmus (LZMA) ist ein Algorithmus, der zur verlustfreien Datenkompression verwendet wird. Dieser Algorithmus verwendet ein Wörterbuchkompressionsverfahren, das dem LZ77-Algorithmus etwas ähnlich ist, und bietet ein hohes Kompressionsverhältnis sowie eine variable Größe des Kompressionswörterbuchs.

Siehe mehr: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | Initialisiert eine neue Instanz der [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) Klasse mit Standardparametern. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | Initialisiert eine neue Instanz der [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) Klasse mit angegebenen Wörterbuchgröße, Anzahl schneller Bytes und Anzahl der Literal-Kontextbits. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | Initialisiert eine neue Instanz der [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) Klasse mit angegebenen Wörterbuchgröße, Anzahl schneller Bytes gleich 32 und Anzahl der Literal-Kontextbits gleich 3. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Die Größe des Wörterbuchs (Verlaufs-Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Liefert die Anzahl der Literal‑Kontext‑Bits. |
| [getMethod()](#getMethod--) | Liefert die Komprimierungs- oder Dekomprimierungsmethode. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Liefert die Anzahl der Bytes, die für die schnelle Mustersuche im LZMA‑Algorithmus verwendet werden. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Die Größe des Wörterbuchs (Verlaufs-Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


Initialisiert eine neue Instanz der [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) Klasse mit Standardparametern.

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

