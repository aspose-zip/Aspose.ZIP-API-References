---
title: "ArjEntryPlain"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο ARJ."
type: docs
weight: 38
url: /el/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο ARJ.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Εξάγει την καταχώρηση του αρχείου ARJ σε ένα αρχείο. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getCompressedSize()](#getCompressedSize--) | Λαμβάνει το μέγεθος του συμπιεσμένου αρχείου. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getName()](#getName--) | Λαμβάνει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το μέγεθος του αρχικού αρχείου. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Εξάγει την καταχώρηση του αρχείου ARJ σε ένα αρχείο.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί |

**Returns:**
java.io.File - οι πληροφορίες αρχείου του σύνθετου αρχείου
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Λαμβάνει το μέγεθος του συμπιεσμένου αρχείου.

**Returns:**
long - το μέγεθος του συμπιεσμένου αρχείου
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


Λαμβάνει το όνομα της καταχώρησης μέσα στο αρχείο.

**Returns:**
java.lang.String - όνομα της καταχώρησης εντός του αρχείου
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Λαμβάνει το μέγεθος του αρχικού αρχείου.

**Returns:**
long - μέγεθος του αρχικού αρχείου
