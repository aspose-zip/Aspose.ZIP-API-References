---
title: "SevenZipArchiveEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μόνο αρχείο μέσα σε αρχείο 7z."
type: docs
weight: 105
url: /el/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Αντιπροσωπεύει ένα μόνο αρχείο μέσα σε αρχείο 7z.

Μετατρέψτε μια παρουσία του [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) σε [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) για να καθορίσετε εάν η καταχώρηση είναι κρυπτογραφημένη ή όχι.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| [extract(String path)](#extract-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται. |
| [getCompressedSize()](#getCompressedSize--) | Λαμβάνει το μέγεθος του συμπιεσμένου αρχείου. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
| [getCompressionSettings()](#getCompressionSettings--) | Αποκτά τις ρυθμίσεις για συμπίεση ή αποσυμπίεση. |
| [getLength()](#getLength--) | Λαμβάνει το μήκος. |
| [getModificationTime()](#getModificationTime--) | Λαμβάνει την ημερομηνία και ώρα τελευταίας τροποποίησης. |
| [getName()](#getName--) | Λαμβάνει το όνομα της καταχώρησης στο αρχείο. |
| [getUncompressedSize()](#getUncompressedSize--) | Λαμβάνει το μέγεθος του αρχικού αρχείου. |
| [isDirectory()](#isDirectory--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [open()](#open--) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης. |
| [open(String password)](#open-java.lang.String-) | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν ένα τμήμα της ακατέργαστης ροής συμπιέζεται. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Εξάγει την καταχώρηση στη ροή που παρέχεται.

Εξάγει μια καταχώρηση του zip αρχείου με κωδικό πρόσβασης.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| προορισμός | java.io.OutputStream | ροή προορισμού. Πρέπει να είναι εγγράψιμη |
| password | java.lang.String | προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Εξάγει την καταχώρηση στο σύστημα αρχείων με τη διαδρομή που παρέχεται.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract("data.bin");
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

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | java.lang.String | η διαδρομή προς το αρχείο προορισμού. Εάν το αρχείο υπάρχει ήδη, θα αντικατασταθεί |
| password | java.lang.String | προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση |

**Returns:**
java.io.File - οι πληροφορίες του αρχείου που εξήχθη.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Λαμβάνει το μέγεθος του συμπιεσμένου αρχείου.

**Returns:**
long - το μέγεθος του συμπιεσμένου αρχείου
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

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
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


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
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

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο του αρχείου. Δείτε την ενότητα παραδειγμάτων.

**Returns:**
java.io.InputStream - η ροή που αντιπροσωπεύει το περιεχόμενο της καταχώρησης.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το περιεχόμενο της καταχώρησης.

Χρήση:

```

``````

SevenZipArchive archive = new SevenZipArchive("archive.7z");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
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

Αποστολέας συμβάντος είναι ένα αντικείμενο τύπου [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry).

Δεν καλείται σε λειτουργία solid και σε πολυνηματική λειτουργία για καταχωρήσεις LZMA2.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | ένα συμβάν που ενεργοποιείται όταν συμπιέζεται ένα τμήμα της ακατέργαστης ροής |

