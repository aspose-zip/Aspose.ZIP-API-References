---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für Deflate-Kompression innerhalb eines ZIP-Archivs."
type: docs
weight: 59
url: /de/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Einstellungen für Deflate-Kompression innerhalb eines ZIP-Archivs.

Deflate ist ein verlustfreier Datenkompressionsalgorithmus, der eine Kombination aus dem LZ77-Algorithmus und Huffman-Codierung verwendet.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Initialisiert eine neue Instanz der Klasse [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Initialisiert eine neue Instanz der Klasse [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



