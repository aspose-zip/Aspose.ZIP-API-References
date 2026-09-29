---
title: "LhaArchiveEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "Lha आर्काइव के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 76
url: /hi/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Lha आर्काइव के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Lha अभिलेख प्रविष्टि को फ़ाइल में निकालता है। |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | Lha अभिलेख प्रविष्टि को पथ द्वारा फ़ाइल प्रणाली में निकालता है। |
| [getLastModified()](#getLastModified--) | प्रविष्टि का अंतिम संशोधित समय प्राप्त करता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | प्रविष्टि का अंतिम संशोधित समय प्राप्त करता है। |
| [getName()](#getName--) | प्रविष्टि का नाम प्राप्त करता है। |
| [getPath()](#getPath--) | प्रविष्टि का पूर्ण पथ प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | एक मान प्राप्त करता है जो दर्शाता है कि यह प्रविष्टि निर्देशिका है या नहीं। |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Lha अभिलेख प्रविष्टि को फ़ाइल में निकालता है।

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | फ़ाइल का पथ जहाँ डिकम्प्रेस्ड डेटा संग्रहीत होगा |

**Returns:**
java.io.File - निकाले गए डेटा को समाहित करने वाला java.io.File इंस्टेंस
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


प्रविष्टि का अंतिम संशोधित समय प्राप्त करता है।

**Returns:**
java.util.Date - प्रविष्टि का अंतिम संशोधित समय
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


प्रविष्टि का अंतिम संशोधित समय प्राप्त करता है।

**Returns:**
java.util.Date - प्रविष्टि का अंतिम संशोधित समय
### getName() {#getName--}
```
public final String getName()
```


प्रविष्टि का नाम प्राप्त करता है।

संकुचन के लिए केवल अभिलेख, जैसे gzip, bzip2, lzip, lzma, xz, z का नाम "File.bin" होता है जब तक हेडर में कोई अन्य नाम न मिले।

**Returns:**
java.lang.String - प्रविष्टि का नाम
### getPath() {#getPath--}
```
public final String getPath()
```


प्रविष्टि का पूर्ण पथ प्राप्त करता है।

**Returns:**
java.lang.String - प्रविष्टि का पूर्ण पथ
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


एक मान प्राप्त करता है जो दर्शाता है कि यह प्रविष्टि निर्देशिका है या नहीं।

**Returns:**
boolean - एक मान जो दर्शाता है कि यह प्रविष्टि निर्देशिका है या नहीं।
