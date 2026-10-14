---
title: "StoreCompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη συμπίεση Store μέσα σε αρχείο ZIP."
type: docs
weight: 124
url: /el/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Ρυθμίσεις για τη συμπίεση Store μέσα σε αρχείο ZIP.

Αυτή η μέθοδος αποθηκεύει τα αρχικά δεδομένα όπως είναι.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



