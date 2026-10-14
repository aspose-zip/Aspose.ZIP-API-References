---
title: "IArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η διεπαφή αντιπροσωπεύει μια αρχειοθήκη."
type: docs
weight: 161
url: /el/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Αυτή η διεπαφή αντιπροσωπεύει μια αρχειοθήκη.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο.

Αν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο.

Τα αρχεία μόνο για συμπίεση, όπως gzip, bzip2, lzip, lzma, lz4, xz, z, αποτελούν το μοναδικό αρχείο - το ίδιο το αρχείο.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
