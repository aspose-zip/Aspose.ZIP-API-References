---
title: "IsoArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αναπαριστά ένα αρχείο ISO ISO 9660."
type: docs
weight: 71
url: /el/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Αντιπροσωπεύει ένα αρχείο ISO (ISO 9660).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και δημιουργεί ένα κενό αρχείο ISO για την προσθήκη νέων αρχείων και καταλόγων. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Προσθέτει έναν κατάλογο στην εικόνα ISO. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Προσθέτει ένα αρχείο στην εικόνα ISO. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Προσθέτει ένα αρχείο στην εικόνα ISO. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Προσθέτει ένα αρχείο στην εικόνα ISO. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλες τις καταχωρήσεις στον καθορισμένο κατάλογο. |
| [getEntries()](#getEntries--) | Λαμβάνει καταχωρήσεις τύπου [IsoEntry](../../com.aspose.zip/isoentry) που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Αποθηκεύει την εικόνα ISO στο καθορισμένο ρεύμα. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Αποθηκεύει την εικόνα ISO στο καθορισμένο ρεύμα. |
| [save(String path)](#save-java.lang.String-) | Αποθηκεύει την εικόνα ISO στη καθορισμένη διαδρομή. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Αποθηκεύει την εικόνα ISO στη καθορισμένη διαδρομή. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και δημιουργεί ένα κενό αρχείο ISO για την προσθήκη νέων αρχείων και καταλόγων.

Το παρακάτω παράδειγμα δείχνει πώς να δημιουργήσετε ένα νέο κενό αρχείο ISO και να προσθέσετε αρχεία σε αυτό:

```

``````

// Δημιουργήστε ένα νέο κενό αρχείο ISO
try (IsoArchive isoArchive = new IsoArchive()) {
// Προσθέστε αρχεία στο αρχείο ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Αποθηκεύστε το αρχείο ISO σε ένα αρχείο
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν κατάλογο.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [IsoArchive](../../com.aspose.zip/isoarchive) και συνθέτει μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν κατάλογο.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | java.lang.String | ο φάκελος στον οποίο θα εξαχθούν οι καταχωρήσεις |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Λαμβάνει καταχωρήσεις τύπου [IsoEntry](../../com.aspose.zip/isoentry) που αποτελούν το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - καταχωρήσεις τύπου [IsoEntry](../../com.aspose.zip/isoentry) που αποτελούν το iso αρχείο
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το iso αρχείο
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Αποθηκεύει την εικόνα ISO στο καθορισμένο ρεύμα.

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε ένα ISO αρχείο σε ροή μνήμης:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Δημιουργήστε ένα νέο κενό αρχείο ISO
try (IsoArchive isoArchive = new IsoArchive()) {
// Προσθέστε αρχεία στο αρχείο ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Αποθήκευση του ISO αρχείου σε ροή μνήμης
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | η ροή στην οποία θα αποθηκευτεί η εικόνα ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | οι επιλογές για την αποθήκευση του ISO αρχείου |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Αποθηκεύει την εικόνα ISO στη καθορισμένη διαδρομή.

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε ένα ISO αρχείο σε αρχείο:

```

``````

// Δημιουργήστε ένα νέο κενό αρχείο ISO
try (IsoArchive isoArchive = new IsoArchive()) {
// Προσθέστε αρχεία στο αρχείο ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Αποθηκεύστε το αρχείο ISO σε ένα αρχείο
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή στην οποία θα αποθηκευτεί η εικόνα ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | οι επιλογές για την αποθήκευση του ISO αρχείου |

