---
title: "Archive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αναπαριστά ένα αρχείο zip."
type: docs
weight: 26
url: /el/java/com.aspose.zip/archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class Archive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο zip. Χρησιμοποιήστε την για σύνθεση, εξαγωγή ή ενημέρωση αρχείων zip.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Archive()](#Archive--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της. |
| [Archive(ArchiveEntrySettings newEntrySettings)](#Archive-com.aspose.zip.ArchiveEntrySettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της. |
| [Archive(InputStream sourceStream)](#Archive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [Archive(String path)](#Archive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [Archive(String path, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [Archive(String mainSegment, String[] segmentsInOrder)](#Archive-java.lang.String-java.lang.String---) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) από πολυτόμο αρχείο ZIP και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) από πολυτόμο αρχείο ZIP και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [deleteEntry(ArchiveEntry entry)](#deleteEntry-com.aspose.zip.ArchiveEntry-) | Αφαιρεί την πρώτη εμφάνιση της συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων με βάση το δείκτη. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο. |
| [getComment()](#getComment--) | Λαμβάνει το σχόλιο για ολόκληρο το αρχείο. |
| [getEntries()](#getEntries--) | Λαμβάνει τις καταχωρήσεις τύπου [ArchiveEntry](../../com.aspose.zip/archiveentry) που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Λαμβάνει τη μορφή του αρχείου (Zip) |
| [getNewEntrySettings()](#getNewEntrySettings--) | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για πρόσφατα προστιθέμενα στοιχεία [ArchiveEntry](../../com.aspose.zip/archiveentry). |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(OutputStream outputStream, ArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [save(String destinationFileName, ArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-) | Αποθηκεύει το πολυτόμο αρχείο στον προορισμένο κατάλογο που δόθηκε. |
### Archive() {#Archive--}
```
public Archive()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της.


Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα μόνο αρχείο με τις προεπιλεγμένες ρυθμίσεις.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```



### Archive(ArchiveEntrySettings newEntrySettings) {#Archive-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries.


The following example shows how to compress a single file with default settings.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα στοιχεία [ArchiveEntry](../../com.aspose.zip/archiveentry). Εάν δεν καθοριστούν, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

### Archive(InputStream sourceStream) {#Archive-java.io.InputStream-}
```
public Archive(InputStream sourceStream)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα εξάγει ένα κρυπτογραφημένο αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώρηση σε ένα `ByteArrayOutputStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Η πηγή του αρχείου. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα εξάγει ένα κρυπτογραφημένο αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώρηση σε ένα `ByteArrayOutputStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, the most common Deflate compression without encryption would be used. |

### Archive(String path) {#Archive-java.lang.String-}
```
public Archive(String path)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η πλήρως καθορισμένη ή η σχετική διαδρομή προς το αρχείο του αρχείου. |

### Archive(String path, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String path, ArchiveLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα εξάγει ένα κρυπτογραφημένο αρχείο, στη συνέχεια αποσυμπιέζει την πρώτη καταχώρηση σε ένα `ByteArrayOutputStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive("encrypted.zip", options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |

### Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η πλήρως καθορισμένη ή η σχετική διαδρομή προς το αρχείο του αρχείου. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τα πρόσφατα προστιθέμενα στοιχεία [ArchiveEntry](../../com.aspose.zip/archiveentry). Εάν δεν καθοριστούν, θα χρησιμοποιηθεί η πιο κοινή συμπίεση Deflate χωρίς κρυπτογράφηση. |

### Archive(String mainSegment, String[] segmentsInOrder) {#Archive-java.lang.String-java.lang.String---}
```
public Archive(String mainSegment, String[] segmentsInOrder)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) από πολυτόμο αρχείο ZIP και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

```

``````

try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
a.extractToDirectory("destination");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mainSegment | java.lang.String | Path to the last segment of multi-volume archive with the central directory.

Usually this segment has \*.zip extension and smaller than others. |
| segmentsInOrder | java.lang.String[] | Paths to each segment but the last of multi-volume zip archive respecting order.

Usually they named filename.z01, filename.z02, ..., filename.z(n-1). |

### Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class from multi-volume ZIP archive and composes an entry list can be extracted from the archive.

This sample extract to a directory an archive of three segments.

```

``````

     try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
         a.extractToDirectory("destination");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | mainSegment | java.lang.String | Διαδρομή προς το τελευταίο τμήμα του πολυ-τόμου αρχείου με τον κεντρικό κατάλογο. |

Συνήθως αυτό το τμήμα έχει επέκταση \\*.zip και είναι μικρότερο από τα άλλα. |
|  | segmentsInOrder | java.lang.String[] | Διαδρομές προς κάθε τμήμα εκτός του τελευταίου του πολυ-τόμου zip αρχείου, τηρώντας τη σειρά. |

Συνήθως ονομάζονται filename.z01, filename.z02, ..., filename.z(n-1). |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final Archive createEntries(File directory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```

``````

try (Archive archive = new Archive()) {
java.io.File folder = new java.io.File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final Archive createEntries(File directory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        java.io.File folder = new java.io.File("C:\\folder");
        archive.createEntries(folder);
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | java.io.File | Κατάλογος προς συμπίεση. |
| includeRootDirectory | boolean | Υποδεικνύει αν θα συμπεριληφθεί ο ριζικός κατάλογος ο ίδιος ή όχι. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final Archive createEntries(String sourceDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```

``````

try (Archive archive = new Archive()) {
archive.createEntries("C:\\folder");
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final Archive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntries("C:\\folder");
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Κατάλογος προς συμπίεση. |
| includeRootDirectory | boolean | Υποδεικνύει αν θα συμπεριληφθεί ο ριζικός κατάλογος ο ίδιος ή όχι. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final ArchiveEntry createEntry(String name, File file)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

Δημιουργήστε αρχείο με καταχωρήσεις κρυπτογραφημένες με διαφορετικές μεθόδους κρυπτογράφησης και κωδικούς πρόσβασης για κάθε μία.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different encryption methods and passwords each.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα του αρχείου που παρέχεται στην παράμετρο `file` δεν επηρεάζει το όνομα της καταχώρησης.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο `openImmediately`, παραμένει κλειδωμένο μέχρι να αποθηκευτεί το αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| file | java.io.File | Τα μεταδεδομένα του αρχείου προς συμπίεση. |
| openImmediately | boolean | Αληθές, εάν το αρχείο ανοίξει αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση του αρχείου. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

Δημιουργήστε αρχείο με καταχωρήσεις κρυπτογραφημένες με διαφορετικές μεθόδους κρυπτογράφησης και κωδικούς πρόσβασης για κάθε μία.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final ArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.zip");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| source | java.io.InputStream | Η ροή εισόδου για το στοιχείο. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {
                    0x00,
                    (byte) 0xFF
            }), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new java.io.File("data1.bin"));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα του αρχείου που παρέχεται στην παράμετρο `file` δεν επηρεάζει το όνομα της καταχώρησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| source | java.io.InputStream | Η ροή εισόδου για το στοιχείο. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για το προστιθέμενο στοιχείο [ArchiveEntry](../../com.aspose.zip/archiveentry). |
| file | java.io.File | Τα μεταδεδομένα του αρχείου ή του φακέλου που θα συμπιεστούν. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final ArchiveEntry createEntry(String name, String path)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

Το όνομα του στοιχείου ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα αρχείου που παρέχεται στην παράμετρο `path` δεν επηρεάζει το όνομα του στοιχείου.

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο `openImmediately`, παραμένει κλειδωμένο μέχρι να αποθηκευτεί το αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | Το όνομα της καταχώρησης. |
| path | java.lang.String | Το πλήρως προσδιορισμένο όνομα του νέου αρχείου ή το σχετικό όνομα αρχείου που θα συμπιεστεί. |
| openImmediately | boolean | Αληθές, εάν το αρχείο ανοίξει αμέσως, διαφορετικά ανοίξτε το αρχείο κατά την αποθήκευση του αρχείου. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("data.bin", "file.dat");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

     Supplier<InputStream> provider = new Supplier<InputStream>() {
         public InputStream get() {
             return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
         }
     };
     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
             archive.save(zipFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | το όνομα του στοιχείου |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | η μέθοδος που παρέχει τη ροή εισόδου για το στοιχείο |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, ArchiveEntrySettings newEntrySettings)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

Δημιουργήστε αρχείο με κρυπτογραφημένο στοιχείο.

```

``````

Supplier<InputStream> provider = new Supplier<InputStream>() {
public InputStream get() {
return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
}
};
try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.save(zipFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | the method providing input stream for the entry |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### deleteEntry(ArchiveEntry entry) {#deleteEntry-com.aspose.zip.ArchiveEntry-}
```
public final Archive deleteEntry(ArchiveEntry entry)
```


Removes the first occurrence of the specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        while (archive.getEntries().size() > 1)
            archive.deleteEntry(archive.getEntries().get(0));
        archive.save("last_entry.zip");
    }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Η καταχώρηση που θα αφαιρεθεί από τη λίστα καταχωρήσεων. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final Archive deleteEntry(int entryIndex)
```


Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων με βάση το δείκτη.

```

``````

try (Archive archive = new Archive("two_files.zip")) {
archive.deleteEntry(0);
archive.save("single_file.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | The zero-based index of the entry to remove. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        archive.extractToDirectory("C:\\extracted");
    }
 
```

Αν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

### getComment() {#getComment--}
```
public final String getComment()
```


Λαμβάνει το σχόλιο για ολόκληρο το αρχείο.

Αν παρέχεται το `ArchiveLoadOptions.Encoding`([ArchiveLoadOptions.getEncoding](../../com.aspose.zip/archiveloadoptions\\#getEncoding)/[ArchiveLoadOptions.setEncoding](../../com.aspose.zip/archiveloadoptions\\#setEncoding)), αποκωδικοποιείται χρησιμοποιώντας το. Διαφορετικά, χρησιμοποιείται UTF-8.

**Returns:**
java.lang.String - σχόλιο για ολόκληρο το αρχείο.
### getEntries() {#getEntries--}
```
public final List<ArchiveEntry> getEntries()
```


Λαμβάνει τις καταχωρήσεις τύπου [ArchiveEntry](../../com.aspose.zip/archiveentry) που αποτελούν το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.ArchiveEntry&gt; - καταχωρήσεις τύπου [ArchiveEntry](../../com.aspose.zip/archiveentry) που αποτελούν το αρχείο.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Λαμβάνει τη μορφή του αρχείου (Zip)

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - Zip archive format.
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final ArchiveEntrySettings getNewEntrySettings()
```


Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για πρόσφατα προστιθέμενα στοιχεία [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Returns:**
[ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) - the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) instance
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Αποθηκεύει το αρχείο στη δοθείσα ροή.

```

``````

try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

`outputStream` must be writable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream. |

### save(OutputStream outputStream, ArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(OutputStream outputStream, ArchiveSaveOptions saveOptions)
```


Saves archive to the stream provided.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry.bin", "data.bin");
            archive.save(zipFile);
        }
    } catch (IOException ex) {
    }
 
```

`outputStream` πρέπει να είναι εγγράψιμο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Ροή προορισμού. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Επιλογές για την αποθήκευση του αρχείου. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncoding(StandardCharsets.US_ASCII);
archive.save("archive.zip", options);
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, ArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(String destinationFileName, ArchiveSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncoding(StandardCharsets.US_ASCII);
        archive.save("archive.zip", options);
    }
 
```

Είναι δυνατόν να αποθηκευτεί ένα αρχείο στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | java.lang.String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Επιλογές για την αποθήκευση του αρχείου. |

### saveSplit(String destinationDirectory, SplitArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)
```


Αποθηκεύει το πολυτόμο αρχείο στον προορισμένο κατάλογο που δόθηκε.

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.saveSplit( "C:\\Folder", new SplitArchiveSaveOptions("volume", 65536));
}
 
```

This method composes several (n) files filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Cannot make existing archive multi-volume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory where archive segments to be created. |
| options | [SplitArchiveSaveOptions](../../com.aspose.zip/splitarchivesaveoptions) | Options for archive saving, including file name. |

