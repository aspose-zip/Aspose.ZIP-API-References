---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7z अभिलेख में PPMd संपीड़न विधि के लिए सेटिंग्स।"
type: docs
weight: 117
url: /hi/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

7z अभिलेख में PPMd संपीड़न विधि के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | 7z आर्काइव के भीतर PPMd संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है। |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | डिफ़ॉल्ट मॉडल क्रम और सब-एलोकेटर आकार के साथ 7z आर्काइव के भीतर PPMd संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | अधिकतम क्रम प्राप्त करता है। |
| [getMethod()](#getMethod--) | संपीड़न या डिकम्प्रेशन विधि प्राप्त करता है। |
| [getSuballocatorSize()](#getSuballocatorSize--) | सब-एलोकेटर आकार MB में प्राप्त करता है। |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


7z आर्काइव के भीतर PPMd संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(\"zipFile.zip\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

डिफ़ॉल्ट मॉडल क्रम 6 है और सब-एलोकेटर आकार 16MB है।

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


अधिकतम क्रम प्राप्त करता है।

**Returns:**
byte - अधिकतम क्रम
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


संपीड़न या डिकम्प्रेशन विधि प्राप्त करता है।

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


सब-एलोकेटर आकार MB में प्राप्त करता है।

**Returns:**
int - सब-एलोकेटर आकार MB में
