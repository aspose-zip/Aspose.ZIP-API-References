---
title: "IArchiveFileEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η διεπαφή αντιπροσωπεύει μια καταχώρηση αρχείου αρχειοθήκης."
type: docs
weight: 162
url: /el/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Αυτή η διεπαφή αντιπροσωπεύει μια καταχώρηση αρχείου αρχειοθήκης.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getName()](#getName--) | Λαμβάνει το όνομα του στοιχείου. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή προορισμού. Πρέπει να είναι εγγράψιμη |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί |

**Returns:**
java.io.File - αντικείμενο java.io.File που περιέχει εξαγόμενα δεδομένα
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Λαμβάνει το μήκος της καταχώρησης σε bytes.

**Returns:**
java.lang.Long - το μήκος της καταχώρησης σε bytes
### getName() {#getName--}
```
public abstract String getName()
```


Λαμβάνει το όνομα του στοιχείου.

Αρχεία μόνο για συμπίεση, όπως gzip, bzip2, lzip, lzma, xz, z, έχουν όνομα "File.bin" εκτός εάν βρεθεί άλλο όνομα στις κεφαλίδες.

**Returns:**
java.lang.String - το όνομα της καταχώρησης
