---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die Store-Komprimierung innerhalb eines ZIP-Archivs."
type: docs
weight: 124
url: /de/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Einstellungen für die Store-Komprimierung innerhalb eines ZIP-Archivs.

Diese Methode speichert die Originaldaten unverändert.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Initialisiert eine neue Instanz der Klasse [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Initialisiert eine neue Instanz der Klasse [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



