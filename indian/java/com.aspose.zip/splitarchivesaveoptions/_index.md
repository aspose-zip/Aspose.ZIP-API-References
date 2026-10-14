---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "बहु-आयतन ZIP संग्रह को सहेजने के विकल्प।"
type: docs
weight: 122
url: /hi/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

बहु-आयतन ZIP संग्रह को सहेजने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | एक बहु-आयतन ZIP अभिलेख को सहेजने के लिए सेटिंग्स को इंस्टैंसिएट करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip फ़ाइल के लिए वैकल्पिक टिप्पणी प्राप्त करता है। |
| [getCloseEntrySource()](#getCloseEntrySource--) | एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं। |
| [getEncoding()](#getEncoding--) | फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग प्राप्त करता है। |
| [getEventsBag()](#getEventsBag--) | आर्काइव सहेजने पर उत्पन्न होने वाली घटनाओं के कंटेनर को प्राप्त करता है। |
| [getFileName()](#getFileName--) | सेगमेंट्स का नाम बिना एक्सटेंशन के प्राप्त करता है। |
| [getSegmentSize()](#getSegmentSize--) | सेगमेंट का आकार प्राप्त करता है। |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip फ़ाइल के लिए वैकल्पिक टिप्पणी सेट करता है। |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | एक मान सेट करता है जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं। |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग सेट करता है। |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | आर्काइव सहेजने पर उत्पन्न होने वाली घटनाओं के कंटेनर को सेट करता है। |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


एक बहु-आयतन ZIP अभिलेख को सहेजने के लिए सेटिंग्स को इंस्टैंसिएट करता है।

कुछ आयतन `segmentSize` से कम हो सकते हैं। अधिकांश मामलों में, अंतिम सेगमेंट कम होगा लेकिन कभी‑कभी सामान्य सेगमेंट भी बहुत कम हो सकते हैं।

फ़ाइलों के नाम इस प्रकार होंगे: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | आयतन के लिए नाम। .zip एक्सटेंशन के साथ या बिना हो सकता है। |
| segmentSize | long | आयतन का आकार। |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Zip फ़ाइल के लिए वैकल्पिक टिप्पणी प्राप्त करता है।

**Returns:**
java.lang.String - ज़िप फ़ाइल के लिए वैकल्पिक टिप्पणी।
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि प्रविष्टियों के स्रोत को संपीड़ित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं।
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग प्राप्त करता है।

यदि सेट नहीं किया गया, तो कोड पेज 437 उपयोग किया जाएगा।

**Returns:**
java.nio.charset.Charset - फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग।
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


आर्काइव सहेजने पर उत्पन्न होने वाली घटनाओं के कंटेनर को प्राप्त करता है।

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


सेगमेंट्स का नाम बिना एक्सटेंशन के प्राप्त करता है।

**Returns:**
java.lang.String - सेगमेंट्स का नाम बिना एक्सटेंशन के।
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


सेगमेंट का आकार प्राप्त करता है।

**Returns:**
long - सेगमेंट का आकार।
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Zip फ़ाइल के लिए वैकल्पिक टिप्पणी सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | Zip फ़ाइल के लिए वैकल्पिक टिप्पणी। |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | एक मान जो दर्शाता है कि प्रविष्टियों के स्रोत को संकुचित होने के तुरंत बाद बंद किया जाना चाहिए या नहीं। |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग सेट करता है।

यदि सेट नहीं किया गया, तो कोड पेज 437 उपयोग किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.nio.charset.Charset | फ़ाइल नामों और अन्य स्ट्रिंग्स को बाइट्स में बदलने के लिए एन्कोडिंग। |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


आर्काइव सहेजने पर उत्पन्न होने वाली घटनाओं के कंटेनर को सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | आर्काइव सहेजने पर घटनाओं को उठाने वाला कंटेनर। |

