---
title: "ZArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αυτή η κλάση αντιπροσωπεύει ένα αρχείο συμπιεσμένου Z."
type: docs
weight: 153
url: /el/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο Z (compress) archive. Χρησιμοποιήστε την για σύνθεση ή εξαγωγή αρχείων Z.

Δείτε [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ZArchive()](#ZArchive--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για συμπίεση. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Εξάγει το Z archive σε ένα αρχείο. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει το Z archive σε ένα ρεύμα. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει το Z archive σε αρχείο με βάση τη διαδρομή. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει το περιεχόμενο του αρχείου στον παρεχόμενο φάκελο. |
| [getFileEntries()](#getFileEntries--) | Αποκτά καταχωρήσεις τύπου [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) που αποτελούν το Z archive. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getName()](#getName--) | Αποκτά το όνομα της καταχώρησης μέσα στο αρχείο. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει το Z archive στο παρεχόμενο ρεύμα. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Αποθηκεύει το Z archive στο παρεχόμενο ρεύμα. |
| [save(String destinationFileName)](#save-java.lang.String-) | Αποθηκεύει το αρχείο Z στην προδιαγεγραμμένη αρχική τοποθεσία. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Αποθηκεύει το αρχείο Z στην προδιαγεγραμμένη αρχική τοποθεσία. |
| [setSource(File file)](#setSource-java.io.File-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για συμπίεση.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| source | java.io.InputStream | η πηγή του αρχείου |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | οι επιλογές για τη φόρτωση του αρχείου |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς την πηγή του αρχείου |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ZArchive](../../com.aspose.zip/zarchive) προετοιμασμένη για αποσυμπίεση.

Αυτός ο κατασκευαστής δεν αποσυμπιέζει. Δείτε τη μέθοδο [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) για αποσυμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς την πηγή του αρχείου |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | οι επιλογές για τη φόρτωση του αρχείου |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Εξάγει το Z archive σε ένα αρχείο.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
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


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


Εξάγει το Z archive σε αρχείο με βάση τη διαδρομή.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

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
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έξοδος | java.io.OutputStream | η ροή προορισμού |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Αποθηκεύει το Z archive στο παρεχόμενο ρεύμα.

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationFileName | java.lang.String | η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου δείχνει σε υπάρχον αρχείο, θα αντικατασταθεί. |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Αποθηκεύει το αρχείο Z στην προδιαγεγραμμένη αρχική τοποθεσία.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File("data.bin"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| file | java.io.File | η πληροφορία του αρχείου που θα ανοίξει ως ροή εισόδου |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ορίζει το περιεχόμενο που θα συμπιεστεί μέσα στο αρχείο.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourcePath | java.lang.String | η διαδρομή προς το αρχείο που θα ανοίξει ως ροή εισόδου |

