---
title: "StoreCompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la compression Store dans une archive ZIP."
type: docs
weight: 124
url: /fr/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Paramètres pour la compression Store dans une archive ZIP.

Cette méthode stocke les données originales telles quelles.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Initialise une nouvelle instance de la classe [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Initialise une nouvelle instance de la classe [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



