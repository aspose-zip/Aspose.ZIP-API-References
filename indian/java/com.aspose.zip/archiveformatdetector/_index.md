---
title: "ArchiveFormatDetector"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "एक अभिलेख प्रारूप का पता लगाता है और अन्य संबंधित जानकारी प्रदान करता है।"
type: docs
weight: 32
url: /hi/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

एक अभिलेख प्रारूप का पता लगाता है और अन्य संबंधित जानकारी प्रदान करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | एक नया उदाहरण प्रारंभ करता है [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) क्लास का। |
## Methods

| Method | विवरण |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | फ़ॉर्मेट जानकारी प्राप्त करता है। |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | फ़ॉर्मेट जानकारी प्राप्त करता है। |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


एक नया उदाहरण प्रारंभ करता है [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector) क्लास का।

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


फ़ॉर्मेट जानकारी प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | आर्काइव फ़ाइल की स्ट्रीम। |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


फ़ॉर्मेट जानकारी प्राप्त करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | आर्काइव फ़ाइल का फ़ाइलनाम। |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
