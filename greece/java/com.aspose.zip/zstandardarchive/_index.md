---
title: "ZstandardArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Zstandard."
type: docs
weight: 156
url: /el/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Zstandard. Χρησιμοποιήστε την για τη σύνθεση αρχείων Zstandard.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive) προετοιμασμένη για συμπίεση. |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive) προετοιμασμένη για αποσυμπίεση. |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive) προετοιμασμένη για αποσυμπίεση. |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει το αρχείο στη δοθείσα ροή. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει το αρχείο στη διαδρομή. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [getFileEntries()](#getFileEntries--) | Αποκτά καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το zstandard αρχείο. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getName()](#getName--) | Αποκτά το όνομα της καταχώρησης μέσα στο αρχείο. |
| [open()](#open--) | Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου. |
| [save(File destination)](#save-java.io.File-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | Αποθηκεύει το αρχείο στη δοθείσα ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε. |
| [setSource(File file)](#setSource-java.io.File-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(String path)](#setSource-java.lang.String-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive) προετοιμασμένη για συμπίεση.

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε ένα αρχείο.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource("data.bin");
archive.save(\"archive.zst\");
}
 
```



### ZstandardArchive(InputStream sourceStream) {#ZstandardArchive-java.io.InputStream-}
```
public ZstandardArchive(InputStream sourceStream)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [open()](../../com.aspose.zip/zstandardarchive\\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive) προετοιμασμένη για αποσυμπίεση.

Ανοίξτε ένα αρχείο από μια ροή και εξάγετέ το σε ένα `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### ZstandardArchive(String path) {#ZstandardArchive-java.lang.String-}
```
public ZstandardArchive(String path)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class.

Open an archive from file by path and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [open()](../../com.aspose.zip/zstandardarchive\\#open--) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο του αρχείου |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [ZstandardArchive](../../com.aspose.zip/zstandardarchive).

Ανοίξτε ένα αρχείο από αρχείο με διαδρομή και εξάγετέ το σε ένα `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

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

     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή προορισμού. Πρέπει να είναι εγγράψιμη |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει το αρχείο στη διαδρομή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί |

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
|  | destinationDirectory | java.lang.String | η διαδρομή προς το φάκελο όπου θα τοποθετηθούν τα εξαγόμενα αρχεία. |

Εάν ο φάκελος δεν υπάρχει, θα δημιουργηθεί |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Αποκτά καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το zstandard αρχείο.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το zstandard αρχείο
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


Λαμβάνει το μήκος της καταχώρησης σε bytes.

**Returns:**
java.lang.Long - το μήκος της καταχώρησης σε bytes
### getName() {#getName--}
```
public final String getName()
```


Αποκτά το όνομα της καταχώρησης μέσα στο αρχείο.

**Returns:**
java.lang.String - το όνομα της καταχώρησης μέσα στο αρχείο
### open() {#open--}
```
public final InputStream open()
```


Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου.

Εξάγει το αρχείο και αντιγράφει το εξαγόμενο περιεχόμενο σε ροή αρχείου.

```

``````

try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
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

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.zst"));
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.File | το αρχείο που θα ανοίξει ως ροή προορισμού |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.zst"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| outputStream | java.io.OutputStream | η ροή προορισμού |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


Αποθηκεύει το αρχείο στη δοθείσα ροή.

Γράψτε τα συμπιεσμένα δεδομένα στη ροή απόκρισης http.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | the destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.zst");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


Αποθηκεύει το αρχείο στο προορισμένο αρχείο που δόθηκε.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.zst");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| file | java.io.File | η αναφορά σε ένα αρχείο που θα συμπιεστεί |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.zst\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | διαδρομή προς το αρχείο που θα συμπιεστεί |

