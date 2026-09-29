---
title: "GzipArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο gzip."
type: docs
weight: 69
url: /el/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο gzip. Χρησιμοποιήστε την για τη δημιουργία ή την εξαγωγή gzip αρχείων.

Ο αλγόριθμος συμπίεσης Gzip βασίζεται στον αλγόριθμο DEFLATE, ο οποίος είναι ένας συνδυασμός των LZ77 και της κωδικοποίησης Huffman.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για συμπίεση. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για αποσυμπίεση. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για αποσυμπίεση. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για αποσυμπίεση. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για αποσυμπίεση. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive). |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει το αρχείο στη δοθείσα ροή. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει το αρχείο στη διαδρομή. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το gzip αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μέγεθος ενός αρχικού αρχείου. |
| [getName()](#getName--) | Το όνομα του αρχικού αρχείου. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το μέγεθος ενός αρχικού αρχείου. |
| [open()](#open--) | Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(File file)](#setSource-java.io.File-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(String path)](#setSource-java.lang.String-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για συμπίεση.

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [open()](../../com.aspose.zip/gziparchive\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Η πηγή του αρχείου. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για αποσυμπίεση.

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [open()](../../com.aspose.zip/gziparchive\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Η πηγή του αρχείου. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Επιλογές για τη φόρτωση του αρχείου. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive) προετοιμασμένη για αποσυμπίεση.

Ανοίξτε ένα αρχείο από το αρχείο με τη διαδρομή και εξάγετε το σε ένα `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [open()](../../com.aspose.zip/gziparchive\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η διαδρομή προς το αρχείο του αρχείου. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [GzipArchive](../../com.aspose.zip/gziparchive).

Ανοίξτε ένα αρχείο από το αρχείο με τη διαδρομή και εξάγετε το σε ένα `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | Ροή προορισμού. Πρέπει να είναι εγγράψιμη. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει το αρχείο στη διαδρομή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |

**Returns:**
java.io.File - οι πληροφορίες του αρχείου που εξήχθη.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | Η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

Αν ο φάκελος δεν υπάρχει, θα δημιουργηθεί. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το gzip αρχείο.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις του τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το gzip αρχείο.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Λαμβάνει το μέγεθος ενός αρχικού αρχείου.

Κατά την αποσυμπίεση, αυτή η ιδιότητα μπορεί να περιέχει λανθασμένο μέγεθος. Εάν το μέγεθος του αποσυμπιεσμένου αρχείου υπερβαίνει τα 4GB, αυτή η ιδιότητα θα δώσει λανθασμένη τιμή λόγω του 32-bit ορίου στην κεφαλίδα.

**Returns:**
java.lang.Long - μέγεθος ενός αρχικού αρχείου
### getName() {#getName--}
```
public final String getName()
```


Το όνομα του αρχικού αρχείου.

**Returns:**
java.lang.String - το όνομα του αρχικού αρχείου
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Λαμβάνει το μέγεθος ενός αρχικού αρχείου.

Κατά την αποσυμπίεση, αυτή η ιδιότητα μπορεί να περιέχει λανθασμένο μέγεθος. Εάν το μέγεθος του αποσυμπιεσμένου αρχείου υπερβαίνει τα 4GB, αυτή η ιδιότητα θα δώσει λανθασμένη τιμή λόγω του 32-bit ορίου στην κεφαλίδα.

**Returns:**
long - μέγεθος ενός αρχικού αρχείου.
### open() {#open--}
```
public final InputStream open()
```


Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου.

Εξάγει το αρχείο και αντιγράφει το εξαγόμενο περιεχόμενο σε ροή αρχείου.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Ροή προορισμού. |

`outputStream` πρέπει να είναι εγγράψιμο. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Χρησιμοποιήστε αυτή τη μέθοδο για να δημιουργήσετε ένα ενιαίο αρχείο tar.gz.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Αρχείο Tar που θα συμπιεστεί. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | Η ροή εισόδου για το αρχείο. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

Ανοίξτε ένα αρχείο από το αρχείο με τη διαδρομή και εξάγετε το σε ένα `MemoryStream`

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

