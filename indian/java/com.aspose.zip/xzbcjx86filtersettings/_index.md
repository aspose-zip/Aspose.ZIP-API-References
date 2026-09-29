---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "xz Bcj X86 फ़िल्टर के लिए सेटिंग्स।"
type: docs
weight: 148
url: /hi/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

xz Bcj X86 फ़िल्टर के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | एक नया उदाहरण प्रारंभ करता है [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


एक नया उदाहरण प्रारंभ करता है [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). इसका उपयोग [XzArchive](../../com.aspose.zip/xzarchive) के भीतर निष्पादन योग्य फ़ाइलों और लाइब्रेरीज़ को संपीड़ित करने के लिए करें।

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save("archive.xz");
}
 
```



