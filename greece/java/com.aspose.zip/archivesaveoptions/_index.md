---
title: "ArchiveSaveOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για αποθήκευση ενός αρχείου ZIP."
type: docs
weight: 36
url: /el/java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Επιλογές για αποθήκευση ενός αρχείου ZIP.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Λαμβάνει προαιρετικό σχόλιο για το αρχείο Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης. |
| [getDataDescriptorPolicy()](#getDataDescriptorPolicy--) | Λαμβάνει ρυθμίσεις για την εκπομπή του Data Descriptor. |
| [getEncoding()](#getEncoding--) | Λαμβάνει κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes. |
| [getEncryptionOptions()](#getEncryptionOptions--) | Λαμβάνει ρυθμίσεις κρυπτογράφησης για την αποθήκευση υπάρχοντος αρχείου ZIP. |
| [getEventsBag()](#getEventsBag--) | Λαμβάνει το δοχείο των γεγονότων που ενεργοποιούνται κατά την αποθήκευση του αρχείου. |
| [getParallelOptions()](#getParallelOptions--) | Λαμβάνει ρυθμίσεις για παράλληλη συμπίεση. |
| [getSelfExtractorOptions()](#getSelfExtractorOptions--) | Λαμβάνει ρυθμίσεις για αυτό-εξαγώγιμο αρχείο. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Ορίζει προαιρετικό σχόλιο για το αρχείο Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης. |
| [setDataDescriptorPolicy(ZipDataDescriptorPolicy value)](#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-) | Ορίζει ρυθμίσεις για την εκπομπή του Data Descriptor. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ορίζει κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes. |
| [setEncryptionOptions(EncryptionSettings value)](#setEncryptionOptions-com.aspose.zip.EncryptionSettings-) | Ορίζει ρυθμίσεις κρυπτογράφησης για την αποθήκευση υπάρχοντος αρχείου ZIP. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Ορίζει το δοχείο των γεγονότων που ενεργοποιούνται κατά την αποθήκευση του αρχείου. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Ορίζει ρυθμίσεις για παράλληλη συμπίεση. |
| [setSelfExtractorOptions(SelfExtractorOptions value)](#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-) | Ορίζει ρυθμίσεις για αυτό-εξαγώγιμο αρχείο. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Λαμβάνει προαιρετικό σχόλιο για το αρχείο Zip.

**Returns:**
java.lang.String - προαιρετικό σχόλιο για το αρχείο Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης.
### getDataDescriptorPolicy() {#getDataDescriptorPolicy--}
```
public final ZipDataDescriptorPolicy getDataDescriptorPolicy()
```


Λαμβάνει ρυθμίσεις για την εκπομπή του Data Descriptor.

Η προεπιλεγμένη επιλογή είναι πάντα ο περιγραφέας δεδομένων που υπάρχει.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) - settings for Data Descriptor emission.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Λαμβάνει κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes.

Εάν δεν οριστεί, θα χρησιμοποιηθεί η κωδικοσελίδα 437.

**Returns:**
java.nio.charset.Charset - κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes.
### getEncryptionOptions() {#getEncryptionOptions--}
```
public final EncryptionSettings getEncryptionOptions()
```


Λαμβάνει ρυθμίσεις κρυπτογράφησης για την αποθήκευση υπάρχοντος αρχείου ZIP.

```

``````

try (Archive archive = new Archive("plain.zip")) {
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
archive.save("encripted.zip", options);
}
 
```

Do not use this options for regular composition of encrypted archive, use

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) instead.

Not compatible with `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) having value [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Returns:**
[EncryptionSettings](../../com.aspose.zip/encryptionsettings) - encryption settings for saving existing ZIP archive.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Gets container of events raising on archive saving.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getParallelOptions() {#getParallelOptions--}
```
public final ParallelOptions getParallelOptions()
```


Gets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Returns:**
[ParallelOptions](../../com.aspose.zip/paralleloptions) - settings for parallel compression.
### getSelfExtractorOptions() {#getSelfExtractorOptions--}
```
public final SelfExtractorOptions getSelfExtractorOptions()
```


Gets settings for self extracted archive.

Assign it if you need to compose executable program to extract an archive without any software installed on the target computer.

**Returns:**
[SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) - settings for self extracted archive.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Sets optional comment for the Zip file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | optional comment for the Zip file. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Sets a value indicating whether entries' sources should be closed right after an entry has been compressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether entries' sources should be closed right after an entry has been compressed. |

### setDataDescriptorPolicy(ZipDataDescriptorPolicy value) {#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-}
```
public final void setDataDescriptorPolicy(ZipDataDescriptorPolicy value)
```


Sets settings for Data Descriptor emission.

Default option is always present data descriptor.

[ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries) is not compatible with archive encryption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy) | settings for Data Descriptor emission. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding for converting file names and other strings to bytes. |

### setEncryptionOptions(EncryptionSettings value) {#setEncryptionOptions-com.aspose.zip.EncryptionSettings-}
```
public final void setEncryptionOptions(EncryptionSettings value)
```


Sets encryption settings for saving existing ZIP archive.

```

``````

    try (Archive archive = new Archive("plain.zip")) {
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncryptionOptions(new AesEncryptionSettings("p@s$", EncryptionMethod.AES256));
        archive.save("encripted.zip", options);
    }
 
```

Μην χρησιμοποιείτε αυτές τις επιλογές για κανονική σύνθεση κρυπτογραφημένου αρχείου, χρησιμοποιήστε

`new com.aspose.zip.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)`([ArchiveEntrySettings.ArchiveEntrySettings(CompressionSettings, EncryptionSettings)](../../com.aspose.zip/archiveentrysettings\#ArchiveEntrySettings-CompressionSettings--EncryptionSettings-)) αντί αυτού.

Μη συμβατό με `DataDescriptorPolicy`([getDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#getDataDescriptorPolicy--)/[setDataDescriptorPolicy](../../com.aspose.zip/archivesaveoptions\#setDataDescriptorPolicy-com.aspose.zip.ZipDataDescriptorPolicy-)) που έχει τιμή [ZipDataDescriptorPolicy.ForAllFileEntries](../../com.aspose.zip/zipdatadescriptorpolicy\#ForAllFileEntries)

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [EncryptionSettings](../../com.aspose.zip/encryptionsettings) | ορίζει τις ρυθμίσεις κρυπτογράφησης για την αποθήκευση υπάρχοντος αρχείου ZIP. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Ορίζει το δοχείο των γεγονότων που ενεργοποιούνται κατά την αποθήκευση του αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | υποδοχέας των γεγονότων που δημιουργούνται κατά την αποθήκευση του αρχείου. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Ορίζει ρυθμίσεις για παράλληλη συμπίεση.

Αντιστοιχίστε το εάν θέλετε να αξιοποιήσετε πολλούς πυρήνες CPU κατά τη συμπίεση πολλαπλών καταχωρήσεων του αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | ρυθμίσεις για παράλληλη συμπίεση. |

### setSelfExtractorOptions(SelfExtractorOptions value) {#setSelfExtractorOptions-com.aspose.zip.SelfExtractorOptions-}
```
public final void setSelfExtractorOptions(SelfExtractorOptions value)
```


Ορίζει ρυθμίσεις για αυτό-εξαγώγιμο αρχείο.

Αναθέστε το εάν χρειάζεστε να δημιουργήσετε εκτελέσιμο πρόγραμμα για την εξαγωγή ενός αρχείου χωρίς κανένα λογισμικό εγκατεστημένο στον υπολογιστή-στόχο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [SelfExtractorOptions](../../com.aspose.zip/selfextractoroptions) | ρυθμίσεις για αυτό-εξαγώγιμο αρχείο. |

