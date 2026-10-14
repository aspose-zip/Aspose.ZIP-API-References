---
title: "TarEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο tar."
type: docs
weight: 126
url: /el/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο tar.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getModificationTime()](#getModificationTime--) | Λαμβάνει την ώρα τροποποίησης του αρχείου ή του φακέλου. |
| [getName()](#getName--) | Λαμβάνει το όνομα της καταχώρησης στο αρχείο. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το μέγεθος ενός αρχικού αρχείου. |
| [isDirectory()](#isDirectory--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [open()](#open--) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης. |
| [setName(String value)](#setName-java.lang.String-) | Ορίζει το όνομα της καταχώρησης μέσα στο αρχείο. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

Εξάγει μια καταχώρηση από το tar αρχείο.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί |

**Returns:**
java.io.File - οι πληροφορίες του αρχείου που εξήχθη.
### getLength() {#getLength--}
```
public final Long getLength()
```


Λαμβάνει το μήκος της καταχώρησης σε bytes.

**Returns:**
java.lang.Long - το μήκος της καταχώρησης σε bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Λαμβάνει την ώρα τροποποίησης του αρχείου ή του φακέλου.

**Returns:**
java.util.Date - η ώρα τροποποίησης του αρχείου ή του καταλόγου.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα της καταχώρησης στο αρχείο.

**Returns:**
java.lang.String - το όνομα της καταχώρησης στο αρχείο
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Λαμβάνει το μέγεθος ενός αρχικού αρχείου.

Έχει την ίδια τιμή με `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - το μέγεθος ενός αρχικού αρχείου.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν η καταχώρηση αντιπροσωπεύει κατάλογο
### open() {#open--}
```
public final InputStream open()
```


Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης.


Χρήση:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

