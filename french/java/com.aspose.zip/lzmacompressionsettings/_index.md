---
title: "LzmaCompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres de la méthode de compression LZMA."
type: docs
weight: 88
url: /fr/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Paramètres de la méthode de compression LZMA.

L'algorithme Lempel\\u2013Ziv\\u2013Markov chain (LZMA) est un algorithme utilisé pour effectuer une compression de données sans perte. Cet algorithme utilise un schéma de compression par dictionnaire quelque peu similaire à l'algorithme LZ77 et offre un taux de compression élevé ainsi qu'une taille de dictionnaire de compression variable.

Voir plus: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Initialise une nouvelle instance de la classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) avec des paramètres par défaut. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | Initialise une nouvelle instance de la classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) avec la taille du dictionnaire spécifiée, le nombre d’octets rapides et le nombre de bits de contexte littéral. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | Initialise une nouvelle instance de la classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) avec la taille du dictionnaire spécifiée, le nombre d’octets rapides par défaut égal à 32 et le nombre de bits de contexte littéral égal à 3. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | La taille du dictionnaire (tampon d'historique) indique combien d'octets des données non compressées récemment traitées sont conservés en mémoire. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Obtient le nombre de bits de contexte littéral. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Obtient le nombre d'octets utilisés pour la recherche de correspondances rapides dans l'algorithme LZMA. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Initialise une nouvelle instance de la classe [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) avec des paramètres par défaut.

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
