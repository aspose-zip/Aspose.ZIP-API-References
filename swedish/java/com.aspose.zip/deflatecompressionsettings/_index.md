---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för Deflate-komprimering i ett ZIP-arkiv."
type: docs
weight: 59
url: /sv/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Inställningar för Deflate-komprimering i ett ZIP-arkiv.

Deflate är en förlustfri datakomprimeringsalgoritm som använder en kombination av LZ77‑algoritmen och Huffman‑kodning.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Initierar en ny instans av klassen [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Initierar en ny instans av klassen [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



