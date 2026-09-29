---
title: "XzCompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη συμπίεση Xz μέσα σε αρχείο ZIP."
type: docs
weight: 149
url: /el/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Ρυθμίσεις για τη συμπίεση Xz μέσα σε αρχείο ZIP.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings). |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



