---
title: "WimFileEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο wim."
type: docs
weight: 133
url: /el/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει ένα μεμονωμένο αρχείο μέσα σε αρχείο wim.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος της καταχώρησης σε bytes. |
| [open()](#open--) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

Εξάγετε μια καταχώρηση του αρχείου wim.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract(httpResponseStream);
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

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract("data.bin");
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
### open() {#open--}
```
public final InputStream open()
```


Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης.

Χρήση:

```

``````

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
