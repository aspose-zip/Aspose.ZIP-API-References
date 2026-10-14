---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ARJ अभिलेख के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 38
url: /hi/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

ARJ अभिलेख के भीतर एक एकल फ़ाइल का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | ARJ आर्काइव प्रविष्टि को फ़ाइल में निकालता है। |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getCompressedSize()](#getCompressedSize--) | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getName()](#getName--) | अभिलेख के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | मूल फ़ाइल का आकार प्राप्त करता है। |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


ARJ आर्काइव प्रविष्टि को फ़ाइल में निकालता है।

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो इसे अधिलेखित किया जाएगा। |

**Returns:**
java.io.File - संयुक्त फ़ाइल की फ़ाइल जानकारी
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


संपीड़ित फ़ाइल का आकार प्राप्त करता है।

**Returns:**
long - संपीड़ित फ़ाइल का आकार
### getLength() {#getLength--}
```
public final Long getLength()
```


प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है।

**Returns:**
java.lang.Long - प्रविष्टि की लंबाई बाइट्स में
### getName() {#getName--}
```
public final String getName()
```


अभिलेख के भीतर प्रविष्टि का नाम प्राप्त करता है।

**Returns:**
java.lang.String - अभिलेख में प्रविष्टि का नाम
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


मूल फ़ाइल का आकार प्राप्त करता है।

**Returns:**
long - मूल फ़ाइल का आकार
