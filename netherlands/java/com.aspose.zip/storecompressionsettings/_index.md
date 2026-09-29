---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor Store-compressie binnen een ZIP-archief."
type: docs
weight: 124
url: /nl/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Instellingen voor Store-compressie binnen een ZIP-archief.

Deze methode slaat originele gegevens op zoals ze zijn.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Initialiseert een nieuw exemplaar van de [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) klasse. |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Initialiseert een nieuw exemplaar van de [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) klasse.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



