---
title: "ArchiveLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές με τις οποίες το αρχείο ZIP φορτώνεται από ένα συμπιεσμένο αρχείο."
type: docs
weight: 35
url: /el/java/com.aspose.zip/archiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveLoadOptions
```

Επιλογές με τις οποίες το αρχείο ZIP φορτώνεται από ένα συμπιεσμένο αρχείο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ArchiveLoadOptions()](#ArchiveLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Λαμβάνει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων. |
| [getEncoding()](#getEncoding--) | Λαμβάνει την κωδικοποίηση για τα ονόματα των καταχωρίσεων. |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes. |
| [getEntryListed()](#getEntryListed--) | Λαμβάνει ένα συμβάν που ενεργοποιείται όταν μια καταχώριση εμφανίζεται στον πίνακα περιεχομένων. |
| [getForwardOnly()](#getForwardOnly--) | Λαμβάνει τη σημαία που υποδεικνύει ότι το αρχείο εξάγεται από ροή μόνο για ανάγνωση. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Λαμβάνει μια τιμή που υποδεικνύει αν η επαλήθευση του checksum των καταχωρίσεων ZIP θα παραλειφθεί και η ασυμφωνία θα αγνοηθεί. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ορίζει την κωδικοποίηση για τα ονόματα των καταχωρίσεων. |
| [setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes. |
| [setEntryListed(Event&lt;EntryEventArgs&gt; value)](#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | Ορίζει ένα συμβάν που ενεργοποιείται όταν μια καταχώριση εμφανίζεται στον πίνακα περιεχομένων. |
| [setForwardOnly(boolean value)](#setForwardOnly-boolean-) | Ορίζει τη σημαία που υποδεικνύει ότι το αρχείο εξάγεται από ροή μόνο για ανάγνωση. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν η επαλήθευση του checksum των καταχωρίσεων ZIP θα παραλειφθεί και η ασυμφωνία θα αγνοηθεί. |
### ArchiveLoadOptions() {#ArchiveLoadOptions--}
```
public ArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Λαμβάνει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων.


Μπορείτε να παρέχετε τον κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή του αρχείου.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.zip")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets the encoding for entries' names.


Entry name composed using specified encoding regardless of zip file properties.

```

``````

    try (FileInputStream fs = new FileInputStream("archive.zip")) {
        ArchiveLoadOptions options = new ArchiveLoadOptions();
        options.setEncoding(Charset.forName("MS932"));
        try (Archive archive = new Archive(fs, options)) {
            String name = archive.getEntries().get(0).getName();
        }
    } catch (IOException ex) {
    }
 
```



**Returns:**
java.nio.charset.Charset - η κωδικοποίηση για τα ονόματα των καταχωρήσεων
### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getEntryExtractionProgressed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes.

Παρακολουθήστε την πρόοδο της εξαγωγής μιας καταχώρησης.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive("archive.zip", options);
 
```

Cancel an entry extraction after a certain time.

```

``````

     long startTime = System.nanoTime();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setEntryExtractionProgressed((s, e) -> {
         if ((System.nanoTime() - startTime) / 1_000_000 > 1000)
             e.setCancel(true);
     });
     try (Archive a = new Archive("big.zip", options)) {
         a.getEntries().get(0).extract("first.bin");
     }
 
```

Ο αποστολέας του συμβάντος είναι το αντικείμενο [ArchiveEntry](../../com.aspose.zip/archiveentry) του οποίου η εξαγωγή προχωρά.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### getEntryListed() {#getEntryListed--}
```
public final Event<EntryEventArgs> getEntryListed()
```


Λαμβάνει ένα συμβάν που ενεργοποιείται όταν μια καταχώριση εμφανίζεται στον πίνακα περιεχομένων.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive("archive.zip", options);
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when an entry listed within table of content
### getForwardOnly() {#getForwardOnly--}
```
public final boolean getForwardOnly()
```


Gets the flag that indicating that archive is extracted from read-only stream.

**Returns:**
boolean - true, if archive's stream is rean-only, false elsewhere.
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public final boolean getSkipChecksumVerification()
```


Gets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. Default is false.

**Returns:**
boolean - a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ZIP archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (Archive a = new Archive("big.zip", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

Η ακύρωση συνήθως οδηγεί σε μη εξαγόμενα κάποια δεδομένα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public final void setDecryptionPassword(String value)
```


Ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων.


Μπορείτε να παρέχετε τον κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή του αρχείου.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.zip")) {
try (FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets the encoding for entries' names.


Entry name composed using specified encoding regardless of zip file properties.

```

``````

    try (FileInputStream fs = new FileInputStream("archive.zip")) {
        ArchiveLoadOptions options = new ArchiveLoadOptions();
        options.setEncoding(Charset.forName("MS932"));
        try (Archive archive = new Archive(fs, options)) {
            String name = archive.getEntries().get(0).getName();
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.nio.charset.Charset | η κωδικοποίηση για τα ονόματα των καταχωρήσεων |

### setEntryExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί κάποια bytes.

Παρακολουθήστε την πρόοδο της εξαγωγής μιας καταχώρησης.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
Archive archive = new Archive("archive.zip", options);
 
```

Cancel an entry extraction after a certain time.

```

``````

     long startTime = System.nanoTime();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setEntryExtractionProgressed((s, e) -> {
         if ((System.nanoTime() - startTime) / 1_000_000 > 1000)
             e.setCancel(true);
     });
     try (Archive a = new Archive("big.zip", options)) {
         a.getEntries().get(0).extract("first.bin");
     }
 
```

Ο αποστολέας του συμβάντος είναι το αντικείμενο [ArchiveEntry](../../com.aspose.zip/archiveentry) του οποίου η εξαγωγή προχωρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | ένα συμβάν που ενεργοποιείται όταν έχουν εξαχθεί ορισμένα byte |

### setEntryListed(Event&lt;EntryEventArgs&gt; value) {#setEntryListed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public final void setEntryListed(Event<EntryEventArgs> value)
```


Ορίζει ένα συμβάν που ενεργοποιείται όταν μια καταχώριση εμφανίζεται στον πίνακα περιεχομένων.

```

``````

ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setEntryListed(new Event<EntryEventArgs>() {
public void invoke(Object sender, EntryEventArgs entryEventArgs) {
System.out.println(entryEventArgs.getEntry().getName());
}
});
Archive archive = new Archive("archive.zip", options);
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | an event that is raised when an entry listed within table of content |

### setForwardOnly(boolean value) {#setForwardOnly-boolean-}
```
public final void setForwardOnly(boolean value)
```


Sets the flag that indicating that archive is extracted from read-only stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true, if archive's stream is rean-only, false elsewhere. |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public final void setSkipChecksumVerification(boolean value)
```


Sets a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether checksum verification of ZIP entries be skipped and mismatch ignored |

