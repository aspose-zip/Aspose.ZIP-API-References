---
title: "ArchiveFactory"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο σύμφωνα με τον τύπο του αρχείου."
type: docs
weight: 31
url: /el/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο [IArchive](../../com.aspose.zip/iarchive) σύμφωνα με τον τύπο του αρχείου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | Συμπιέζει τον καθορισμένο κατάλογο σε αρχείο αρχειοθέτησης χρησιμοποιώντας τη δοθείσα μορφή αρχείου. |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο [IArchive](../../com.aspose.zip/iarchive) σύμφωνα με τον τύπο του αρχείου που καθορίζεται από το δεδομένο stream. |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο [IArchive](../../com.aspose.zip/iarchive) σύμφωνα με τον τύπο του κρυπτογραφημένου αρχείου που καθορίζεται από το δεδομένο stream. |
| [getArchive(String path)](#getArchive-java.lang.String-) | Ανιχνεύει τη μορφή του αρχείου και δημιουργεί το κατάλληλο αντικείμενο [IArchive](../../com.aspose.zip/iarchive) σύμφωνα με τον τύπο του αρχείου που καθορίζεται από το δεδομένο μονοπάτι. |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


Συμπιέζει τον καθορισμένο κατάλογο σε αρχείο αρχειοθέτησης χρησιμοποιώντας τη δοθείσα μορφή αρχείου.

Ακολουθεί ένα παράδειγμα για το πώς να χρησιμοποιήσετε τη μέθοδο CompressDirectory:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// Αυτό θα δημιουργήσει ένα αρχείο ZIP με τα περιεχόμενα του καταλόγου στο καθορισμένο μονοπάτι.
 
```

This method will create an archive file at the location specified by the `path` parameter. The name of the archive file will typically be the directory name followed by the appropriate file extension based on the `archiveFormat`. The directory itself is not modified or deleted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the directory that will be compressed |
| outputFileName | java.lang.String | destination file name |
| archiveFormat | [ArchiveFormat](../../com.aspose.zip/archiveformat) | the format of the archive to create (e.g., zip, rar, tar, etc.) |

### getArchive(InputStream stream) {#getArchive-java.io.InputStream-}
```
public static IArchive getArchive(InputStream stream)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(InputStream stream, String password) {#getArchive-java.io.InputStream-java.lang.String-}
```
public static IArchive getArchive(InputStream stream, String password)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of encrypted archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |
| password | java.lang.String | password to decrypt an encrypted archive |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(String path) {#getArchive-java.lang.String-}
```
public static IArchive getArchive(String path)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive to be analyzed |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
