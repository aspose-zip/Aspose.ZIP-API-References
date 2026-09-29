---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "बहु-आयतन 7-zip संग्रह को सहेजने के विकल्प।"
type: docs
weight: 123
url: /hi/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

बहु-आयतन 7-zip संग्रह को सहेजने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | बहु-आयतन 7z संग्रह को सहेजने के लिए सेटिंग्स को इंस्टैंसिएट करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getFileName()](#getFileName--) | सेगमेंट्स का नाम बिना एक्सटेंशन के प्राप्त करता है। |
| [getSegmentSize()](#getSegmentSize--) | सेगमेंट का आकार प्राप्त करता है। |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


बहु-आयतन 7z संग्रह को सहेजने के लिए सेटिंग्स को इंस्टैंसिएट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fileName | java.lang.String | आयतनों के लिए नाम। .7z एक्सटेंशन के साथ या बिना भी हो सकता है। |

फ़ाइलों के नाम इस प्रकार होंगे: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | आयतन का आकार। |

कुछ आयतन `segmentSize` से कम हो सकते हैं। अधिकांश मामलों में, अंतिम सेगमेंट कम होगा लेकिन कभी‑कभी नियमित सेगमेंट भी बहुत छोटा हो सकता है। |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


सेगमेंट्स का नाम बिना एक्सटेंशन के प्राप्त करता है।

**Returns:**
java.lang.String - एक्सटेंशन के बिना सेगमेंट का नाम
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


सेगमेंट का आकार प्राप्त करता है।

**Returns:**
long - सेगमेंट का आकार।
