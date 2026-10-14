---
title: "SevenZipLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές με τις οποίες  φορτώνεται από ένα συμπιεσμένο αρχείο."
type: docs
weight: 116
url: /el/java/com.aspose.zip/sevenziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipLoadOptions
```

Επιλογές με τις οποίες το [SevenZipArchive](../../com.aspose.zip/sevenziparchive) φορτώνεται από ένα συμπιεσμένο αρχείο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SevenZipLoadOptions()](#SevenZipLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Λαμβάνει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων και των ονομάτων καταχωρίσεων. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων και των ονομάτων καταχωρίσεων. |
### SevenZipLoadOptions() {#SevenZipLoadOptions--}
```
public SevenZipLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public final String getDecryptionPassword()
```


Λαμβάνει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων και των ονομάτων καταχωρίσεων.

Μπορείτε να παρέχετε τον κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή του αρχείου.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Returns:**
java.lang.String - the password to decrypt entries and entry names.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel 7Z archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setCancellationFlag(cf);
         try (SevenZipArchive a = new SevenZipArchive("big.7z", options)) {
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


Ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων και των ονομάτων καταχωρίσεων.

Μπορείτε να παρέχετε τον κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή του αρχείου.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted_archive.7z");
FileOutputStream extracted = new FileOutputStream("extracted.bin")) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("p@s$");
try (SevenZipArchive archive = new SevenZipArchive(fs, options);
InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the password to decrypt entries and entry names. |

