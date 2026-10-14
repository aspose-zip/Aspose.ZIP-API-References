---
title: "RarArchiveEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αναπαριστά ένα μοναδικό αρχείο μέσα σε ένα αρχείο."
type: docs
weight: 98
url: /el/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Αναπαριστά ένα μοναδικό αρχείο μέσα σε ένα αρχείο.

Μετατρέψτε μια παρουσία του [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) σε [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) για να προσδιορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getCompressedSize()](#getCompressedSize--) | Λαμβάνει το μέγεθος του συμπιεσμένου αρχείου. |
| [getCreationTime()](#getCreationTime--) | Λαμβάνει την ημερομηνία και ώρα δημιουργίας. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Λαμβάνει ένα γεγονός που ενεργοποιείται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής. |
| [getLastAccessTime()](#getLastAccessTime--) | Λαμβάνει την ημερομηνία και ώρα τελευταίας πρόσβασης. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος. |
| [getModificationTime()](#getModificationTime--) | Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [getName()](#getName--) | Λαμβάνει το όνομα της καταχώρησης στο αρχείο. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το μέγεθος του αρχικού αρχείου. |
| [isDirectory()](#isDirectory--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [open()](#open--) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο της καταχώρησης. |
| [open(String password)](#open-java.lang.String-) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο της καταχώρησης. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα γεγονός που ενεργοποιείται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.


Αποσυμπιέζει μια καταχώρηση του rar αρχείου με κωδικό πρόσβασης.

```

``````

try (FileInputStream rarFile = new FileInputStream(\"archive.rar\")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | Ροή προορισμού. Πρέπει να είναι εγγράψιμη. |
| password | java.lang.String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται.


Αποσυμπιέζει δύο καταχωρήσεις του rar αρχείου.

```

``````

try (FileInputStream rarFile = new FileInputStream(\"archive.rar\")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(\"first.bin\", \"pass\");
archive.getEntries().get(1).extract(\"second.bin\", \"pass\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | Η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί. |
| password | java.lang.String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. |

**Returns:**
java.io.File - οι πληροφορίες του αρχείου που εξήχθη.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Λαμβάνει το μέγεθος του συμπιεσμένου αρχείου.

**Returns:**
long - το μέγεθος του συμπιεσμένου αρχείου
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Λαμβάνει την ημερομηνία και ώρα δημιουργίας.

**Returns:**
java.util.Date - ημερομηνία και ώρα δημιουργίας.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Λαμβάνει ένα γεγονός που ενεργοποιείται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
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


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο του αρχείου. Δείτε την ενότητα παραδειγμάτων.

**Returns:**
java.io.InputStream - Η ροή που αντιπροσωπεύει το περιεχόμενο της καταχώρησης.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο της καταχώρησης.


Χρήση:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Ο αποστολέας Event είναι μια παρουσία του [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής έχει εξαχθεί. |

