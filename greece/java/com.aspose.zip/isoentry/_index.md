---
title: "IsoEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αναπαριστά ένα αρχείο ή κατάλογο στοιχείου μέσα σε ένα αρχείο ISO."
type: docs
weight: 72
url: /el/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει μια καταχώρηση (αρχείο ή φάκελο) μέσα σε ένα αρχείο ISO.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος του στοιχείου. |
| [getModificationTime()](#getModificationTime--) | Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [getName()](#getName--) | Λαμβάνει το όνομα του στοιχείου. |
| [isDirectory()](#isDirectory--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το στοιχείο είναι κατάλογος. |
| [toString()](#toString--) | Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει την τρέχουσα καταχώρηση. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή προορισμού |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |

**Returns:**
java.io.File - αντικείμενο java.io.File που περιέχει εξαγόμενα δεδομένα
### getLength() {#getLength--}
```
public Long getLength()
```


Λαμβάνει το μήκος του στοιχείου.

**Returns:**
java.lang.Long - το μήκος της καταχώρησης
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης.

**Returns:**
java.util.Date - ημερομηνία και ώρα τελευταίας τροποποίησης
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα του στοιχείου.

**Returns:**
java.lang.String - το όνομα της καταχώρησης
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το στοιχείο είναι κατάλογος.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν η καταχώρηση αντιπροσωπεύει κατάλογο
### toString() {#toString--}
```
public String toString()
```


Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει την τρέχουσα καταχώρηση.

**Returns:**
java.lang.String - το όνομα της καταχώρησης
