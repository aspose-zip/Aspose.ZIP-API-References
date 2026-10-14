---
title: "DeflateCompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk kompresi Deflate dalam arsip ZIP."
type: docs
weight: 59
url: /id/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

Pengaturan untuk kompresi Deflate dalam arsip ZIP.

Deflate adalah algoritma kompresi data tanpa kehilangan yang menggunakan kombinasi algoritma LZ77 dan pengkodean Huffman.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Menginisialisasi instance baru dari kelas [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings). |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Menginisialisasi instance baru dari kelas [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



