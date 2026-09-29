---
title: "LzmaCompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη μέθοδο συμπίεσης LZMA."
type: docs
weight: 88
url: /el/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

Ρυθμίσεις για τη μέθοδο συμπίεσης LZMA.

Ο αλγόριθμος αλυσίδας Lempel\\u2013Ziv\\u2013Markov (LZMA) είναι ένας αλγόριθμος που χρησιμοποιείται για την εκτέλεση συμπίεσης δεδομένων χωρίς απώλειες. Αυτός ο αλγόριθμος χρησιμοποιεί ένα σχήμα συμπίεσης λεξικού κάπως παρόμοιο με τον αλγόριθμο LZ77 και διαθέτει υψηλό λόγο συμπίεσης και μεταβλητό μέγεθος λεξικού συμπίεσης.

Δείτε περισσότερα: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) με προεπιλεγμένες παραμέτρους. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων byte και αριθμό bits κυριολεκτικού πλαισίου. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) με καθορισμένο μέγεθος λεξικού, προεπιλεγμένο αριθμό γρήγορων byte ίσο με 32 και αριθμό bits κυριολεκτικού πλαισίου ίσο με 3. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Επιστρέφει τον αριθμό των bits κυριολεκτικού πλαισίου. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Επιστρέφει τον αριθμό των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) με προεπιλεγμένες παραμέτρους.

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
