---
title: "AlzEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "एक ALZ अभिलेख में फ़ाइल प्रविष्टि को उसके मेटाडेटा के साथ प्रतिनिधित्व करता है।"
type: docs
weight: 13
url: /hi/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

एक ALZ अभिलेख में फ़ाइल प्रविष्टि को उसके मेटाडेटा के साथ प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | एंट्री को लिखने योग्य स्ट्रीम में एक्सट्रैक्ट करता है। |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | वैकल्पिक पासवर्ड का उपयोग करके एंट्री को लिखने योग्य स्ट्रीम में एक्सट्रैक्ट करता है। |
| [extract(String path)](#extract-java.lang.String-) | एंट्री को निर्दिष्ट फ़ाइल में एक्सट्रैक्ट करता है। |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | वैकल्पिक पासवर्ड का उपयोग करके एंट्री को निर्दिष्ट फ़ाइल में एक्सट्रैक्ट करता है। |
| [getCompressedSize()](#getCompressedSize--) | एंट्री डेटा के संकुचित आकार को बाइट्स में प्राप्त करता है। |
| [getLength()](#getLength--) | इस एंट्री की अनकम्प्रेस्ड लंबाई प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव में संग्रहीत एंट्री नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | एंट्री डेटा के अनकम्प्रेस्ड आकार को बाइट्स में प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | क्या यह एंट्री एक डायरेक्टरी का प्रतिनिधित्व करती है, यह प्राप्त करता है। |
| [open()](#open--) | एंट्री को खोलता है और डिकम्प्रेस्ड डेटा वाली स्ट्रीम प्रदान करता है। |
| [open(String password)](#open-java.lang.String-) | एंट्री को खोलता है और डिकम्प्रेस्ड डेटा वाली स्ट्रीम प्रदान करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


एंट्री को लिखने योग्य स्ट्रीम में एक्सट्रैक्ट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


वैकल्पिक पासवर्ड का उपयोग करके एंट्री को लिखने योग्य स्ट्रीम में एक्सट्रैक्ट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम |
| पासवर्ड | java.lang.String | इस एंट्री के लिए वैकल्पिक पासवर्ड |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


एंट्री को निर्दिष्ट फ़ाइल में एक्सट्रैक्ट करता है। मौजूदा फ़ाइल को ओवरराइट किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल पथ |

**Returns:**
java.io.File - निकाली गई फ़ाइल
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


वैकल्पिक पासवर्ड का उपयोग करके एंट्री को निर्दिष्ट फ़ाइल में एक्सट्रैक्ट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल पथ |
| पासवर्ड | java.lang.String | इस एंट्री के लिए वैकल्पिक पासवर्ड |

**Returns:**
java.io.File - निकाली गई फ़ाइल
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


एंट्री डेटा के संकुचित आकार को बाइट्स में प्राप्त करता है।

**Returns:**
long - बाइट्स में संकुचित आकार
### getLength() {#getLength--}
```
public final Long getLength()
```


इस एंट्री की अनकम्प्रेस्ड लंबाई प्राप्त करता है।

**Returns:**
java.lang.Long - बाइट्स में असंकुचित लंबाई
### getName() {#getName--}
```
public final String getName()
```


आर्काइव में संग्रहीत एंट्री नाम प्राप्त करता है।

**Returns:**
java.lang.String - प्रविष्टि नाम
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


एंट्री डेटा के अनकम्प्रेस्ड आकार को बाइट्स में प्राप्त करता है।

**Returns:**
long - बाइट्स में असंकुचित आकार
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


क्या यह एंट्री एक डायरेक्टरी का प्रतिनिधित्व करती है, यह प्राप्त करता है।

**Returns:**
boolean - निर्देशिका प्रविष्टि के लिए `true`
### open() {#open--}
```
public final InputStream open()
```


एंट्री को खोलता है और डिकम्प्रेस्ड डेटा वाली स्ट्रीम प्रदान करता है।

**Returns:**
java.io.InputStream - प्रविष्टि डेटा को डिकम्प्रेस्ड करने वाली स्ट्रीम
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


एंट्री को खोलता है और डिकम्प्रेस्ड डेटा वाली स्ट्रीम प्रदान करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| पासवर्ड | java.lang.String | इस एंट्री के लिए वैकल्पिक पासवर्ड |

**Returns:**
java.io.InputStream - प्रविष्टि डेटा को डिकम्प्रेस्ड करने वाली स्ट्रीम
