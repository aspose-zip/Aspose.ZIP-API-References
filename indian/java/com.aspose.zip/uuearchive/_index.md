---
title: "UueArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह वर्ग uuencoded फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 128
url: /hi/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

यह वर्ग uuencoded फ़ाइल का प्रतिनिधित्व करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [UueArchive()](#UueArchive--) | एन्कोडिंग के लिए तैयार [UueArchive](../../com.aspose.zip/uuearchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | डिकोडिंग के लिए तैयार [UueArchive](../../com.aspose.zip/uuearchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | [UueArchive](../../com.aspose.zip/uuearchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा फ़ाइल में संग्रह को निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है जो uue संग्रह बनाते हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getName()](#getName--) | मूल फ़ाइल का नाम। |
| [open()](#open--) | डिकोडिंग के लिए संग्रह खोलता है और संग्रह सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | प्रदान किए गए लक्ष्य फ़ाइल में संग्रह को सहेजता है। |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | प्रदान किए गए लक्ष्य फ़ाइल में संग्रह को सहेजता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | संग्रह के भीतर एन्कोड की जाने वाली सामग्री सेट करता है। |
| [setSource(String path)](#setSource-java.lang.String-) | संग्रह के भीतर एन्कोड की जाने वाली सामग्री सेट करता है। |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


एन्कोडिंग के लिए तैयार [UueArchive](../../com.aspose.zip/uuearchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

निम्न उदाहरण दिखाता है कि फ़ाइल को uuencode कैसे किया जाता है।

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource("data.bin");
archive.save("archive.uue");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर डिकोड नहीं करता है। डिकम्प्रेस करने के लिए [open()](../../com.aspose.zip/uuearchive\#open--) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


[UueArchive](../../com.aspose.zip/uuearchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

फ़ाइल पथ से एक संग्रह खोलें और उसे `MemoryStream` में डिकोड करें।

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream("archive.uue"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


पथ द्वारा फ़ाइल में संग्रह को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो इसे अधिलेखित किया जाएगा। |

**Returns:**
java.io.File - निकाली गई फ़ाइल की जानकारी
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाले डायरेक्टरी का पथ। |

यदि डायरेक्टरी मौजूद नहीं है, तो इसे बनाया जाएगा |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है जो uue संग्रह बनाते हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियाँ जो uue संग्रह बनाते हैं
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


लंबाई प्राप्त करता है।

**Returns:**
java.lang.Long - लंबाई
### getName() {#getName--}
```
public final String getName()
```


मूल फ़ाइल का नाम।

**Returns:**
java.lang.String - मूल फ़ाइल का नाम
### open() {#open--}
```
public final InputStream open()
```


डिकोडिंग के लिए संग्रह खोलता है और संग्रह सामग्री के साथ एक स्ट्रीम प्रदान करता है।

उपयोग:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | java.io.OutputStream | गंतव्य स्ट्रीम |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

संपीड़ित डेटा को http प्रतिक्रिया स्ट्रीम में लिखें।

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


प्रदान किए गए लक्ष्य फ़ाइल में संग्रह को सहेजता है।

फ़ाइल में एन्कोडेड डेटा लिखें।

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइल | java.io.File | संपीड़ित की जाने वाली फ़ाइल का संदर्भ |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


संग्रह के भीतर एन्कोड की जाने वाली सामग्री सेट करता है।

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save("archive.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | एन्कोड की जाने वाली फ़ाइल का पथ |

