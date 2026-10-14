---
title: "LzipArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Lzip."
type: docs
weight: 83
url: /el/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Lzip. Χρησιμοποιήστε την για να δημιουργήσετε ή να εξάγετε αρχεία Lzip.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | Αρχικοποιεί μια νέα παρουσία του [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | Αρχικοποιεί μια νέα παρουσία του [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzipArchive](../../com.aspose.zip/lziparchive) προετοιμασμένη για αποσυμπίεση. |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzipArchive](../../com.aspose.zip/lziparchive) προετοιμασμένη για αποσυμπίεση. |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzipArchive](../../com.aspose.zip/lziparchive) προετοιμασμένη για αποσυμπίεση. |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [LzipArchive](../../com.aspose.zip/lziparchive) προετοιμασμένη για αποσυμπίεση. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Αποσυμπιέζει το αρχείο lzip σε αρχείο. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Αποσυμπιέζει το αρχείο lzip σε ροή. |
| [extract(String path)](#extract-java.lang.String-) | Αποσυμπιέζει το αρχείο lzip σε αρχείο με διαδρομή. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [getFileEntries()](#getFileEntries--) | Λαμβάνει τις καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το αρχείο lzip. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος. |
| [getName()](#getName--) | Το όνομα του αρχικού αρχείου. |
| [getSettings()](#getSettings--) | Λαμβάνει τη ρύθμιση του συγκεκριμένου αρχείου lzip. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το ασυμπίεστο μέγεθος των δεδομένων του αρχείου σε byte. |
| [save(File destination)](#save-java.io.File-) | Αποθηκεύει το αρχείο lzip στο προσαρτημένο αρχείο προορισμού. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Αποθηκεύει το αρχείο lzip στην παρεχόμενη ροή. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο lzip στο προσαρτημένο αρχείο προορισμού. |
| [setSource(File file)](#setSource-java.io.File-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(String path)](#setSource-java.lang.String-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


Αρχικοποιεί μια νέα παρουσία του [LzipArchive](../../com.aspose.zip/lziparchive).

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


Αρχικοποιεί μια νέα παρουσία του [LzipArchive](../../com.aspose.zip/lziparchive).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | η ρύθμιση του συγκεκριμένου αρχείου lzip με ορισμό του μεγέθους λεξικού |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzipArchive](../../com.aspose.zip/lziparchive) προετοιμασμένη για αποσυμπίεση.

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | java.io.InputStream | η πηγή του αρχείου |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Επιλογές για τη φόρτωση του αρχείου. |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [LzipArchive](../../com.aspose.zip/lziparchive) προετοιμασμένη για αποσυμπίεση.

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς την πηγή του αρχείου |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Επιλογές για τη φόρτωση του αρχείου. |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Αποσυμπιέζει το αρχείο lzip σε αρχείο.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | η ροή για την αποθήκευση αποσυμπιεσμένων δεδομένων |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Αποσυμπιέζει το αρχείο lzip σε αρχείο με διαδρομή.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
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


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.File | το αρχείο, το οποίο θα ανοιχτεί ως ροή προορισμού |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Αποθηκεύει το αρχείο lzip στην παρεχόμενη ροή.

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File("data.bin"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η ροή εισόδου για το αρχείο |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

