---
title: "ArchiveEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αναπαριστά ένα μοναδικό αρχείο μέσα σε ένα αρχείο."
type: docs
weight: 27
url: /el/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Αναπαριστά ένα μοναδικό αρχείο μέσα σε ένα αρχείο.

Μετατρέψτε μια παρουσία του [ArchiveEntry](../../com.aspose.zip/archiveentry) σε [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) για να προσδιορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getComment()](#getComment--) | Αποκτά το σχόλιο της καταχώρησης μέσα στο αρχείο. |
| [getCompressedSize()](#getCompressedSize--) | Αποκτά το μέγεθος του συμπιεσμένου αρχείου. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [getCompressionSettings()](#getCompressionSettings--) | Αποκτά τις ρυθμίσεις για συμπίεση ή αποσυμπίεση. |
| [getDataSource()](#getDataSource--) | Πηγή για την καταχώρηση εάν η καταχώρηση προστέθηκε στο αρχείο, χωρίς εξαγωγή. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Λαμβάνει ένα γεγονός που ενεργοποιείται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος. |
| [getModificationTime()](#getModificationTime--) | Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [getName()](#getName--) | Λαμβάνει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το μέγεθος του αρχικού αρχείου. |
| [isDirectory()](#isDirectory--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [open()](#open--) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο της καταχώρησης. |
| [open(String password)](#open-java.lang.String-) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με αποσυμπιεσμένο περιεχόμενο της καταχώρησης. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Ορίζει ένα γεγονός που ενεργοποιείται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Ορίζει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

Εξάγει μια καταχώρηση του zip αρχείου με κωδικό πρόσβασης.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
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

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
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

Εξάγετε δύο καταχωρήσεις του αρχείου ZIP, η καθεμία με τον δικό της κωδικό πρόσβασης

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
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
### getComment() {#getComment--}
```
public final String getComment()
```


Αποκτά το σχόλιο της καταχώρησης μέσα στο αρχείο.

**Returns:**
java.lang.String - σχόλιο της καταχώρησης μέσα στο αρχείο
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Αποκτά το μέγεθος του συμπιεσμένου αρχείου.

**Returns:**
long - μέγεθος του συμπιεσμένου αρχείου
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Σε αυτό το παράδειγμα, ο διαχειριστής συμβάντων χρησιμοποιείται για ακύρωση μετά την εξαγωγή των πρώτων εκατό MB της καταχώρησης.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
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

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο του αρχείου.

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
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

Ο αποστολέας του συμβάντος είναι ένα αντικείμενο [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ένα συμβάν που ενεργοποιείται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Ορίζει ένα γεγονός που ενεργοποιείται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής.

Σε αυτό το παράδειγμα, ο διαχειριστής συμβάντων χρησιμοποιείται για τον υπολογισμό του ποσοστού του επεξεργασμένου μεγέθους σε ποσοστά.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Ο αποστολέας του συμβάντος είναι ένα αντικείμενο [ArchiveEntry](../../com.aspose.zip/archiveentry). Είναι δυνατόν να ακυρωθεί η εξαγωγή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής έχει εξαχθεί. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Ορίζει την ημερομηνία και ώρα τελευταίας τροποποίησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.util.Date | τελευταία τροποποιημένη ημερομηνία και ώρα |

