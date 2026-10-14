---
title: "LzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die LZMA-Komprimierungsmethode."
type: docs
weight: 88
url: /de/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Einstellungen für die LZMA-Komprimierungsmethode.

Der Lempel\u2013Ziv\u2013Markov‑Ketten‑Algorithmus (LZMA) ist ein Algorithmus, der zur verlustfreien Datenkompression verwendet wird. Dieser Algorithmus verwendet ein Wörterbuchkompressionsverfahren, das dem LZ77-Algorithmus etwas ähnlich ist, und bietet ein hohes Kompressionsverhältnis sowie eine variable Größe des Kompressionswörterbuchs.

Siehe mehr: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Initialisiert eine neue Instanz der [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings)-Klasse mit Standardparametern. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | Initialisiert eine neue Instanz der [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings)-Klasse mit angegebener Wörterbuchgröße, Anzahl schneller Bytes und Anzahl der Literal-Kontextbits. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | Initialisiert eine neue Instanz der [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings)-Klasse mit angegebener Wörterbuchgröße, standardmäßiger Anzahl schneller Bytes von 32 und Anzahl der Literal-Kontextbits von 3. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Die Größe des Wörterbuchs (History‑Puffer) gibt an, wie viele Bytes der zuletzt verarbeiteten unkomprimierten Daten im Speicher gehalten werden. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Liefert die Anzahl der Literal‑Kontext‑Bits. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Liefert die Anzahl der Bytes, die für die schnelle Mustersuche im LZMA‑Algorithmus verwendet werden. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Initialisiert eine neue Instanz der [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings)-Klasse mit Standardparametern.

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
