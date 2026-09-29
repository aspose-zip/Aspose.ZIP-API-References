---
title: "ZstandardArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास Zstandard अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 156
url: /hi/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

यह क्लास Zstandard आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग Zstandard आर्काइव बनाने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | संपीड़न के लिए तैयार [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | डिकम्प्रेशन के लिए तैयार [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | डिकम्प्रेशन के लिए तैयार [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | नए [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की इंस्टेंस को इनिशियलाइज़ करता है। |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | नए [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की इंस्टेंस को इनिशियलाइज़ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा फ़ाइल में संग्रह को निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ प्राप्त करता है जो zstandard आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर एंट्री का नाम प्राप्त करता है। |
| [open()](#open--) | निकालने के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [save(File destination)](#save-java.io.File-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String path)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


संपीड़न के लिए तैयार [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource("data.bin");
archive.save(\"archive.zst\");
}
 
```



### ZstandardArchive(InputStream sourceStream) {#ZstandardArchive-java.io.InputStream-}
```
public ZstandardArchive(InputStream sourceStream)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

यह कन्स्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [open()](../../com.aspose.zip/zstandardarchive\#open--) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


डिकम्प्रेशन के लिए तैयार [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।

स्ट्रीम से एक अभिलेख खोलें और उसे `ByteArrayOutputStream` में निकालें

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream(\"archive.zst\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### ZstandardArchive(String path) {#ZstandardArchive-java.lang.String-}
```
public ZstandardArchive(String path)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class.

Open an archive from file by path and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

यह कन्स्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [open()](../../com.aspose.zip/zstandardarchive\#open--) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


नए [ZstandardArchive](../../com.aspose.zip/zstandardarchive) क्लास की इंस्टेंस को इनिशियलाइज़ करता है।

फ़ाइल पथ से एक अभिलेख खोलें और उसे `ByteArrayOutputStream` में निकालें

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(\"archive.zst\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

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

     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम। लिखने योग्य होना चाहिए |

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
java.io.File - निकाली गई फ़ाइल की फ़ाइल जानकारी
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


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ प्राप्त करता है जो zstandard आर्काइव बनाती हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - zstandard अभिलेख बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ
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


प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है।

**Returns:**
java.lang.Long - प्रविष्टि की लंबाई बाइट्स में
### getName() {#getName--}
```
public final String getName()
```


आर्काइव के भीतर एंट्री का नाम प्राप्त करता है।

**Returns:**
java.lang.String - अभिलेख के भीतर प्रविष्टि का नाम
### open() {#open--}
```
public final InputStream open()
```


निकालने के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है।

अभिलेख को निकालता है और निकाले गए सामग्री को फ़ाइल स्ट्रीम में कॉपी करता है।

```

``````

try (ZstandardArchive archive = new ZstandardArchive(\"archive.zst\")) {
try (FileOutputStream extracted = new FileOutputStream(\"data.bin\")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.zst"));
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.File | फ़ाइल जिसे गंतव्य स्ट्रीम के रूप में खोला जाएगा |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.zst\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | java.io.OutputStream | गंतव्य स्ट्रीम |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

संपीड़ित डेटा को http प्रतिक्रिया स्ट्रीम में लिखें।

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | the destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.zst");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.zst\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.zst");
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


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save(\"archive.zst\");
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


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | संपीड़ित करने के लिए फ़ाइल का पथ |

