---
title: "Lz4Archive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LZ4."
type: docs
weight: 80
url: /el/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει αρχείο συμπιεσμένου LZ4. Χρησιμοποιήστε την για εξαγωγή ή δημιουργία αρχείων LZ4.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive) προετοιμασμένη για αποσυμπίεση. |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive) προετοιμασμένη για αποσυμπίεση. |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive()](#Lz4Archive--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive) προετοιμασμένη για συμπίεση. |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive) προετοιμασμένη για συμπίεση. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει το αρχείο στη δοθείσα ροή. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει το αρχείο στη διαδρομή. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος. |
| [getName()](#getName--) | Λαμβάνει το αρχικό όνομα. |
| [open()](#open--) | Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου. |
| [save(File destination)](#save-java.io.File-) | Αποθηκεύει το αρχείο lz4 στο προσαρτημένο αρχείο προορισμού. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο lz4 στη ροή που παρέχεται. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(File fileInfo)](#setSource-java.io.File-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(String path)](#setSource-java.lang.String-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive) προετοιμασμένη για αποσυμπίεση.

Ανοίξτε ένα αρχείο από ροή και εξάγετέ το σε ένα `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [open()](../../com.aspose.zip/lz4archive\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Οι επιλογές για τη φόρτωση του αρχείου. |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive).

Ανοίξτε ένα αρχείο από το αρχείο με τη διαδρομή και εξάγετε το σε ένα `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [open()](../../com.aspose.zip/lz4archive\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Οι επιλογές για τη φόρτωση του αρχείου. |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive) προετοιμασμένη για συμπίεση.

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [Lz4Archive](../../com.aspose.zip/lz4archive) προετοιμασμένη για συμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | Η ρύθμιση του συντιθέμενου αρχείου. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει το αρχείο στη δοθείσα ροή.

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο ενός αρχείου. Δείτε την ενότητα παραδειγμάτων.

**Returns:**
java.io.InputStream - η ροή που αντιπροσωπεύει το περιεχόμενο του αρχείου.
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Αποθηκεύει το αρχείο lz4 στο προσαρτημένο αρχείο προορισμού.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lz4"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έξοδος | java.io.OutputStream | Ροή προορισμού. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource("data.bin");
archive.save("archive.lz4");
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
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

Χρησιμοποιήστε αυτή τη μέθοδο για να δημιουργήσετε ένα συνδυασμένο αρχείο tar.lz4.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Αρχείο Tar που θα συμπιεστεί. |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileInfo | java.io.File | Η αναφορά σε ένα αρχείο που θα συμπιεστεί. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.lz4");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Διαδρομή προς το αρχείο που θα συμπιεστεί. |

