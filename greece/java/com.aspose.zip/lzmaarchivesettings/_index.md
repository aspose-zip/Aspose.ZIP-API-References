---
title: "LzmaArchiveSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για το αρχείο lzma."
type: docs
weight: 87
url: /el/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

Ρυθμίσεις για το αρχείο lzma.

Ο αλγόριθμος αλυσίδας Lempel\\u2013Ziv\\u2013Markov (LZMA) είναι ένας αλγόριθμος που χρησιμοποιείται για την εκτέλεση συμπίεσης δεδομένων χωρίς απώλειες. Αυτός ο αλγόριθμος χρησιμοποιεί ένα σχήμα συμπίεσης λεξικού κάπως παρόμοιο με τον αλγόριθμο LZ77 και διαθέτει υψηλό λόγο συμπίεσης και μεταβλητό μέγεθος λεξικού συμπίεσης.

Δείτε περισσότερα: [Lempel\\u2013Ziv\\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) με προεπιλεγμένο μέγεθος λεξικού, ίσο με 16 megabytes, αριθμό γρήγορων byte ίσο με 32 και bits κυριολεκτικού πλαισίου ίσα με 3. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [getDictionarySize()](#getDictionarySize--) | Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. |
| [getLiteralContextBits()](#getLiteralContextBits--) | Επιστρέφει τον αριθμό των bits κυριολεκτικού πλαισίου. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | Επιστρέφει τον αριθμό των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | Ορίζει τον αριθμό των bits κυριολεκτικού πλαισίου. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | Ορίζει τον αριθμό των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) με προεπιλεγμένο μέγεθος λεξικού, ίσο με 16 megabytes, αριθμό γρήγορων byte ίσο με 32 και bits κυριολεκτικού πλαισίου ίσα με 3.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource("data.bin");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. Εάν δεν οριστεί, θα επιλεγεί ανάλογα με το μέγεθος της καταχώρησης.

Όσο μεγαλύτερο είναι το λεξικό, συνήθως τόσο καλύτερος είναι ο λόγος συμπίεσης - αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM. Το μέγεθος του λεξικού του αρχείου LZMA πρέπει να είναι είτε δύναμη του 2 (2^n) είτε τρεις φορές μια δύναμη του 2 (3\\*2^n).

**Returns:**
int - Μέγεθος λεξικού (buffer ιστορικού).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Επιστρέφει τον αριθμό των bits κυριολεκτικού πλαισίου.

Τα bits κυριολεκτικού πλαισίου ορίζουν πόσα από τα πιο σημαντικά bits του προηγούμενου ασυμπίεστου byte χρησιμοποιούνται για την πρόβλεψη των bits του επόμενου κυριολεκτικού byte. Πρέπει να είναι από 0 έως 8.

**Returns:**
int - ο αριθμός των bits κυριολεκτικού πλαισίου.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Επιστρέφει τον αριθμό των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA.

Μια υψηλότερη τιμή επιτρέπει στον συμπιεστή να αναζητήσει μεγαλύτερες αντιστοιχίες, κάτι που μπορεί να βελτιώσει ελαφρώς τον λόγο συμπίεσης, αλλά επιβραδύνει τη διαδικασία συμπίεσης.

**Returns:**
int - ο αριθμός των byte που χρησιμοποιούνται για γρήγορη αναζήτηση αντιστοιχίας στον αλγόριθμο LZMA.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται.

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

