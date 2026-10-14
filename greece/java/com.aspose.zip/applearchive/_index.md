---
title: "AppleArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Apple Archive .aar."
type: docs
weight: 16
url: /el/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Apple Archive (.aar). Χρησιμοποιήστε την για τη δημιουργία αρχείων Apple Archive.

Apple και Apple Archive είναι εμπορικά σήματα της Apple Inc.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) με ρυθμίσεις που χρησιμοποιούνται για τις συντεθειμένες καταχωρίσεις. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) με ρυθμίσεις που χρησιμοποιούνται για τις συντεθειμένες καταχωρίσεις. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [dispose()](#dispose--) | Εκτελεί εργασίες που ορίζονται από την εφαρμογή και σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο. |
| [getEntries()](#getEntries--) | Λαμβάνει τις καταχωρίσεις που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Λαμβάνει τις ρυθμίσεις που χρησιμοποιούνται για τις νεοσυντεθειμένες καταχωρίσεις. |
| [isSolid()](#isSolid--) | Λαμβάνει μια τιμή που υποδεικνύει αν το αρχείο χρησιμοποιεί συμπίεση solid. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο σε ένα προσαρμοσμένο αρχείο προορισμού. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) με ρυθμίσεις που χρησιμοποιούνται για τις συντεθειμένες καταχωρίσεις.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) με ρυθμίσεις που χρησιμοποιούνται για τις συντεθειμένες καταχωρίσεις.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Ρυθμίσεις που χρησιμοποιούνται κατά τη δημιουργία ενός νέου Apple Archive. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | Η πηγή του αρχείου. |

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τις μεθόδους [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) και [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) για αποσυμπίεση. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Η πηγή του αρχείου. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τις μεθόδους [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) και [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) για αποσυμπίεση. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η πλήρως καθορισμένη ή η σχετική διαδρομή προς το αρχείο του αρχείου. |

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τις μεθόδους [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) και [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) για αποσυμπίεση. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleArchive](../../com.aspose.zip/applearchive) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η πλήρως καθορισμένη ή η σχετική διαδρομή προς το αρχείο του αρχείου. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τις μεθόδους [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) και [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) για αποσυμπίεση. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | java.io.File | Κατάλογος προς συμπίεση. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | java.io.File | Κατάλογος προς συμπίεση. |
| includeRootDirectory | boolean | Υποδεικνύει αν θα συμπεριληφθεί ο ριζικός κατάλογος ο ίδιος ή όχι. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| fileInfo | java.io.File | Τα μεταδεδομένα του αρχείου προς συμπίεση. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| fileInfo | java.io.File | Τα μεταδεδομένα του αρχείου προς συμπίεση. |
| openImmediately | boolean | Αληθές, εάν το αρχείο ανοίξει αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση του αρχείου. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| source | java.io.InputStream | Η ροή εισόδου για το στοιχείο. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| path | java.lang.String | Η διαδρομή προς το αρχείο προς συμπίεση. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| path | java.lang.String | Η διαδρομή προς το αρχείο προς συμπίεση. |
| openImmediately | boolean | Αληθές, εάν το αρχείο ανοίξει αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση του αρχείου. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Εκτελεί εργασίες που ορίζονται από την εφαρμογή και σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Λαμβάνει τις καταχωρίσεις που αποτελούν το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - καταχωρίσεις που αποτελούν το αρχείο.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρίσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Λαμβάνει τις ρυθμίσεις που χρησιμοποιούνται για τις νεοσυντεθειμένες καταχωρίσεις.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το αρχείο χρησιμοποιεί συμπίεση solid. Σε λειτουργία solid, όλα τα δεδομένα των καταχωρίσεων συμπιέζονται ως ένα ενιαίο ρεύμα και η ατομική εξαγωγή καταχωρίσεων δεν είναι διαθέσιμη. Χρησιμοποιήστε το [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) αντ' αυτού.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν το αρχείο χρησιμοποιεί συμπίεση solid.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Αποθηκεύει το αρχείο στη δοθείσα ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | Ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο. Ορισμένες ρυθμίσεις συμπίεσης, όπως το LZ4, απαιτούν επίσης ένα ρεύμα με δυνατότητα αναζήτησης. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Αποθηκεύει το αρχείο σε ένα προσαρμοσμένο αρχείο προορισμού.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | java.lang.String | Η διαδρομή του αρχείου που θα δημιουργηθεί. |

