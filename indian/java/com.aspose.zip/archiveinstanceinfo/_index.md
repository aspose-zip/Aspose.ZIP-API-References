---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "अभिलेख इंस्टेंस के बारे में जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 34
url: /hi/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

अभिलेख इंस्टेंस के बारे में जानकारी का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | एक मान प्राप्त करता है जो दर्शाता है कि आर्काइव की एंट्री (फ़ाइलों) के नाम एन्क्रिप्टेड हैं या नहीं। |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | आर्काइव फ़ॉर्मेट जानकारी प्राप्त करता है। |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | आर्काइव फ़ॉर्मेट जानकारी प्राप्त करता है। |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | आर्काइव इंस्टेंस जानकारी प्राप्त करता है। |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | आर्काइव इंस्टेंस जानकारी प्राप्त करता है। |
| [getFormatInfo()](#getFormatInfo--) | आर्काइव फ़ॉर्मेट जानकारी प्राप्त करता है। |
| [isContentEncrypted()](#isContentEncrypted--) | आर्काइव की सामग्री एन्क्रिप्टेड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


एक मान प्राप्त करता है जो दर्शाता है कि आर्काइव की एंट्री (फ़ाइलों) के नाम एन्क्रिप्टेड हैं या नहीं।

**Returns:**
boolean - आर्काइव की प्रविष्टियों (फ़ाइलों) के नाम एन्क्रिप्टेड हैं या नहीं, यह दर्शाने वाला मान।
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


आर्काइव फ़ॉर्मेट जानकारी प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | आर्काइव फ़ाइल की स्ट्रीम। |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


आर्काइव फ़ॉर्मेट जानकारी प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | आर्काइव फ़ाइल का फ़ाइलनाम। |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


आर्काइव इंस्टेंस जानकारी प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | आर्काइव फ़ाइल की स्ट्रीम। |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


आर्काइव इंस्टेंस जानकारी प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | आर्काइव फ़ाइल का फ़ाइलनाम। |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


आर्काइव फ़ॉर्मेट जानकारी प्राप्त करता है।

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


आर्काइव की सामग्री एन्क्रिप्टेड है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean - आर्काइव की सामग्री एन्क्रिप्टेड है या नहीं, यह दर्शाने वाला मान।
