---
title: "AlzEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αναπαριστά μια καταχώριση αρχείου σε ένα αρχείο ALZ μαζί με τα μεταδεδομένα του."
type: docs
weight: 13
url: /el/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Αναπαριστά μια καταχώριση αρχείου σε ένα αρχείο ALZ μαζί με τα μεταδεδομένα του.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση σε μια εγγράψιμη ροή. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Εξάγει την καταχώρηση σε μια εγγράψιμη ροή χρησιμοποιώντας έναν προαιρετικό κωδικό πρόσβασης. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο καθορισμένο αρχείο. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Εξάγει την καταχώρηση στο καθορισμένο αρχείο χρησιμοποιώντας έναν προαιρετικό κωδικό πρόσβασης. |
| [getCompressedSize()](#getCompressedSize--) | Επιστρέφει το συμπιεσμένο μέγεθος των δεδομένων της καταχώρησης σε bytes. |
| [getLength()](#getLength--) | Επιστρέφει το αποσυμπιεσμένο μήκος αυτής της καταχώρησης. |
| [getName()](#getName--) | Επιστρέφει το όνομα της καταχώρησης που αποθηκεύεται στο αρχείο. |
| [getUncompressedSize()](#getUncompressedSize--) | Επιστρέφει το αποσυμπιεσμένο μέγεθος των δεδομένων της καταχώρησης σε bytes. |
| [isDirectory()](#isDirectory--) | Επιστρέφει αν αυτή η καταχώρηση αντιπροσωπεύει έναν φάκελο. |
| [open()](#open--) | Ανοίγει την καταχώρηση και παρέχει μια ροή που περιέχει αποσυμπιεσμένα δεδομένα. |
| [open(String password)](#open-java.lang.String-) | Ανοίγει την καταχώρηση και παρέχει μια ροή που περιέχει αποσυμπιεσμένα δεδομένα. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση σε μια εγγράψιμη ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή προορισμού |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Εξάγει την καταχώρηση σε μια εγγράψιμη ροή χρησιμοποιώντας έναν προαιρετικό κωδικό πρόσβασης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή προορισμού |
| password | java.lang.String | προαιρετικός κωδικός πρόσβασης για αυτήν την καταχώρηση |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει την καταχώρηση στο καθορισμένο αρχείο. Ένα υπάρχον αρχείο αντικαθίσταται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | διαδρομή αρχείου προορισμού |

**Returns:**
java.io.File - εξαγόμενο αρχείο
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Εξάγει την καταχώρηση στο καθορισμένο αρχείο χρησιμοποιώντας έναν προαιρετικό κωδικό πρόσβασης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | διαδρομή αρχείου προορισμού |
| password | java.lang.String | προαιρετικός κωδικός πρόσβασης για αυτήν την καταχώρηση |

**Returns:**
java.io.File - εξαγόμενο αρχείο
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Επιστρέφει το συμπιεσμένο μέγεθος των δεδομένων της καταχώρησης σε bytes.

**Returns:**
long - συμπιεσμένο μέγεθος σε bytes
### getLength() {#getLength--}
```
public final Long getLength()
```


Επιστρέφει το αποσυμπιεσμένο μήκος αυτής της καταχώρησης.

**Returns:**
java.lang.Long - μη συμπιεσμένο μήκος σε bytes
### getName() {#getName--}
```
public final String getName()
```


Επιστρέφει το όνομα της καταχώρησης που αποθηκεύεται στο αρχείο.

**Returns:**
java.lang.String - όνομα καταχώρησης
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Επιστρέφει το αποσυμπιεσμένο μέγεθος των δεδομένων της καταχώρησης σε bytes.

**Returns:**
long - μη συμπιεσμένο μέγεθος σε bytes
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Επιστρέφει αν αυτή η καταχώρηση αντιπροσωπεύει έναν φάκελο.

**Returns:**
boolean - `true` για καταχώρηση καταλόγου
### open() {#open--}
```
public final InputStream open()
```


Ανοίγει την καταχώρηση και παρέχει μια ροή που περιέχει αποσυμπιεσμένα δεδομένα.

**Returns:**
java.io.InputStream - ροή που περιέχει αποσυμπιεσμένα δεδομένα καταχώρησης
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Ανοίγει την καταχώρηση και παρέχει μια ροή που περιέχει αποσυμπιεσμένα δεδομένα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | java.lang.String | προαιρετικός κωδικός πρόσβασης για αυτήν την καταχώρηση |

**Returns:**
java.io.InputStream - ροή που περιέχει αποσυμπιεσμένα δεδομένα καταχώρησης
