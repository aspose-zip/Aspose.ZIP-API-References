---
title: "StoreCompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk kompresi Store dalam arsip ZIP."
type: docs
weight: 124
url: /id/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

Pengaturan untuk kompresi Store dalam arsip ZIP.

Metode ini menyimpan data asli apa adanya.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Menginisialisasi instance baru dari kelas [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings). |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Menginisialisasi instance baru dari kelas [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



