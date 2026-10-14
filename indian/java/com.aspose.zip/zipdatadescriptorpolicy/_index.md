---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "डेटा डिस्क्रिप्टर की उपस्थिति के विकल्प।"
type: docs
weight: 171
url: /hi/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

डेटा डिस्क्रिप्टर की उपस्थिति के विकल्प।
## Fields

| Field | विवरण |
| --- | --- |
| [Always](#Always) | Data Descriptor सभी zip प्रविष्टियों के लिए हमेशा मौजूद रहता है। |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor केवल फ़ाइल डेटा वाली प्रविष्टियों के लिए मौजूद है; निर्देशिकाओं के लिए छोड़ दिया गया है। |
## Methods

| Method | विवरण |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor सभी zip प्रविष्टियों के लिए हमेशा मौजूद रहता है।

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor केवल फ़ाइल डेटा वाली प्रविष्टियों के लिए मौजूद है; निर्देशिकाओं के लिए छोड़ दिया गया है। इस विकल्प का उपयोग करने की सलाह नहीं दी जाती है।

केवल गैर-एन्क्रिप्टेड अभिलेखों पर लागू किया जा सकता है।

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
