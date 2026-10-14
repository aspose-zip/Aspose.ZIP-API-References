---
title: "LhaArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LHA .lzh."
type: docs
weight: 75
url: /el/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LHA (.lzh).

Μόνο οι ακόλουθες μέθοδοι συμπίεσης υποστηρίζονται:

| ------ | --------------------------------------------- |
| Method | Explanation                                   |
| lh0    | Ασυμπίεστο                                  |
| lh4    | 8 KiB λεξικό κυλιόμενου παραθύρου και στατικός Huffman   |
| lh5    | 16 KiB λεξικό κυλιόμενου παραθύρου και στατικός Huffman  |
| lh6    | 64 KiB λεξικό κυλιόμενου παραθύρου και στατικός Huffman  |
| lh7    | 128 KiB λεξικό κυλιόμενου παραθύρου και στατικός Huffman |
| lhx    | 1 Mib λεξικό κυλιόμενου παραθύρου και στατικός Huffman   |
| lhd    | Κατάλογος                                     |
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LhaArchive](../../com.aspose.zip/lhaarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LhaArchive](../../com.aspose.zip/lhaarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LhaArchive](../../com.aspose.zip/lhaarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LhaArchive](../../com.aspose.zip/lhaarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία και τους καταλόγους στο αρχείο στον παρεχόμενο φάκελο. |
| [getEntries()](#getEntries--) | Λαμβάνει καταχωρήσεις αρχείων τύπου [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LhaArchive](../../com.aspose.zip/lhaarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LhaArchive](../../com.aspose.zip/lhaarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LhaArchive](../../com.aspose.zip/lhaarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Το παρακάτω παράδειγμα εξάγει ένα αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώρηση σε ένα `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η πλήρως καθορισμένη ή η σχετική διαδρομή προς το αρχείο |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία και τους καταλόγους στο αρχείο στον παρεχόμενο φάκελο.

```

``````

try (LhaArchive archive = new LhaArchive(\"archive.lzh\")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
