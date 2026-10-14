---
title: "CabEntrySettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "CAB प्रविष्टि को लिखने के तरीके को नियंत्रित करने वाली सेटिंग्स।"
type: docs
weight: 47
url: /hi/java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

CAB प्रविष्टि को लिखने के तरीके को नियंत्रित करने वाली सेटिंग्स।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | विशिष्ट संपीड़न प्रोफ़ाइल के साथ सेटिंग्स को प्रारंभ करता है। |
| [CabEntrySettings()](#CabEntrySettings--) | डिफ़ॉल्ट MSZip संपीड़न के साथ सेटिंग्स को प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | एंट्री पर लागू संपीड़न कॉन्फ़िगरेशन प्राप्त करता है। |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


विशिष्ट संपीड़न प्रोफ़ाइल के साथ सेटिंग्स को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | उपयोग करने के लिए संपीड़न सेटिंग्स। |

इनमें से कोई एक हो सकता है: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


डिफ़ॉल्ट MSZip संपीड़न के साथ सेटिंग्स को प्रारंभ करता है।

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


एंट्री पर लागू संपीड़न कॉन्फ़िगरेशन प्राप्त करता है।

इनमें से एक हो सकता है:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
