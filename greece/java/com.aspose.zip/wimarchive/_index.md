---
title: "WimArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο αρχειοθέτησης wim."
type: docs
weight: 130
url: /el/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο αρχειοθέτησης wim.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [WimArchive](../../com.aspose.zip/wimarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [WimArchive](../../com.aspose.zip/wimarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [WimArchive](../../com.aspose.zip/wimarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [WimArchive](../../com.aspose.zip/wimarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το αρχείο στη διαδρομή. |
| [getBootImageIndex()](#getBootImageIndex--) | Λαμβάνει το (μηδενικής βάσης) δείκτη της εκκινήσιμης εικόνας. |
| [getEntries()](#getEntries--) | Λαμβάνει καταχωρήσεις τύπου [WimEntry](../../com.aspose.zip/wimentry) που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το wim αρχείο. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Λαμβάνει την έκδοση της μορφής του αρχείου. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getGuid()](#getGuid--) | Λαμβάνει το αναγνωριστικό UUID για το αρχείο. |
| [getImages()](#getImages--) | Λαμβάνει καταχωρήσεις τύπου [WimImage](../../com.aspose.zip/wimimage) που αποτελούν το αρχείο. |
| [getManifest()](#getManifest--) | Λαμβάνει το ενσωματωμένο μανιφέστο που περιγράφει το αρχείο και τις περιεχόμενες εικόνες. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [WimArchive](../../com.aspose.zip/wimarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν φάκελο.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream(\"archive.wim\"))) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [WimArchive](../../com.aspose.zip/wimarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορούν να εξαχθούν από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν φάκελο.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει το αρχείο στη διαδρομή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | java.lang.String | η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Λαμβάνει το (μηδενικής βάσης) δείκτη της εκκινήσιμης εικόνας.

**Returns:**
int - ο (μηδενικής βάσης) δείκτης της εκκινήσιμης εικόνας
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Λαμβάνει καταχωρήσεις τύπου [WimEntry](../../com.aspose.zip/wimentry) που αποτελούν το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - καταχωρήσεις που αποτελούν το αρχείο
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το wim αρχείο.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το wim αρχείο
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Λαμβάνει την έκδοση της μορφής του αρχείου.

**Returns:**
int - η έκδοση της μορφής του αρχείου
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Λαμβάνει το αναγνωριστικό UUID για το αρχείο.

**Returns:**
java.util.UUID - το αναγνωριστικό UUID για το αρχείο
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Λαμβάνει καταχωρήσεις τύπου [WimImage](../../com.aspose.zip/wimimage) που αποτελούν το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - στοιχεία τύπου [WimImage](../../com.aspose.zip/wimimage) που αποτελούν το αρχείο
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Λαμβάνει το ενσωματωμένο μανιφέστο που περιγράφει το αρχείο και τις περιεχόμενες εικόνες.

**Returns:**
java.lang.String - το ενσωματωμένο μανιφέστ που περιγράφει το αρχείο και τις περιεχόμενες εικόνες
