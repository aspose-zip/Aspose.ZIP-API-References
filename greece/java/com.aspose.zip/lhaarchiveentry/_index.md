---
title: "LhaArchiveEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μοναδικό αρχείο μέσα σε αρχείο Lha."
type: docs
weight: 76
url: /el/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει ένα μοναδικό αρχείο μέσα σε αρχείο Lha.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Εξάγει την καταχώρηση Lha σε αρχείο. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση Lha σε σύστημα αρχείων με βάση τη διαδρομή. |
| [getLastModified()](#getLastModified--) | Αποκτά την ώρα τελευταίας τροποποίησης της καταχώρησης. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getModificationTime()](#getModificationTime--) | Αποκτά την ώρα τελευταίας τροποποίησης της καταχώρησης. |
| [getName()](#getName--) | Λαμβάνει το όνομα του στοιχείου. |
| [getPath()](#getPath--) | Αποκτά την πλήρη διαδρομή προς την καταχώρηση. |
| [isDirectory()](#isDirectory--) | Αποκτά μια τιμή που υποδεικνύει εάν αυτή η καταχώρηση είναι κατάλογος. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Εξάγει την καταχώρηση Lha σε αρχείο.

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο που θα αποθηκεύσει τα αποσυμπιεσμένα δεδομένα |

**Returns:**
java.io.File - αντικείμενο java.io.File που περιέχει εξαγόμενα δεδομένα
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Αποκτά την ώρα τελευταίας τροποποίησης της καταχώρησης.

**Returns:**
java.util.Date - η ώρα τελευταίας τροποποίησης της καταχώρησης
### getLength() {#getLength--}
```
public final Long getLength()
```


Λαμβάνει το μήκος της καταχώρησης σε bytes.

**Returns:**
java.lang.Long - το μήκος της καταχώρησης σε bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Αποκτά την ώρα τελευταίας τροποποίησης της καταχώρησης.

**Returns:**
java.util.Date - η ώρα τελευταίας τροποποίησης της καταχώρησης
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα του στοιχείου.

Αρχεία μόνο για συμπίεση, όπως gzip, bzip2, lzip, lzma, xz, z, έχουν όνομα "File.bin" εκτός εάν βρεθεί άλλο όνομα στις κεφαλίδες.

**Returns:**
java.lang.String - το όνομα της καταχώρησης
### getPath() {#getPath--}
```
public final String getPath()
```


Αποκτά την πλήρη διαδρομή προς την καταχώρηση.

**Returns:**
java.lang.String - η πλήρης διαδρομή προς την καταχώρηση
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Αποκτά μια τιμή που υποδεικνύει εάν αυτή η καταχώρηση είναι κατάλογος.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν αυτή η καταχώρηση είναι κατάλογος.
