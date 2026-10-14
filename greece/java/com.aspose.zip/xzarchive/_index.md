---
title: "XzArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει το αρχείο xz."
type: docs
weight: 146
url: /el/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει αρχείο συμπιεσμένου xz. Χρησιμοποιήστε την για τη δημιουργία και την εξαγωγή αρχείων xz.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XzArchive()](#XzArchive--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) και δημιουργεί το αρχείο σε μορφή xz. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) και δημιουργεί το αρχείο σε μορφή xz. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Εξάγει το αρχείο xz σε ένα αρχείο. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει το αρχείο xz σε μια ροή. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει το αρχείο xz σε ένα αρχείο με βάση τη διαδρομή. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει καταχωρήσεις του τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο xz. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getName()](#getName--) | Αποκτά το όνομα της καταχώρησης μέσα στο αρχείο. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το ασυμπίεστο μέγεθος των δεδομένων του αρχείου σε byte. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο xz στη δοθείσα ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο xz στο παρεχόμενο αρχείο προορισμού. |
| [setSource(File file)](#setSource-java.io.File-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) και δημιουργεί το αρχείο σε μορφή xz.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) και δημιουργεί το αρχείο σε μορφή xz.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | σύνολο ρυθμίσεων συγκεκριμένου αρχείου xz: μέγεθος λεξικού, μέγεθος μπλοκ, τύπος ελέγχου |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Επιλογές για τη φόρτωση του αρχείου. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | διαδρομή προς την πηγή του αρχείου |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchive](../../com.aspose.zip/xzarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | διαδρομή προς την πηγή του αρχείου |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Εξάγει το αρχείο xz σε ένα αρχείο.

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή για αποθήκευση αποσυμπιεσμένων δεδομένων |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει το αρχείο xz σε ένα αρχείο με βάση τη διαδρομή.

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
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


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


Αποθηκεύει το αρχείο xz στο παρεχόμενο αρχείο προορισμού.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File("data.bin"));
archive.save(\"result.xz\");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| file | java.io.File | αρχείο, το οποίο θα ανοίξει ως ροή εισόδου |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourcePath | java.lang.String | διαδρομή προς το αρχείο που θα ανοίξει ως ροή εισόδου |

