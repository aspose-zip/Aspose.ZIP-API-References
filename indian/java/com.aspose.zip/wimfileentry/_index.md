---
title: "WimFileEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "wim संग्रह के भीतर एकल फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 133
url: /hi/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

wim संग्रह के भीतर एकल फ़ाइल का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [open()](#open--) | निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

wim अभिलेख की एक प्रविष्टि को निकालें।

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract(httpResponseStream);
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

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract("data.bin");
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
### open() {#open--}
```
public final InputStream open()
```


निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है।

उपयोग:

```

``````

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
