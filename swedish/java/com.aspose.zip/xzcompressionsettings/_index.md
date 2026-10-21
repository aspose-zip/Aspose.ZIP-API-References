---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för Xz-komprimering i ett ZIP-arkiv."
type: docs
weight: 149
url: /sv/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Inställningar för Xz-komprimering i ett ZIP-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Initierar en ny instans av klassen [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings). |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Initierar en ny instans av klassen [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



