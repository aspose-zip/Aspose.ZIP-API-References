---
title: "StoreCompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات ضغط Store داخل أرشيف ZIP."
type: docs
weight: 124
url: /ar/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

إعدادات ضغط Store داخل أرشيف ZIP.

هذه الطريقة تخزن البيانات الأصلية كما هي.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | ينشئ مثيلًا جديدًا من الفئة [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


ينشئ مثيلًا جديدًا من الفئة [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



