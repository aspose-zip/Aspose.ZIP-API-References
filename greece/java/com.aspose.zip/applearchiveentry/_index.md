---
title: "AppleArchiveEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει μια καταχώρηση αρχείου ή καταλόγου μέσα σε ένα ."
type: docs
weight: 17
url: /el/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει μια καταχώρηση αρχείου ή καταλόγου μέσα σε ένα [AppleArchive](../../com.aspose.zip/applearchive).

Μια παρουσία αυτής της κλάσης μπορεί να αντιπροσωπεύει είτε μια καταχώρηση που έχει αναλυθεί από ένα υπάρχον Apple Archive είτε μια καταχώρηση που προστέθηκε σε ένα αρχείο που δημιουργείται.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση Apple archive σε σύστημα αρχείων με βάση τη διαδρομή. |
| [getLength()](#getLength--) | Αποκτά το μη συμπιεσμένο μήκος της καταχώρησης σε byte. |
| [getName()](#getName--) | Αποκτά τη διαδρομή της καταχώρησης μέσα στο αρχείο. |
| [isDirectory()](#isDirectory--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [open()](#open--) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα (stream) με το περιεχόμενο της καταχώρησης. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή προορισμού. Πρέπει να είναι εγγράψιμη |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει την καταχώρηση Apple archive σε σύστημα αρχείων με βάση τη διαδρομή.

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
