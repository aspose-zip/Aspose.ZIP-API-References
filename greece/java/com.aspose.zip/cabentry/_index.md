---
title: "CabEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο cab."
type: docs
weight: 46
url: /el/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο cab.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [getModificationTime()](#getModificationTime--) | Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [getName()](#getName--) | Λαμβάνει το όνομα της καταχώρησης στο αρχείο. |
| [open()](#open--) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης. |
| [toString()](#toString--) | Επιστρέφει την αναπαράσταση ως συμβολοσειρά του αντικειμένου της κλάσης [CabEntry](../../com.aspose.zip/cabentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

Εξάγετε μια καταχώρηση από το αρχείο CAB.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί |

**Returns:**
java.io.File - οι πληροφορίες αρχείου ενός συντιθέμενου αρχείου
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


Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης.

**Returns:**
java.util.Date - η ημερομηνία και ώρα τελευταίας τροποποίησης.
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα της καταχώρησης στο αρχείο.

**Returns:**
java.lang.String - το όνομα της καταχώρησης στο αρχείο
### open() {#open--}
```
public final InputStream open()
```


Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης.

Χρήση:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
