---
title: "LzmaArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LZMA."
type: docs
weight: 86
url: /el/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο συμπιεσμένου LZMA. Χρησιμοποιήστε την για τη δημιουργία ή την εξαγωγή αρχείων LZMA.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) και δημιουργεί το αρχείο σε μορφή lzma. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) και δημιουργεί το αρχείο σε μορφή lzma. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) προετοιμασμένη για αποσυμπίεση. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) προετοιμασμένη για αποσυμπίεση. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Εξάγει το αρχείο lzma σε ένα αρχείο. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει το αρχείο lzma σε μια ροή. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει το αρχείο lzma σε αρχείο με βάση τη διαδρομή. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο lzma. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος. |
| [getName()](#getName--) | Το όνομα του αρχικού αρχείου. |
| [save(File destination)](#save-java.io.File-) | Αποθηκεύει το αρχείο lzma στο παρεχόμενο αρχείο προορισμού. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο lzma στη ροή που παρέχεται. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο lzma στο παρεχόμενο αρχείο προορισμού. |
| [setSource(File file)](#setSource-java.io.File-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) και δημιουργεί το αρχείο σε μορφή lzma.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) και δημιουργεί το αρχείο σε μορφή lzma.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | σύνολο ρυθμίσεων συγκεκριμένου αρχείου lzma |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzmaArchive](../../com.aspose.zip/lzmaarchive) προετοιμασμένη για αποσυμπίεση.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| file | java.io.File | το αρχείο για την αποθήκευση αποσυμπιεσμένων δεδομένων |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει το αρχείο lzma σε μια ροή.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο που θα αποθηκεύσει τα αποσυμπιεσμένα δεδομένα |

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


Λαμβάνει καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο lzma.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο lzma.
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


Λαμβάνει το μήκος.

**Returns:**
java.lang.Long - μήκος
### getName() {#getName--}
```
public final String getName()
```


Το όνομα του αρχικού αρχείου.

**Returns:**
java.lang.String - το όνομα του αρχικού αρχείου
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Αποθηκεύει το αρχείο lzma στο παρεχόμενο αρχείο προορισμού.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lzma"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έξοδος | java.io.OutputStream | ροή προορισμού |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Αποθηκεύει το αρχείο lzma στο παρεχόμενο αρχείο προορισμού.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| file | java.io.File | το αρχείο, το οποίο θα ανοίξει ως ροή εισόδου |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourcePath | java.lang.String | διαδρομή προς το αρχείο, το οποίο θα ανοιχτεί ως ροή εισόδου |

