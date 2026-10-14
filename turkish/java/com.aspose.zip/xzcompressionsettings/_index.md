---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ZIP arşivi içinde Xz sıkıştırması için ayarlar."
type: docs
weight: 149
url: /tr/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

ZIP arşivi içinde Xz sıkıştırması için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | Yeni bir [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) sınıfı örneği başlatır. |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


Yeni bir [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) sınıfı örneği başlatır.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(\"archive.zip\");
}
 
```



