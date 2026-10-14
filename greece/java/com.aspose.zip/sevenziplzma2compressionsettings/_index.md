---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 μέσα σε αρχείο 7z."
type: docs
weight: 114
url: /el/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

Ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 μέσα σε αρχείο 7z.

Το LZMA2 υποστηρίζει πολλαπλές εκτελέσεις συμπιεσμένων δεδομένων LZMA και ασυμπίεστα δεδομένα.

Δείτε περισσότερα: [Lempel\\\\u2013Ziv\\\\u2013Markov\\_chain\\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 σε αρχείο 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 σε αρχείο 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 σε αρχείο 7z. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Λαμβάνει τον αριθμό των νημάτων συμπίεσης. |
| [getDictionarySize()](#getDictionarySize--) | Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη. |
| [getFastBytes()](#getFastBytes--) | Λαμβάνει τον αριθμό ελέγχου των γρήγορων byte που χρησιμοποιεί ο συμπιεστής LZMA2. |
| [getMethod()](#getMethod--) | Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Ορίζει τον αριθμό των νημάτων συμπίεσης. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 σε αρχείο 7z.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 σε αρχείο 7z.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | dictionarySize | int | το μέγεθος του buffer ιστορικού, πρέπει να είναι μεταξύ 4096 και 1073741824. |

Όσο μεγαλύτερο είναι το λεξικό, συνήθως τόσο καλύτερος είναι ο λόγος συμπίεσης - αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


Δημιουργεί ρυθμίσεις για τη μέθοδο συμπίεσης LZMA2 σε αρχείο 7z.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | dictionarySize | int | το μέγεθος του buffer ιστορικού, πρέπει να είναι μεταξύ 4096 και 1073741824. |

Όσο μεγαλύτερο είναι το λεξικό, συνήθως τόσο καλύτερος είναι ο λόγος συμπίεσης - αλλά τα λεξικά μεγαλύτερα από τα ασυμπίεστα δεδομένα είναι σπατάλη μνήμης RAM. |
| fastBytes | int | ελέγχει τον αριθμό των γρήγορων byte που χρησιμοποιούν οι συμπιεστές LZMA2. Ένας μεγαλύτερος αριθμός γρήγορων byte μπορεί να προσφέρει καλύτερο λόγο συμπίεσης με κόστος την ταχύτητα συμπίεσης. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Λαμβάνει τον αριθμό των νημάτων συμπίεσης. Εάν η τιμή είναι μεγαλύτερη από 1, θα χρησιμοποιηθεί συμπίεση πολλαπλών νημάτων.

**Returns:**
int - αριθμός νημάτων συμπίεσης
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Το μέγεθος του λεξικού (buffer ιστορικού) υποδεικνύει πόσα byte των πρόσφατα επεξεργασμένων ασυμπίεστων δεδομένων διατηρούνται στη μνήμη.

**Returns:**
int - μέγεθος λεξικού (buffer ιστορικού)
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Λαμβάνει τον αριθμό ελέγχου των γρήγορων byte που χρησιμοποιεί ο συμπιεστής LZMA2.

**Returns:**
int - ο αριθμός ελέγχου των γρήγορων byte που χρησιμοποιεί ο συμπιεστής LZMA2
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Ορίζει τον αριθμό των νημάτων συμπίεσης. Εάν η τιμή είναι μεγαλύτερη από 1, θα χρησιμοποιηθεί συμπίεση πολυνηματική.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | int | αριθμός νημάτων συμπίεσης. |

Μην ορίσετε αυτόν τον αριθμό μεγαλύτερο από τους πυρήνες CPU. |

