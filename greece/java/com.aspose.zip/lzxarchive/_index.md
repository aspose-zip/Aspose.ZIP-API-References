---
title: "LzxArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LZX .lzx."
type: docs
weight: 89
url: /el/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LZX (.lzx).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LzxArchive](../../com.aspose.zip/lzxarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LzxArchive](../../com.aspose.zip/lzxarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LzxArchive](../../com.aspose.zip/lzxarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LzxArchive](../../com.aspose.zip/lzxarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία και τους καταλόγους στο αρχείο στον παρεχόμενο φάκελο. |
| [getEntries()](#getEntries--) | Αποκτά τις καταχωρήσεις αρχείων τύπου [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LzxArchive](../../com.aspose.zip/lzxarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Η πηγή του αρχείου. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LzxArchive](../../com.aspose.zip/lzxarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| extractionSource | java.io.InputStream | Η πηγή του αρχείου. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [LzxArchive](../../com.aspose.zip/lzxarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Το παρακάτω παράδειγμα εξάγει ένα αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώρηση σε ένα `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η πλήρως καθορισμένη ή η σχετική διαδρομή προς το αρχείο του αρχείου. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

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

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
