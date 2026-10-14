---
title: "XzCompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات ضغط Xz داخل أرشيف ZIP."
type: docs
weight: 149
url: /ar/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

إعدادات ضغط Xz داخل أرشيف ZIP.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | ينشئ مثيلاً جديداً من الفئة [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings). |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


ينشئ مثيلاً جديداً من الفئة [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(\"archive.zip\");
}
 
```



