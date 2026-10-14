---
title: "UueSaveOptions"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "uuencoded फ़ाइल को सहेजने के विकल्प।"
type: docs
weight: 129
url: /hi/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

uuencoded फ़ाइल को सहेजने के विकल्प।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | उपयोगकर्ता द्वारा प्रदान किए गए फ़ाइल नाम और नई पंक्ति के साथ विकल्पों को प्रारंभ करता है। |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | उपयोगकर्ता द्वारा प्रदान किए गए फ़ाइल नाम और डिफ़ॉल्ट नई पंक्ति के साथ विकल्पों को प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getFileName()](#getFileName--) | डिकोडेड डेटा को पुनः बनाने के समय उपयोग किए जाने वाले फ़ाइल नाम को प्राप्त करता है। |
| [getNewLine()](#getNewLine--) | प्रत्येक पंक्ति को समाप्त करने वाले अक्षर को प्राप्त करता है, आमतौर पर "\n" या "\r\n"। |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | फ़ाइल की Unix फ़ाइल अनुमतियों को प्राप्त करता है। |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | फ़ाइल की Unix फ़ाइल अनुमतियों को सेट करता है। |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


उपयोगकर्ता द्वारा प्रदान किए गए फ़ाइल नाम और नई पंक्ति के साथ विकल्पों को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | डिकोड किए गए डेटा को पुनः बनाने के समय उपयोग किया जाने वाला फ़ाइल नाम |
| newLine | java.lang.String | प्रत्येक पंक्ति को समाप्त करने वाला अक्षर |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


उपयोगकर्ता द्वारा प्रदान किए गए फ़ाइल नाम और डिफ़ॉल्ट नई पंक्ति के साथ विकल्पों को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileName | java.lang.String | डिकोड किए गए डेटा को पुनः बनाने के समय उपयोग किया जाने वाला फ़ाइल नाम |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


डिकोडेड डेटा को पुनः बनाने के समय उपयोग किए जाने वाले फ़ाइल नाम को प्राप्त करता है।

**Returns:**
java.lang.String - डिकोड किए गए डेटा को पुनः बनाने के समय उपयोग किया जाने वाला फ़ाइल नाम
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


प्रत्येक पंक्ति को समाप्त करने वाले अक्षर को प्राप्त करता है, आमतौर पर "\n" या "\r\n"।

**Returns:**
java.lang.String - प्रत्येक पंक्ति को समाप्त करने वाला अक्षर, आमतौर पर "\\n" या "\\r\\n"।
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


फ़ाइल की Unix फ़ाइल अनुमतियों को प्राप्त करता है।

डिफ़ॉल्ट 644 है।

**Returns:**
java.lang.String - फ़ाइल की Unix फ़ाइल अनुमतियाँ
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


फ़ाइल की Unix फ़ाइल अनुमतियों को सेट करता है।

डिफ़ॉल्ट 644 है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | फ़ाइल की Unix फ़ाइल अनुमतियाँ |

