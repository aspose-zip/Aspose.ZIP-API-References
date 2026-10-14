---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP अभिलेख के भीतर Deflate संपीड़न के लिए सेटिंग्स।"
type: docs
weight: 59
url: /hi/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

ZIP अभिलेख के भीतर Deflate संपीड़न के लिए सेटिंग्स।

Deflate एक लॉसलैस डेटा संपीड़न एल्गोरिदम है जो LZ77 एल्गोरिदम और Huffman कोडिंग के संयोजन का उपयोग करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) क्लास का नया उदाहरण प्रारंभ करता है। |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


[DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) क्लास का नया उदाहरण प्रारंभ करता है।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



