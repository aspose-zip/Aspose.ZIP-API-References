---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ZIP अभिलेख के भीतर Bzip2 संपीड़न के लिए सेटिंग्स।"
type: docs
weight: 41
url: /hi/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

ZIP अभिलेख के भीतर Bzip2 संपीड़न के लिए सेटिंग्स।

bzip2 फ़ाइलों को Burrows-Wheeler ब्लॉक सॉर्टिंग टेक्स्ट संपीड़न एल्गोरिदम और Huffman कोडिंग का उपयोग करके संपीड़ित करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | एक नया उदाहरण प्रारंभ करता है [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) क्लास का। |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | डिफ़ॉल्ट ब्लॉक आकार के साथ, जो 9 सौ किलोबाइट के बराबर है, [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) क्लास का एक नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | ब्लॉक आकार सौ किलोबाइट में। |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


एक नया उदाहरण प्रारंभ करता है [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) क्लास का।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


ब्लॉक आकार सौ किलोबाइट में।

**Returns:**
int - ब्लॉक आकार सौ किलोबाइट में
