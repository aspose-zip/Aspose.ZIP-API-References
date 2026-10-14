---
title: "Bzip2CompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη συμπίεση Bzip2 μέσα σε αρχείο ZIP."
type: docs
weight: 41
url: /el/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

Ρυθμίσεις για τη συμπίεση Bzip2 μέσα σε αρχείο ZIP.

το bzip2 συμπιέζει αρχεία χρησιμοποιώντας τον αλγόριθμο συμπίεσης κειμένου Burrows‑Wheeler με ταξινόμηση μπλοκ, και την κωδικοποίηση Huffman.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings). |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) με προεπιλεγμένο μέγεθος μπλοκ, ίσο με 9 εκατοντάδες kilobytes. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Μέγεθος μπλοκ σε εκατοντάδες kilobytes. |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Μέγεθος μπλοκ σε εκατοντάδες kilobytes.

**Returns:**
int - μέγεθος μπλοκ σε εκατοντάδες kilobytes
