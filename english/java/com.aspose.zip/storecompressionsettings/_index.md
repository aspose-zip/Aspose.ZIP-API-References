---
title: StoreCompressionSettings
second_title: Aspose.ZIP for Java API Reference
description: Settings for Store compression method.
type: docs
weight: 101
url: /java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Settings for Store compression method.

This method stores original data as it is.
## Constructors

| Constructor | Description |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Initializes a new instance of the [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) class. |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Initializes a new instance of the [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) class.

```

    try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
        archive.createEntry("data.bin", "data.bin");
        archive.save(zipFile);
    }
 
```



