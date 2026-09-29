---
title: "PPMdCompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη συμπίεση PPMd μέσα σε ένα αρχείο ZIP."
type: docs
weight: 93
url: /el/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Ρυθμίσεις για τη συμπίεση PPMd μέσα σε ένα αρχείο ZIP.

Το PPMd είναι ένας αλγόριθμος συμπίεσης δεδομένων που αναπτύχθηκε από τον Dmitry Shkarin. Αυτός ο αλγόριθμος βασίζεται στην προβλεπτική αντιστοίχιση φράσεων σε πολλαπλά συμφραζόμενα τάξης.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) με προεπιλεγμένη σειρά μοντέλου και μέγεθος υπο-εκχωρητή. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Λαμβάνει τη σειρά του μοντέλου. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Λαμβάνει το μέγεθος του υπο-κατανεμητή σε MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

Η προεπιλεγμένη σειρά μοντέλου είναι 8 και το μέγεθος του υπο-εκχωρητή είναι 50 MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Λαμβάνει τη σειρά του μοντέλου.

**Returns:**
int - η σειρά του μοντέλου
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Λαμβάνει το μέγεθος του υπο-κατανεμητή σε MB.

**Returns:**
int - το μέγεθος του υπο-κατανεμητή σε MB
