---
title: "IsoEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ISO आर्काइव के भीतर एक प्रविष्टि फ़ाइल या निर्देशिका का प्रतिनिधित्व करता है।"
type: docs
weight: 72
url: /hi/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

ISO आर्काइव के भीतर एक एंट्री (फ़ाइल या डायरेक्टरी) का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | अंतिम संशोधित तिथि और समय प्राप्त करता है। |
| [getName()](#getName--) | प्रविष्टि का नाम प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टि एक निर्देशिका है या नहीं। |
| [toString()](#toString--) | वर्तमान प्रविष्टि का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
```


प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो इसे अधिलेखित किया जाएगा। |

**Returns:**
java.io.File - निकाले गए डेटा को समाहित करने वाला java.io.File इंस्टेंस
### getLength() {#getLength--}
```
public Long getLength()
```


प्रविष्टि की लंबाई प्राप्त करता है।

**Returns:**
java.lang.Long - प्रविष्टि की लंबाई
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


अंतिम संशोधित तिथि और समय प्राप्त करता है।

**Returns:**
java.util.Date - अंतिम संशोधित तिथि और समय
### getName() {#getName--}
```
public final String getName()
```


प्रविष्टि का नाम प्राप्त करता है।

**Returns:**
java.lang.String - प्रविष्टि का नाम
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


एक मान प्राप्त करता है जो दर्शाता है कि प्रविष्टि एक निर्देशिका है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि प्रविष्टि एक निर्देशिका का प्रतिनिधित्व करती है या नहीं
### toString() {#toString--}
```
public String toString()
```


वर्तमान प्रविष्टि का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है।

**Returns:**
java.lang.String - प्रविष्टि का नाम
