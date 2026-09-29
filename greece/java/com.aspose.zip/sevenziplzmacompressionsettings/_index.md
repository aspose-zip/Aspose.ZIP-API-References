---
title: "SevenZipLZMACompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη μέθοδο συμπίεσης LZMA μέσα σε αρχείο 7z."
type: docs
weight: 115
url: /el/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

Ρυθμίσεις για τη μέθοδο συμπίεσης LZMA μέσα σε αρχείο 7z.

Ο αλγόριθμος αλυσίδας Lempel\\u2013Ziv\\u2013Markov (LZMA) είναι ένας αλγόριθμος που χρησιμοποιείται για την εκτέλεση συμπίεσης δεδομένων χωρίς απώλειες. Αυτός ο αλγόριθμος χρησιμοποιεί ένα σχήμα συμπίεσης λεξικού κάπως παρόμοιο με τον αλγόριθμο LZ77 και διαθέτει υψηλό λόγο συμπίεσης και μεταβλητό μέγεθος λεξικού συμπίεσης.

Δείτε περισσότερα: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) με προεπιλεγμένες παραμέτρους. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων byte και αριθμό bits κυριολεκτικού πλαισίου. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) με καθορισμένο μέγεθος λεξικού, αριθμό γρήγορων byte ίσο με 32, αριθμό bits κυριολεκτικού πλαισίου ίσο με 3. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Επιστρέφει τον αριθμό των bits κυριολεκτικού πλαισίου. |
| [getMethod()](#getMethod--) | Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Επιστρέφει τον αριθμό των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) με προεπιλεγμένες παραμέτρους.

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

