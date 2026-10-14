---
title: "CpioArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο cpio."
type: docs
weight: 57
url: /el/java/com.aspose.zip/cpioarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class CpioArchive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο cpio.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [CpioArchive()](#CpioArchive--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CpioArchive](../../com.aspose.zip/cpioarchive). |
| [CpioArchive(InputStream sourceStream)](#CpioArchive-java.io.InputStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CpioArchive](../../com.aspose.zip/cpioarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [CpioArchive(String path)](#CpioArchive-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CpioArchive](../../com.aspose.zip/cpioarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
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
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [deleteEntry(CpioEntry entry)](#deleteEntry-com.aspose.zip.CpioEntry-) | Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων με βάση το δείκτη. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο. |
| [getEntries()](#getEntries--) | Αποκτά καταχωρήσεις τύπου [CpioEntry](../../com.aspose.zip/cpioentry) που αποτελούν το cpio αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο cpio. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(OutputStream output, CpioFormat cpioFormat)](#save-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [save(String destinationFileName, CpioFormat cpioFormat)](#save-java.lang.String-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [saveGzipped(OutputStream output, CpioFormat cpioFormat)](#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση gzip. |
| [saveGzipped(String path, CpioFormat cpioFormat)](#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση gzip. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA. |
| [saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzma. |
| [saveLZMACompressed(String path, CpioFormat cpioFormat)](#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip. |
| [saveLzipped(OutputStream output, CpioFormat cpioFormat)](#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzip. |
| [saveLzipped(String path, CpioFormat cpioFormat)](#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz. |
| [saveXzCompressed(String path, CpioFormat cpioFormat)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz. |
| [saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Z. |
| [saveZCompressed(OutputStream output, CpioFormat cpioFormat)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Z. |
| [saveZCompressed(String path, CpioFormat cpioFormat)](#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Zstandard. |
| [saveZstandard(OutputStream output, CpioFormat cpioFormat)](#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Zstandard. |
| [saveZstandard(String path, CpioFormat cpioFormat)](#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Zstandard. |
### CpioArchive() {#CpioArchive--}
```
public CpioArchive()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CpioArchive](../../com.aspose.zip/cpioarchive).

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```



### CpioArchive(InputStream sourceStream) {#CpioArchive-java.io.InputStream-}
```
public CpioArchive(InputStream sourceStream)
```


Initializes a new instance of the [CpioArchive](../../com.aspose.zip/cpioarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CpioArchive archive = new CpioArchive(new FileInputStream("archive.cpio"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |

### CpioArchive(String path) {#CpioArchive-java.lang.String-}
```
public CpioArchive(String path)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [CpioArchive](../../com.aspose.zip/cpioarchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν κατάλογο.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CpioArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | java.io.File | κατάλογος προς συμπίεση |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CpioArchive createEntries(File directory, boolean includeRootDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CpioArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | java.lang.String | κατάλογος προς συμπίεση |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CpioArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final CpioEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new File("data.bin");
     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | το όνομα του στοιχείου |
| file | java.io.File | τα μεταδεδομένα του αρχείου ή του φακέλου που θα συμπιεστεί |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final CpioEntry createEntry(String name, File file, boolean openImmediately)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

java.io.File file = new File("data.bin");
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CpioEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.cpio");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | το όνομα του στοιχείου |
| source | java.io.InputStream | η ροή εισόδου για την καταχώρηση |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final CpioEntry createEntry(String name, String sourcePath)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | path to file to be compressed. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final CpioEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.cpio");
     }
 
```

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα αρχείου που παρέχεται στην παράμετρο `sourcePath` δεν επηρεάζει το όνομα της καταχώρησης

Εάν το αρχείο ανοίξει αμέσως με την παράμετρο `openImmediately`, παραμένει κλειδωμένο μέχρι να αποδεσμευθεί το αρχείο

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | το όνομα του στοιχείου |
| sourcePath | java.lang.String | διαδρομή προς το αρχείο που θα συμπιεστεί. |
| openImmediately | boolean | αληθές, εάν το αρχείο ανοιχτεί αμέσως, διαφορετικά ανοίγεται κατά την αποθήκευση του αρχείου. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### deleteEntry(CpioEntry entry) {#deleteEntry-com.aspose.zip.CpioEntry-}
```
public final CpioArchive deleteEntry(CpioEntry entry)
```


Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων.

Ακολουθεί πώς μπορείτε να αφαιρέσετε όλες τις καταχωρήσεις εκτός της τελευταίας:

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputCpioFile.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [CpioEntry](../../com.aspose.zip/cpioentry) | the entry to remove from the entries list |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final CpioArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (CpioArchive archive = new CpioArchive("two_files.cpio")) {
         archive.deleteEntry(0);
         archive.save("single_file.cpio");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entryIndex | int | ο δείκτης μηδενικής βάσης της καταχώρησης που θα αφαιρεθεί |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<CpioEntry> getEntries()
```


Gets entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.

**Returns:**
java.util.List&lt;com.aspose.zip.CpioEntry&gt; - entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |

### save(OutputStream output, CpioFormat cpioFormat) {#save-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void save(OutputStream output, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στη δοθείσα ροή.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

Είναι δυνατόν να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο |

### save(String destinationFileName, CpioFormat cpioFormat) {#save-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void save(String destinationFileName, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |

### saveGzipped(OutputStream output, CpioFormat cpioFormat) {#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(OutputStream output, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.cpio.gz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### saveGzipped(String path, CpioFormat cpioFormat) {#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(String path, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.cpio.gz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Saves the archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Σημαντικό: το cpio αρχείο δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |

### saveLZMACompressed(OutputStream output, CpioFormat cpioFormat) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Saves the archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.cpio.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Σημαντικό: το cpio αρχείο δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### saveLZMACompressed(String path, CpioFormat cpioFormat) {#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(String path, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.cpio.lzma");
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |

### saveLzipped(OutputStream output, CpioFormat cpioFormat) {#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(OutputStream output, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.cpio.lz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### saveLzipped(String path, CpioFormat cpioFormat) {#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(String path, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.cpio.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output`Η ροή πρέπει να είναι εγγράψιμη |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output`Η ροή πρέπει να είναι εγγράψιμη. |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | ορίζει τη μορφή κεφαλίδας cpio |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | σύνολο ρυθμίσεων συγκεκριμένου αρχείου xz: μέγεθος λεξικού, μέγεθος μπλοκ, τύπος ελέγχου |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveXzCompressed(String path, CpioFormat cpioFormat) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.cpio.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | ορίζει τη μορφή κεφαλίδας cpio |

### saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | η ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |

### saveZCompressed(OutputStream output, CpioFormat cpioFormat) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(OutputStream output, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.cpio.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### saveZCompressed(String path, CpioFormat cpioFormat) {#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(String path, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.cpio.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | d cpio header format |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |

### saveZstandard(OutputStream output, CpioFormat cpioFormat) {#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(OutputStream output, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.cpio.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### saveZstandard(String path, CpioFormat cpioFormat) {#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(String path, CpioFormat cpioFormat)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.cpio.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

