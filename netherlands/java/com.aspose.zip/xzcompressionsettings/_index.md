---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor Xz-compressie binnen een ZIP-archief."
type: docs
weight: 149
url: /nl/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Instellingen voor Xz-compressie binnen een ZIP-archief.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Initialiseert een nieuw exemplaar van de [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) klasse. |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Initialiseert een nieuw exemplaar van de [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) klasse.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



