---
title: "AppleArchiveEntrySettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "फ़ाइल के अंदर प्रविष्टियों को संयोजित करने के लिए उपयोग की जाने वाली सेटिंग्स।"
type: docs
weight: 18
url: /hi/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

फ़ाइल के अंदर प्रविष्टियों को संयोजित करने के लिए उपयोग की जाने वाली सेटिंग्स [AppleArchive](../../com.aspose.zip/applearchive) में।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | नए उदाहरण को प्रारंभ करता है [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) क्लास का। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | संयुक्त Apple Archive पेलोड पर लागू संपीड़न सेटिंग्स प्राप्त करता है। |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | संयुक्त फ़ाइल प्रविष्टियों के लिए CRC32 चेकसम फ़ील्ड शामिल हैं या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | संयुक्त फ़ाइल प्रविष्टियों के लिए CRC32 चेकसम फ़ील्ड शामिल हैं या नहीं, यह दर्शाने वाला मान सेट करता है। |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


नए उदाहरण को प्रारंभ करता है [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) क्लास का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | संयुक्त Apple Archive पेलोड पर लागू संपीड़न सेटिंग्स। |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


संयुक्त Apple Archive पेलोड पर लागू संपीड़न सेटिंग्स प्राप्त करता है।

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


संयुक्त फ़ाइल प्रविष्टियों के लिए CRC32 चेकसम फ़ील्ड शामिल हैं या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - एक मान जो दर्शाता है कि संयुक्त फ़ाइल प्रविष्टियों के लिए CRC32 चेकसम फ़ील्ड शामिल हैं या नहीं।
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


संयुक्त फ़ाइल प्रविष्टियों के लिए CRC32 चेकसम फ़ील्ड शामिल हैं या नहीं, यह दर्शाने वाला मान सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | एक मान जो दर्शाता है कि संयुक्त फ़ाइल प्रविष्टियों के लिए CRC32 चेकसम फ़ील्ड शामिल हैं या नहीं। |

