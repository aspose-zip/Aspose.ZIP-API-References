---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP संग्रह के भीतर Store संपीड़न के लिए सेटिंग्स।"
type: docs
weight: 124
url: /hi/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

ZIP संग्रह के भीतर Store संपीड़न के लिए सेटिंग्स।

यह मेथड मूल डेटा को जैसा है वैसा ही संग्रहीत करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | एक नया उदाहरण [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) क्लास का प्रारंभ करता है। |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


एक नया उदाहरण [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) क्लास का प्रारंभ करता है।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



