---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor Deflate-compressie binnen een ZIP-archief."
type: docs
weight: 59
url: /nl/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Instellingen voor Deflate-compressie binnen een ZIP-archief.

Deflate is een verliesloos gegevenscompressie-algoritme dat een combinatie van het LZ77-algoritme en Huffman-codering gebruikt.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Initialiseert een nieuw exemplaar van de [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) klasse. |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Initialiseert een nieuw exemplaar van de [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) klasse.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



