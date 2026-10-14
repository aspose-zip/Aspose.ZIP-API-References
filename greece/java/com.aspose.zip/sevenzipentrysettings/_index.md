---
title: "SevenZipEntrySettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις που χρησιμοποιούνται για τη συμπίεση ή αποσυμπίεση καταχωρήσεων 7z."
type: docs
weight: 113
url: /el/java/com.aspose.zip/sevenzipentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class SevenZipEntrySettings
```

Ρυθμίσεις που χρησιμοποιούνται για τη συμπίεση ή αποσυμπίεση καταχωρήσεων 7z.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SevenZipEntrySettings()](#SevenZipEntrySettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
| [SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)](#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompressHeader()](#getCompressHeader--) | Λαμβάνει τιμή που υποδεικνύει εάν θα συμπιεστεί η κεφαλίδα του αρχείου. |
| [getCompressionSettings()](#getCompressionSettings--) | Λαμβάνει τις ρυθμίσεις για τη διαδικασία συμπίεσης ή αποσυμπίεσης. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Λαμβάνει τις ρυθμίσεις για κρυπτογράφηση ή αποκρυπτογράφηση. |
| [getSolid()](#getSolid--) | Λαμβάνει τιμή που υποδεικνύει εάν θα συνενωθούν οι καταχωρήσεις και θα αντιμετωπίζονται ως ένα ενιαίο μπλοκ δεδομένων. |
| [setCompressHeader(boolean value)](#setCompressHeader-boolean-) | Ορίζει τιμή που υποδεικνύει εάν θα συμπιεστεί η κεφαλίδα του αρχείου. |
| [setSolid(boolean value)](#setSolid-boolean-) | Ορίζει τιμή που υποδεικνύει εάν θα συνενωθούν οι καταχωρήσεις και θα αντιμετωπίζονται ως ένα ενιαίο μπλοκ δεδομένων. |
### SevenZipEntrySettings() {#SevenZipEntrySettings--}
```
public SevenZipEntrySettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | ρυθμίσεις για συμπίεση. Περάστε null για τις προεπιλεγμένες ρυθμίσεις LZMA. |

Μπορεί να είναι ένα από τα παρακάτω:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |

### SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings) {#SevenZipEntrySettings-com.aspose.zip.SevenZipCompressionSettings-com.aspose.zip.SevenZipEncryptionSettings-}
```
public SevenZipEntrySettings(SevenZipCompressionSettings compressionSettings, SevenZipEncryptionSettings encryptionSettings)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | compressionSettings | [SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) | ρυθμίσεις για συμπίεση. Περάστε null για τις προεπιλεγμένες ρυθμίσεις LZMA. |

Μπορεί να είναι ένα από τα παρακάτω:

 *  [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings)
 *  [SevenZipLZMA2CompressionSettings](../../com.aspose.zip/sevenziplzma2compressionsettings)
 *  [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings)
 *  [SevenZipPPMdCompressionSettings](../../com.aspose.zip/sevenzipppmdcompressionsettings)
 *  [SevenZipStoreCompressionSettings](../../com.aspose.zip/sevenzipstorecompressionsettings) |
|  | encryptionSettings | [SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) | ρυθμίσεις για κρυπτογράφηση. Περάστε null εάν δεν χρειάζεται κρυπτογράφηση ή αποκρυπτογράφηση. |

Μπορεί να είναι μόνο ένα:

 *  [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) |

### getCompressHeader() {#getCompressHeader--}
```
public final boolean getCompressHeader()
```


Λαμβάνει τιμή που υποδεικνύει εάν θα συμπιεστεί η κεφαλίδα του αρχείου.

Αυτή η ρύθμιση είναι ισοδύναμη με τη μεταβλητή `-mhc=on` του εργαλείου 7-Zip. Προς το παρόν, είναι ασύμβατη με την κρυπτογράφηση της κεφαλίδας.

**Returns:**
boolean - τιμή που υποδεικνύει εάν θα συμπιεστεί η κεφαλίδα του αρχείου
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Λαμβάνει τις ρυθμίσεις για τη διαδικασία συμπίεσης ή αποσυμπίεσης.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression routine
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final SevenZipEncryptionSettings getEncryptionSettings()
```


Λαμβάνει τις ρυθμίσεις για κρυπτογράφηση ή αποκρυπτογράφηση. Οι ρυθμίσεις μιας συγκεκριμένης καταχώρησης μπορεί να διαφέρουν.

Το [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) είναι η μοναδική επιλογή για αρχεία 7z.

**Returns:**
[SevenZipEncryptionSettings](../../com.aspose.zip/sevenzipencryptionsettings) - settings for encryption or decryption
### getSolid() {#getSolid--}
```
public final boolean getSolid()
```


Λαμβάνει τιμή που υποδεικνύει εάν θα συνενωθούν οι καταχωρήσεις και θα αντιμετωπίζονται ως ένα ενιαίο μπλοκ δεδομένων.

Το παρακάτω παράδειγμα δείχνει πώς να συμπιέσετε έναν φάκελο σε συμπαγές αρχείο 7z με συμπίεση LZMA2 χωρίς κρυπτογράφηση.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream(\"archive.7z\")) {
SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
settings.setSolid(true);
try (SevenZipArchive archive = new SevenZipArchive(settings)) {
archive.createEntries(\"C:\\\\Documents\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

Provide `SevenZipEntrySettings` for solid 7z archive on archive instantiation.

**Returns:**
boolean - value indicating whether to concatenate entries and treat them as a single data block.
### setCompressHeader(boolean value) {#setCompressHeader-boolean-}
```
public final void setCompressHeader(boolean value)
```


Sets value indicating whether to compress archive header.

This setting is equivalent `-mhc=on` switch of 7-Zip tool. Currently, it is incompatible with header encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to compress archive header |

### setSolid(boolean value) {#setSolid-boolean-}
```
public final void setSolid(boolean value)
```


Sets value indicating whether to concatenate entries and treat them as a single data block.

The following example shows how to compress a directory to solid 7z archive with LZMA2 compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         SevenZipEntrySettings settings = new SevenZipEntrySettings(new SevenZipLZMACompressionSettings());
         settings.setSolid(true);
         try (SevenZipArchive archive = new SevenZipArchive(settings)) {
             archive.createEntries("C:\\Documents");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Παρέχετε `SevenZipEntrySettings` για συμπαγές αρχείο 7z κατά τη δημιουργία του αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | τιμή που υποδεικνύει εάν θα συνενωθούν οι καταχωρήσεις και θα αντιμετωπίζονται ως ένα ενιαίο μπλοκ δεδομένων. |

