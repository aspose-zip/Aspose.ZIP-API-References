---
title: "ArjArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο ARJ."
type: docs
weight: 37
url: /el/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο ARJ.

Μόνο οι ακόλουθες μέθοδοι συμπίεσης υποστηρίζονται:

| ------ | ------------------------------------------------------------ |
| Μέθοδος | Εξήγηση                                                  |
| 0      | Ασυμπίεστο                                                 |
| 1      | Συνδυασμός LZ77 και προσαρμοστικού κωδικοποιητή Huffman. Καλύτερος λόγος. |
| 2      | Συνδυασμός LZ77 και προσαρμοστικού κωδικοποιητή Huffman.             |
| 3      | Συνδυασμός LZ77 και προσαρμοστικού κωδικοποιητή Huffman. Καλύτερη ταχύτητα. |
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ArjArchive](../../com.aspose.zip/arjarchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ArjArchive](../../com.aspose.zip/arjarchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ArjArchive](../../com.aspose.zip/arjarchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ArjArchive](../../com.aspose.zip/arjarchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλες τις καταχωρήσεις στον καθορισμένο κατάλογο. |
| [getCommentary()](#getCommentary--) | Λαμβάνει το σχόλιο. |
| [getEntries()](#getEntries--) | Λαμβάνει καταχωρίσεις τύπου [ArjEntryPlain](../../com.aspose.zip/arjentryplain) που αποτελούν το αρχείο ARJ. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getName()](#getName--) | Λαμβάνει το αρχικό όνομα. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ArjArchive](../../com.aspose.zip/arjarchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τη μέθοδο [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| extractionSource | java.io.InputStream | η πηγή του αρχείου |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ArjArchive](../../com.aspose.zip/arjarchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τη μέθοδο [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| extractionSource | java.io.InputStream | η πηγή του αρχείου |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ArjArchive](../../com.aspose.zip/arjarchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν κατάλογο.

```

``````

try (ArjArchive archive = new ArjArchive(\"archive.arj\")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τη μέθοδο [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλες τις καταχωρήσεις στον καθορισμένο κατάλογο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρίσεις σε έναν φάκελο:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream(\"archive.arj\"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
