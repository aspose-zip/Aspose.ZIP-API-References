---
title: "DeflateCompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη συμπίεση Deflate μέσα σε αρχείο ZIP."
type: docs
weight: 59
url: /el/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Ρυθμίσεις για τη συμπίεση Deflate μέσα σε αρχείο ZIP.

Το Deflate είναι ένας αλγόριθμος συμπίεσης δεδομένων χωρίς απώλειες που χρησιμοποιεί έναν συνδυασμό του αλγορίθμου LZ77 και της κωδικοποίησης Huffman.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



