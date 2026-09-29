---
title: "XzCompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk kompresi Xz dalam arsip ZIP."
type: docs
weight: 149
url: /id/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

Pengaturan untuk kompresi Xz dalam arsip ZIP.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Menginisialisasi instance baru dari kelas [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings). |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Menginisialisasi instance baru dari kelas [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



