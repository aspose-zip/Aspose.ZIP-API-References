---
title: "DeflateCompressionSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per la compressione Deflate all'interno di un archivio ZIP."
type: docs
weight: 59
url: /it/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Impostazioni per la compressione Deflate all'interno di un archivio ZIP.

Deflate è un algoritmo di compressione dati senza perdita che utilizza una combinazione dell'algoritmo LZ77 e della codifica Huffman.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Inizializza una nuova istanza della classe [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Inizializza una nuova istanza della classe [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



