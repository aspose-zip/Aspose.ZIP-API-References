---
title: "SevenZipLZMACompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la méthode de compression LZMA dans une archive 7z."
type: docs
weight: 115
url: /fr/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

Paramètres pour la méthode de compression LZMA dans une archive 7z.

L'algorithme Lempel\\u2013Ziv\\u2013Markov chain (LZMA) est un algorithme utilisé pour effectuer une compression de données sans perte. Cet algorithme utilise un schéma de compression par dictionnaire quelque peu similaire à l'algorithme LZ77 et offre un taux de compression élevé ainsi qu'une taille de dictionnaire de compression variable.

Voir plus: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | Initialise une nouvelle instance de la classe [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) avec les paramètres par défaut. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | Initialise une nouvelle instance de la classe [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) avec la taille du dictionnaire spécifiée, le nombre d’octets rapides et le nombre de bits de contexte littéral. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | Initialise une nouvelle instance de la classe [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) avec la taille du dictionnaire spécifiée, le nombre d’octets rapides égal à 32, le nombre de bits de contexte littéral égal à 3. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | La taille du dictionnaire (tampon d’historique) indique combien d’octets des données non compressées récemment traitées sont conservés en mémoire. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Obtient le nombre de bits de contexte littéral. |
| [getMethod()](#getMethod--) | Obtient la méthode de compression ou de décompression. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Obtient le nombre d'octets utilisés pour la recherche de correspondances rapides dans l'algorithme LZMA. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | La taille du dictionnaire (tampon d’historique) indique combien d’octets des données non compressées récemment traitées sont conservés en mémoire. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


Initialise une nouvelle instance de la classe [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) avec les paramètres par défaut.

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

