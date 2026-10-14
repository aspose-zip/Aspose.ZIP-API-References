---
title: "ArchiveEntrySettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις που χρησιμοποιούνται για τη συμπίεση ή την αποσυμπίεση καταχωρίσεων."
type: docs
weight: 30
url: /el/java/com.aspose.zip/archiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveEntrySettings
```

Ρυθμίσεις που χρησιμοποιούνται για τη συμπίεση ή την αποσυμπίεση καταχωρίσεων.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ArchiveEntrySettings()](#ArchiveEntrySettings--) | Αρχικοποιεί μια νέα παρουσία της [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) κλάσης. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-) | Αρχικοποιεί μια νέα παρουσία της [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) κλάσης. |
| [ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)](#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-) | Αρχικοποιεί μια νέα παρουσία της [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) κλάσης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getComment()](#getComment--) | Λαμβάνει το σχόλιο για την καταχώρηση μέσα στο αρχείο ZIP. |
| [getCompressionSettings()](#getCompressionSettings--) | Λαμβάνει τις ρυθμίσεις για τη διαδικασία συμπίεσης ή αποσυμπίεσης. |
| [getEncryptionSettings()](#getEncryptionSettings--) | Λαμβάνει τις ρυθμίσεις για κρυπτογράφηση ή αποκρυπτογράφηση. |
| [setComment(String value)](#setComment-java.lang.String-) | Σχόλιο για την καταχώρηση μέσα στο αρχείο ZIP. |
### ArchiveEntrySettings() {#ArchiveEntrySettings--}
```
public ArchiveEntrySettings()
```


Αρχικοποιεί μια νέα παρουσία της [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) κλάσης.

### ArchiveEntrySettings(CompressionSettings compressionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings)
```


Αρχικοποιεί μια νέα παρουσία της [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) κλάσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Ρυθμίσεις για συμπίεση. Δώστε null για τις προεπιλεγμένες ρυθμίσεις deflate. |

Μπορεί να είναι ένα από τα παρακάτω:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |

### ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings) {#ArchiveEntrySettings-com.aspose.zip.CompressionSettings-com.aspose.zip.EncryptionSettings-}
```
public ArchiveEntrySettings(CompressionSettings compressionSettings, EncryptionSettings encryptionSettings)
```


Αρχικοποιεί μια νέα παρουσία της [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) κλάσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | compressionSettings | [CompressionSettings](../../com.aspose.zip/compressionsettings) | Ρυθμίσεις για συμπίεση. Δώστε null για τις προεπιλεγμένες ρυθμίσεις deflate. |

Μπορεί να είναι ένα από τα παρακάτω:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) |
|  | encryptionSettings | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | Ρυθμίσεις για κρυπτογράφηση. Δώστε null αν δεν χρειάζεται κρυπτογράφηση ή αποκρυπτογράφηση. |

Μπορεί να είναι ένα από τα παρακάτω:

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings) |

### getComment() {#getComment--}
```
public final String getComment()
```


Λαμβάνει το σχόλιο για την καταχώρηση μέσα στο αρχείο ZIP.

**Returns:**
java.lang.String - σχόλιο για την καταχώρηση μέσα στο αρχείο ZIP.
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Λαμβάνει τις ρυθμίσεις για τη διαδικασία συμπίεσης ή αποσυμπίεσης.

Μπορεί να είναι ένα από τα παρακάτω:

 *  [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings)
 *  [EnhancedDeflateCompressionSettings](../../com.aspose.zip/enhanceddeflatecompressionsettings)
 *  [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings)

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression routine.
### getEncryptionSettings() {#getEncryptionSettings--}
```
public final EncryptionSettings getEncryptionSettings()
```


Λαμβάνει τις ρυθμίσεις για κρυπτογράφηση ή αποκρυπτογράφηση. Οι ρυθμίσεις μιας συγκεκριμένης καταχώρησης μπορεί να διαφέρουν.

 *  [TraditionalEncryptionSettings](../../com.aspose.zip/traditionalencryptionsettings)
 *  [AesEncryptionSettings](../../com.aspose.zip/aesencryptionsettings)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - settings for encryption or decryption. Settings of particular entry may vary.
### setComment(String value) {#setComment-java.lang.String-}
```
public final void setComment(String value)
```


Σχόλιο για την καταχώρηση μέσα στο αρχείο ZIP.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.lang.String |  |

