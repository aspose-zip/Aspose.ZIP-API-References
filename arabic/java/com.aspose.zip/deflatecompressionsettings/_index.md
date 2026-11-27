---
title: "DeflateCompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات ضغط Deflate داخل أرشيف ZIP."
type: docs
weight: 59
url: /ar/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

إعدادات ضغط Deflate داخل أرشيف ZIP.

Deflate هو خوارزمية ضغط بيانات غير فقدانية تستخدم مزيجًا من خوارزمية LZ77 وترميز هوفمان.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | يُنشئ مثيلًا جديدًا من الفئة [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


يُنشئ مثيلًا جديدًا من الفئة [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



