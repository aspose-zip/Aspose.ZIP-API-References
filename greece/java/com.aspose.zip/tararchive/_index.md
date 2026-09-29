---
title: "TarArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο αρχειοθέτησης tar."
type: docs
weight: 125
url: /el/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο tar. Χρησιμοποιήστε την για δημιουργία, εξαγωγή ή ενημέρωση αρχείων tar.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [TarArchive()](#TarArchive--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Archive](../../com.aspose.zip/archive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [TarArchive](../../com.aspose.zip/tararchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο. |
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
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων με βάση το δείκτη. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία του αρχείου στον παρεχόμενο κατάλογο. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Εξάγει το παρεχόμενο αρχείο gzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Εξάγει το παρεχόμενο αρχείο gzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Εξάγει το παρεχόμενο αρχείο LZ4 και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Εξάγει το παρεχόμενο αρχείο LZ4 και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Εξάγει το παρεχόμενο αρχείο LZMA και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Εξάγει το παρεχόμενο αρχείο LZMA και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Εξάγει το παρεχόμενο αρχείο lzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Εξάγει το παρεχόμενο αρχείο lzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Εξάγει το παρεχόμενο αρχείο μορφής xz και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Εξάγει το παρεχόμενο αρχείο μορφής xz και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Εξάγει το παρεχόμενο αρχείο μορφής Z και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Εξάγει το παρεχόμενο αρχείο μορφής Z και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Εξάγει το παρεχόμενο αρχείο Zstandard και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Εξάγει το παρεχόμενο αρχείο Zstandard και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα. |
| [getEntries()](#getEntries--) | Λαμβάνει τις καταχωρήσεις τύπου [TarEntry](../../com.aspose.zip/tarentry) που αποτελούν το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει τις καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο tar. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση gzip. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση gzip. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZ4. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZ4. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο διαδρομής με συμπίεση LZ4. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο σε αρχείο διαδρομής με συμπίεση LZ4. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο διαδρομής με συμπίεση lzma. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο σε αρχείο διαδρομής με συμπίεση lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzip. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Z. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Z. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Zstandard. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο στη ροή με συμπίεση Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Zstandard. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Zstandard. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [TarArchive](../../com.aspose.zip/tararchive).

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Δείτε τη μέθοδο [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [TarArchive](../../com.aspose.zip/tararchive) και δημιουργεί μια λίστα καταχωρήσεων που μπορεί να εξαχθεί από το αρχείο.

Το παρακάτω παράδειγμα δείχνει πώς να εξαχθούν όλες οι καταχωρήσεις σε έναν κατάλογο.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

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
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | java.io.File | κατάλογος προς συμπίεση |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | java.lang.String | κατάλογος προς συμπίεση |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Προσθέτει στο αρχείο όλα τα αρχεία και τους καταλόγους αναδρομικά στον δοσμένο κατάλογο.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα του αρχείου που παρέχεται στην παράμετρο `file` δεν επηρεάζει το όνομα της καταχώρησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | το όνομα του στοιχείου |
| file | java.io.File | τα μεταδεδομένα του αρχείου ή του φακέλου που θα συμπιεστεί |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

Το όνομα της καταχώρησης ορίζεται αποκλειστικά μέσα στην παράμετρο `name`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | το όνομα του στοιχείου |
| source | java.io.InputStream | η ροή εισόδου για την καταχώρηση |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

Το όνομα του στοιχείου ορίζεται αποκλειστικά μέσα στην παράμετρο `name`. Το όνομα αρχείου που παρέχεται στην παράμετρο `path` δεν επηρεάζει το όνομα του στοιχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String | το όνομα του στοιχείου |
| path | java.lang.String | διαδρομή προς το αρχείο που θα συμπιεστεί |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Δημιουργεί μια μοναδική καταχώρηση μέσα στο αρχείο.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | η καταχώρηση προς αφαίρεση από τη λίστα καταχωρήσεων |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων με βάση το δείκτη.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Αν ο φάκελος δεν υπάρχει, θα δημιουργηθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | java.lang.String | η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Εξάγει το παρεχόμενο αρχείο gzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: το gzip αρχείο εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Η ροή εξαγωγής GZip δεν είναι αναζητήσιμη λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί με αναζητήσιμη ροή στο παρασκήνιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Εξάγει το παρεχόμενο αρχείο gzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: το gzip αρχείο εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Η ροή εξαγωγής GZip δεν είναι αναζητήσιμη λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί με αναζητήσιμη ροή στο παρασκήνιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Εξάγει το παρεχόμενο αρχείο LZ4 και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: το LZ4 αρχείο εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | source | java.io.InputStream | Η πηγή του αρχείου. |

Η ροή εξαγωγής LZ4 δεν είναι δυνατόν να γίνει αναζήτηση λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Εξάγει το παρεχόμενο αρχείο LZ4 και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: το LZ4 αρχείο εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | path | java.lang.String | Η διαδρομή προς το αρχείο του αρχείου. |

Η ροή εξαγωγής LZ4 δεν είναι δυνατόν να γίνει αναζήτηση λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Εξάγει το παρεχόμενο αρχείο LZMA και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο LZMA εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Η ροή εξαγωγής LZMA δεν είναι δυνατόν να γίνει αναζήτηση λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Εξάγει το παρεχόμενο αρχείο LZMA και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο LZMA εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Η ροή εξαγωγής LZMA δεν είναι δυνατόν να γίνει αναζήτηση λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Εξάγει το παρεχόμενο αρχείο lzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο lzip εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Η ροή εξαγωγής Lzip δεν είναι δυνατόν να γίνει αναζήτηση λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Εξάγει το παρεχόμενο αρχείο lzip και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο lzip εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Η ροή εξαγωγής Lzip δεν είναι δυνατόν να γίνει αναζήτηση λόγω της φύσης του αλγορίθμου συμπίεσης. Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Εξάγει το παρεχόμενο αρχείο μορφής xz και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο xz εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Εξάγει το παρεχόμενο αρχείο μορφής xz και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο xz εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

Το αρχείο Tar παρέχει δυνατότητα εξαγωγής αυθαίρετης εγγραφής, επομένως πρέπει να λειτουργεί σε ροή με δυνατότητα αναζήτησης στο παρασκήνιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Εξάγει το παρεχόμενο αρχείο μορφής Z και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο Z εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Εξάγει το παρεχόμενο αρχείο μορφής Z και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο Z εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Εξάγει το παρεχόμενο αρχείο Zstandard και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο Zstandard εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Εξάγει το παρεχόμενο αρχείο Zstandard και δημιουργεί ένα [TarArchive](../../com.aspose.zip/tararchive) από τα εξαγόμενα δεδομένα.

Σημαντικό: Το αρχείο Zstandard εξάγεται πλήρως μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Λαμβάνει τις καταχωρήσεις τύπου [TarEntry](../../com.aspose.zip/tarentry) που αποτελούν το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - καταχωρίσεις τύπου [TarEntry](../../com.aspose.zip/tarentry) που αποτελούν το αρχείο
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Λαμβάνει τις καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο tar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρίσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο tar
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Αποθηκεύει το αρχείο στη δοθείσα ροή.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(\"myarchive.tar\");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

Είναι δυνατόν να αποθηκεύσετε ένα αρχείο στην ίδια διαδρομή από την οποία φορτώθηκε. Ωστόσο, αυτό δεν συνιστάται επειδή αυτή η προσέγγιση χρησιμοποιεί αντιγραφή σε προσωρινό αρχείο

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip.

```

``````

try (FileOutputStream result = new FileOutputStream(\"result.tar.gz\")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(\"result.tar.gz\");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση LZ4.

```

``````

try (FileOutputStream result = new FileOutputStream(\"result.tar.lz4\")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έξοδος | java.io.OutputStream | Ροή προορισμού. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Αποθηκεύει το αρχείο σε αρχείο διαδρομής με συμπίεση LZ4.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Σημαντικό: το αρχείο tar δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | ροή προορισμού. |

`output` πρέπει να είναι εγγράψιμο |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Αποθηκεύει το αρχείο σε αρχείο διαδρομής με συμπίεση lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Σημαντικό: το αρχείο tar δημιουργείται και στη συνέχεια συμπιέζεται μέσα σε αυτή τη μέθοδο, το περιεχόμενό του διατηρείται εσωτερικά. Προσέξτε την κατανάλωση μνήμης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | σύνολο ρυθμίσεων συγκεκριμένου αρχείου xz: μέγεθος λεξικού, μέγεθος μπλοκ, τύπος ελέγχου |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| έξοδος | java.io.OutputStream | η ροή προορισμού |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Αποθηκεύει το αρχείο στη ροή με συμπίεση Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Αποθηκεύει το αρχείο σε αρχείο με διαδρομή με συμπίεση Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | ορίζει τη μορφή της κεφαλίδας tar. Η τιμή Null θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν |

