---
title: "Lz4ArchiveSetting"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "LZ4 आर्काइव निर्माण के लिए सेटिंग्स।"
type: docs
weight: 81
url: /hi/java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

LZ4 आर्काइव निर्माण के लिए सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | डिफ़ॉल्ट पैरामीटरों के साथ नया उदाहरण प्रारंभ करता है [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) का। |
## Methods

| Method | विवरण |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | एक मान प्राप्त करता है जो दर्शाता है कि संपीड़ित ब्लॉक के अंत में संपीड़ित xxh32 हैश शामिल किया जाए या नहीं। |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | एक मान प्राप्त करता है जो दर्शाता है कि LZ4 अभिलेख के अंत में सामग्री xxh32 हैश शामिल किया जाए या नहीं। |
| [getIncludeContentSize()](#getIncludeContentSize--) | एक मान प्राप्त करता है जो दर्शाता है कि फ्रेम में सामग्री का आकार शामिल किया जाए या नहीं। |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | एक मान सेट करता है जो दर्शाता है कि संपीड़ित ब्लॉक के अंत में संपीड़ित xxh32 हैश शामिल किया जाए या नहीं। |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | एक मान सेट करता है जो दर्शाता है कि LZ4 अभिलेख के अंत में सामग्री xxh32 हैश शामिल किया जाए या नहीं। |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | एक मान सेट करता है जो दर्शाता है कि फ्रेम में सामग्री का आकार शामिल किया जाए या नहीं। |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


डिफ़ॉल्ट पैरामीटरों के साथ नया उदाहरण प्रारंभ करता है [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) का।

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


एक मान प्राप्त करता है जो दर्शाता है कि संपीड़ित ब्लॉक के अंत में संपीड़ित xxh32 हैश शामिल किया जाए या नहीं।

डिफ़ॉल्ट false है।

**Returns:**
boolean - एक मान जो दर्शाता है कि संपीड़ित ब्लॉक के अंत में संपीड़ित xxh32 हैश शामिल किया जाए या नहीं।
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


एक मान प्राप्त करता है जो दर्शाता है कि LZ4 अभिलेख के अंत में सामग्री xxh32 हैश शामिल किया जाए या नहीं।

डिफ़ॉल्ट true है।

**Returns:**
boolean - यह मान दर्शाता है कि क्या LZ4 संग्रह के अंत में सामग्री xxh32 हैश शामिल किया जाए।
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


एक मान प्राप्त करता है जो दर्शाता है कि फ्रेम में सामग्री का आकार शामिल किया जाए या नहीं।

डिफ़ॉल्ट मान false है। जब स्रोत स्ट्रीम seekable हो तो लागू होता है।

**Returns:**
boolean - यह मान दर्शाता है कि क्या फ्रेम में सामग्री का आकार शामिल किया जाए।
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि संपीड़ित ब्लॉक के अंत में संपीड़ित xxh32 हैश शामिल किया जाए या नहीं।

डिफ़ॉल्ट false है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | यह मान दर्शाता है कि क्या संकुचित ब्लॉक के अंत में संकुचित xxh32 हैश शामिल किया जाए। |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि LZ4 अभिलेख के अंत में सामग्री xxh32 हैश शामिल किया जाए या नहीं।

डिफ़ॉल्ट true है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | यह मान दर्शाता है कि क्या LZ4 संग्रह के अंत में सामग्री xxh32 हैश शामिल किया जाए। |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि फ्रेम में सामग्री का आकार शामिल किया जाए या नहीं।

डिफ़ॉल्ट मान false है। जब स्रोत स्ट्रीम seekable हो तो लागू होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | यह मान दर्शाता है कि क्या फ्रेम में सामग्री का आकार शामिल किया जाए। |

