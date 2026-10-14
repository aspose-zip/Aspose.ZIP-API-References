---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7z अभिलेख में BZip2 संपीड़न विधि के लिए सेटिंग्स।"
type: docs
weight: 109
url: /hi/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

7z अभिलेख में BZip2 संपीड़न विधि के लिए सेटिंग्स।

Bzip2 फ़ाइलों को Burrows-Wheeler ब्लॉक सॉर्टिंग टेक्स्ट कंप्रेशन एल्गोरिदम और Huffman कोडिंग का उपयोग करके संपीड़ित करता है।

और अधिक देखें: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | एक नया उदाहरण प्रारंभ करता है [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) क्लास का। |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | डिफ़ॉल्ट ब्लॉक आकार के साथ [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) क्लास का नया उदाहरण प्रारंभ करता है, जो 9 सौ किलोबाइट के बराबर है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ब्लॉक आकार सौ किलोबाइट में। |
| [getMethod()](#getMethod--) | संपीड़न या डिकम्प्रेशन विधि प्राप्त करता है। |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


एक नया उदाहरण प्रारंभ करता है [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| blockSize | int | ब्लॉक आकार सौ किलोबाइट में |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


डिफ़ॉल्ट ब्लॉक आकार के साथ [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) क्लास का नया उदाहरण प्रारंभ करता है, जो 9 सौ किलोबाइट के बराबर है।

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


ब्लॉक आकार सौ किलोबाइट में।

**Returns:**
int - ब्लॉक आकार सौ किलोबाइट में
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


संपीड़न या डिकम्प्रेशन विधि प्राप्त करता है।

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
