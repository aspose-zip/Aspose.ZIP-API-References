---
title: "XarBzip2CompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "Bzip2 संपीड़न विधि के लिए सेटिंग्स।"
type: docs
weight: 137
url: /hi/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Bzip2 संपीड़न विधि के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | एक नया उदाहरण प्रारंभ करता है [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) क्लास का। |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | डिफ़ॉल्ट ब्लॉक आकार, जो 9 सौ किलोबाइट के बराबर है, के साथ [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) क्लास का नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ब्लॉक आकार सौ किलोबाइट में। |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


एक नया उदाहरण प्रारंभ करता है [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) क्लास का।

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", "data.bin", false, new XarBzip2CompressionSettings(1));
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | block size in hundreds of kilobytes |

### XarBzip2CompressionSettings() {#XarBzip2CompressionSettings--}
```
public XarBzip2CompressionSettings()
```


Initializes a new instance of the [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
