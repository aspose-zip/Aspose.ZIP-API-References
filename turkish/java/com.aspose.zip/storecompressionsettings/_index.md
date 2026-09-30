---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivindeki Store sıkıştırması için ayarlar."
type: docs
weight: 124
url: /tr/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

ZIP arşivindeki Store sıkıştırması için ayarlar.

Bu yöntem, orijinal veriyi olduğu gibi depolar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | Yeni bir [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) sınıfının örneğini başlatır. |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


Yeni bir [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) sınıfının örneğini başlatır.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(zipFile);
}
 
```



