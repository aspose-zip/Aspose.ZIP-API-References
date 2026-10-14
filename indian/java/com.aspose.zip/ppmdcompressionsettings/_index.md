---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP अभिलेख में PPMd संपीड़न के लिए सेटिंग्स।"
type: docs
weight: 93
url: /hi/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

ZIP अभिलेख में PPMd संपीड़न के लिए सेटिंग्स।

PPMd एक डेटा संपीड़न एल्गोरिदम है जिसे Dmitry Shkarin ने विकसित किया है। यह एल्गोरिदम कई क्रम संदर्भों में भविष्यवाणी वाक्यांश मिलान पर आधारित है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | एक नया उदाहरण [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) क्लास का प्रारंभ करता है। |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | डिफ़ॉल्ट मॉडल क्रम और सब-एलोकेटर आकार के साथ [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) क्लास का एक नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | मॉडल का क्रम प्राप्त करता है। |
| [getSuballocatorSize()](#getSuballocatorSize--) | सब-एलोकेटर आकार MB में प्राप्त करता है। |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


एक नया उदाहरण [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) क्लास का प्रारंभ करता है।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(\"zipFile.zip\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

डिफ़ॉल्ट मॉडल क्रम 8 है, और सब-एलोकेटर आकार 50MB है।

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


मॉडल का क्रम प्राप्त करता है।

**Returns:**
int - मॉडल का क्रम
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


सब-एलोकेटर आकार MB में प्राप्त करता है।

**Returns:**
int - सब-एलोकेटर आकार MB में
