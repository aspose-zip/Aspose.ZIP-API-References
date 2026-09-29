---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP अभिलेख के भीतर Xz संपीड़न के लिए सेटिंग्स।"
type: docs
weight: 149
url: /hi/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

ZIP अभिलेख के भीतर Xz संपीड़न के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | एक नया उदाहरण प्रारंभ करता है [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) क्लास का। |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


एक नया उदाहरण प्रारंभ करता है [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) क्लास का।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



