---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für die Xz-Komprimierung innerhalb eines ZIP-Archivs."
type: docs
weight: 149
url: /de/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Einstellungen für die Xz-Komprimierung innerhalb eines ZIP-Archivs.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Initialisiert eine neue Instanz der [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings)-Klasse. |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Initialisiert eine neue Instanz der [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings)-Klasse.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



