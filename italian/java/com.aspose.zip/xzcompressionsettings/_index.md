---
title: "XzCompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la compressione Xz all'interno di un archivio ZIP."
type: docs
weight: 149
url: /it/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Impostazioni per la compressione Xz all'interno di un archivio ZIP.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Inizializza una nuova istanza della classe [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings). |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Inizializza una nuova istanza della classe [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



