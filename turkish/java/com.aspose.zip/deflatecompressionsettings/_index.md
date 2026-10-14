---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivi içinde Deflate sıkıştırması için ayarlar."
type: docs
weight: 59
url: /tr/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

ZIP arşivi içinde Deflate sıkıştırması için ayarlar.

Deflate, LZ77 algoritması ve Huffman kodlamasının bir kombinasyonunu kullanan kayıpsız bir veri sıkıştırma algoritmasıdır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | Yeni bir [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) sınıfı örneği başlatır. |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


Yeni bir [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) sınıfı örneği başlatır.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



