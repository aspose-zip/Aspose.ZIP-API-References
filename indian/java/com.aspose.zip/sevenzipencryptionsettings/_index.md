---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "कई 7z एन्क्रिप्शन विधियों की सेटिंग्स के लिए बेस क्लास।"
type: docs
weight: 112
url: /hi/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

कई 7z एन्क्रिप्शन विधियों की सेटिंग्स के लिए बेस क्लास।

AES-256 7z अभिलेख के लिए एकमात्र संभव एन्क्रिप्शन विधि है। इसलिए [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) एकमात्र कार्यान्वयन है।
## Methods

| Method | विवरण |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | हेडर एन्क्रिप्शन को दर्शाने वाला मान प्राप्त करता है। |
| [getPassword()](#getPassword--) | एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड प्राप्त करता है। |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | हेडर एन्क्रिप्शन को दर्शाने वाला मान सेट करता है। |
| [setPassword(String value)](#setPassword-java.lang.String-) | एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड सेट करता है। |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


हेडर एन्क्रिप्शन को दर्शाने वाला मान प्राप्त करता है।

यह सेटिंग 7-Zip टूल के `-mhe=on` स्विच के समान है। वर्तमान में, यह हेडर संपीड़न के साथ असंगत है।

**Returns:**
boolean - हेडर एन्क्रिप्शन को दर्शाने वाला मान
### getPassword() {#getPassword--}
```
public final String getPassword()
```


एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड प्राप्त करता है।

**Returns:**
java.lang.String - एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


हेडर एन्क्रिप्शन को दर्शाने वाला मान सेट करता है।

यह सेटिंग 7-Zip टूल के `-mhe=on` स्विच के समान है। वर्तमान में, यह हेडर संपीड़न के साथ असंगत है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | हेडर एन्क्रिप्शन को दर्शाने वाला मान |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.lang.String | एन्क्रिप्शन या डिक्रिप्शन के लिए पासवर्ड |

