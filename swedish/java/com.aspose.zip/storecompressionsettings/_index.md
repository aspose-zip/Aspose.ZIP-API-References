---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för Store-komprimering i ett ZIP-arkiv."
type: docs
weight: 124
url: /sv/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Inställningar för Store-komprimering i ett ZIP-arkiv.

Denna metod lagrar originaldata som den är.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Initierar en ny instans av klassen [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Initierar en ny instans av klassen [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



