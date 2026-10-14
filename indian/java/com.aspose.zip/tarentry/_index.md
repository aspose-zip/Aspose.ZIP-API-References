---
title: "TarEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "tar संग्रह के भीतर एकल फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 126
url: /hi/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

tar संग्रह के भीतर एकल फ़ाइल का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | फ़ाइल या निर्देशिका का संशोधन समय प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | मूल फ़ाइल का आकार प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं। |
| [open()](#open--) | निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [setName(String value)](#setName-java.lang.String-) | आर्काइव के भीतर प्रविष्टि का नाम सेट करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

टार आर्काइव की एक प्रविष्टि निकालें।

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो इसे अधिलेखित किया जाएगा। |

**Returns:**
java.io.File - निकाली गई फ़ाइल की फ़ाइल जानकारी
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


फ़ाइल या निर्देशिका का संशोधन समय प्राप्त करता है।

**Returns:**
java.util.Date - फ़ाइल या निर्देशिका का संशोधन समय।
### getName() {#getName--}
```
public final String getName()
```


आर्काइव के भीतर प्रविष्टि का नाम प्राप्त करता है।

**Returns:**
java.lang.String - आर्काइव के भीतर प्रविष्टि का नाम
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


मूल फ़ाइल का आकार प्राप्त करता है।

`Length`([getLength](../../com.aspose.zip/tarentry\#getLength--)) के समान मान रखता है।

**Returns:**
long - मूल फ़ाइल का आकार।
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं।

**Returns:**
boolean - यह दर्शाने वाला मान कि प्रविष्टि एक निर्देशिका का प्रतिनिधित्व करती है या नहीं
### open() {#open--}
```
public final InputStream open()
```


निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है।


उपयोग:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

