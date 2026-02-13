---
title: XzCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for Xz compression within a ZIP archive.
type: docs
weight: 132
url: /java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Settings for Xz compression within a ZIP archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Initializes a new instance of the [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) class. |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Initializes a new instance of the [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) class.

```

     try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("archive.zip");
     }
 
```



