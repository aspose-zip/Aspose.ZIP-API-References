---
title: "LzxArchiveEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μοναδικό αρχείο μέσα σε αρχείο LZX."
type: docs
weight: 90
url: /el/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει ένα μοναδικό αρχείο μέσα σε αρχείο LZX.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση αρχείου Lzx σε σύστημα αρχείων με βάση τη διαδρομή. |
| [getCommentary()](#getCommentary--) | Λαμβάνει το σχόλιο. |
| [getCompressedSize()](#getCompressedSize--) | Αποκτά το μέγεθος του συμπιεσμένου αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getModificationTime()](#getModificationTime--) | Αποκτά την ώρα τελευταίας τροποποίησης της καταχώρησης. |
| [getName()](#getName--) | Λαμβάνει το όνομα του στοιχείου. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το μέγεθος του αρχικού αρχείου. |
| [isDirectory()](#isDirectory--) | Αποκτά μια τιμή που υποδεικνύει εάν αυτή η καταχώρηση είναι κατάλογος. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | Ροή προορισμού. Πρέπει να είναι εγγράψιμη. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει την καταχώρηση αρχείου Lzx σε σύστημα αρχείων με βάση τη διαδρομή.

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
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
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
