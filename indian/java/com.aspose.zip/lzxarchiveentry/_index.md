---
title: "LzxArchiveEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "LZX आर्काइव के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 90
url: /hi/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

LZX आर्काइव के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | Lzx आर्काइव एंट्री को पथ द्वारा फ़ाइल सिस्टम में निकालता है। |
| [getCommentary()](#getCommentary--) | टिप्पणी प्राप्त करता है। |
| [getCompressedSize()](#getCompressedSize--) | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | प्रविष्टि का अंतिम संशोधित समय प्राप्त करता है। |
| [getName()](#getName--) | प्रविष्टि का नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | मूल फ़ाइल का आकार प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | एक मान प्राप्त करता है जो दर्शाता है कि यह प्रविष्टि निर्देशिका है या नहीं। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम। लिखने योग्य होना चाहिए। |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Lzx आर्काइव एंट्री को पथ द्वारा फ़ाइल सिस्टम में निकालता है।

```

``````

try (FileInputStream lzxFile = new FileInputStream("archive.lzx")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
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
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
