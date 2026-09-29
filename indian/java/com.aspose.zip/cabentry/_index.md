---
title: "CabEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "cab अभिलेख के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 46
url: /hi/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

cab अभिलेख के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | अंतिम संशोधित तिथि और समय प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [open()](#open--) | निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [toString()](#toString--) | इंस्टेंस का स्ट्रिंग प्रतिनिधित्व लौटाता है [CabEntry](../../com.aspose.zip/cabentry) क्लास का। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

CAB आर्काइव की एक प्रविष्टि निकालें।

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो इसे अधिलेखित किया जाएगा। |

**Returns:**
java.io.File - एक संयुक्त फ़ाइल की फ़ाइल जानकारी
### getLength() {#getLength--}
```
public final Long getLength()
```


प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है।

**Returns:**
java.lang.Long - प्रविष्टि की लंबाई बाइट्स में
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


अंतिम संशोधित तिथि और समय प्राप्त करता है।

**Returns:**
java.util.Date - अंतिम संशोधित तिथि और समय।
### getName() {#getName--}
```
public final String getName()
```


आर्काइव के भीतर प्रविष्टि का नाम प्राप्त करता है।

**Returns:**
java.lang.String - आर्काइव के भीतर प्रविष्टि का नाम
### open() {#open--}
```
public final InputStream open()
```


निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है।

उपयोग:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
