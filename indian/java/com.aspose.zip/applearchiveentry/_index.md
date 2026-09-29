---
title: "AppleArchiveEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "एक फ़ाइल या निर्देशिका प्रविष्टि का प्रतिनिधित्व करता है।"
type: docs
weight: 17
url: /hi/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

एक फ़ाइल या निर्देशिका प्रविष्टि का प्रतिनिधित्व करता है जो [AppleArchive](../../com.aspose.zip/applearchive) के भीतर है।

इस क्लास का एक उदाहरण या तो मौजूदा Apple Archive से पार्स की गई प्रविष्टि या निर्मित हो रहे आर्काइव में जोड़ी गई प्रविष्टि का प्रतिनिधित्व कर सकता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | Apple आर्काइव प्रविष्टि को पथ द्वारा फ़ाइल सिस्टम में निकालता है। |
| [getLength()](#getLength--) | प्रविष्टि की अनकम्प्रेस्ड लंबाई बाइट्स में प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर प्रविष्टि का पथ प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं। |
| [open()](#open--) | निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम। लिखने योग्य होना चाहिए |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Apple आर्काइव प्रविष्टि को पथ द्वारा फ़ाइल सिस्टम में निकालता है।

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
