---
title: "StoreCompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la compressione Store all'interno di un archivio ZIP."
type: docs
weight: 124
url: /it/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Impostazioni per la compressione Store all'interno di un archivio ZIP.

Questo metodo memorizza i dati originali così come sono.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Inizializza una nuova istanza della classe [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Inizializza una nuova istanza della classe [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



