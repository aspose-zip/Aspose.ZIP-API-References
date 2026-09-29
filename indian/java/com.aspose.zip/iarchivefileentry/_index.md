---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह इंटरफ़ेस एक अभिलेख फ़ाइल प्रविष्टि का प्रतिनिधित्व करता है।"
type: docs
weight: 162
url: /hi/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

यह इंटरफ़ेस एक अभिलेख फ़ाइल प्रविष्टि का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getName()](#getName--) | प्रविष्टि का नाम प्राप्त करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम। लिखने योग्य होना चाहिए |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
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
public abstract Long getLength()
```


प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है।

**Returns:**
java.lang.Long - प्रविष्टि की लंबाई बाइट्स में
### getName() {#getName--}
```
public abstract String getName()
```


प्रविष्टि का नाम प्राप्त करता है।

संकुचन के लिए केवल अभिलेख, जैसे gzip, bzip2, lzip, lzma, xz, z का नाम "File.bin" होता है जब तक हेडर में कोई अन्य नाम न मिले।

**Returns:**
java.lang.String - प्रविष्टि का नाम
