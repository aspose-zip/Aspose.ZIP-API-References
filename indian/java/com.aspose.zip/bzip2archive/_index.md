---
title: "Bzip2Archive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास bzip2 अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 40
url: /hi/java/com.aspose.zip/bzip2archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Bzip2Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

यह क्लास bzip2 अभिलेख फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग bzip2 अभिलेखों को बनाने या निकालने के लिए करें।

bzip2 फ़ाइलों को Burrows-Wheeler ब्लॉक सॉर्टिंग टेक्स्ट कंप्रेशन एल्गोरिदम और Huffman कोडिंग का उपयोग करके संपीड़ित करता है। और अधिक देखें: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Bzip2Archive()](#Bzip2Archive--) | संपीड़न के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [Bzip2Archive(InputStream sourceStream)](#Bzip2Archive-java.io.InputStream-) | डिकम्प्रेशन के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-) | डिकम्प्रेशन के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [Bzip2Archive(String path)](#Bzip2Archive-java.lang.String-) | डिकम्प्रेशन के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [Bzip2Archive(String path, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-) | डिकम्प्रेशन के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा फ़ाइल में संग्रह को निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है जो bzip2 अभिलेख बनाते हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getName()](#getName--) | मूल फ़ाइल का नाम। |
| [open()](#open--) | निकालने के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream outputStream, Bzip2SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, Bzip2SaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [setSource(CpioArchive cpioArchive)](#setSource-com.aspose.zip.CpioArchive-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(CpioArchive cpioArchive, CpioFormat format)](#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String path)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### Bzip2Archive() {#Bzip2Archive--}
```
public Bzip2Archive()
```


संपीड़न के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save("archive.bz2");
}
 
```



### Bzip2Archive(InputStream sourceStream) {#Bzip2Archive-java.io.InputStream-}
```
public Bzip2Archive(InputStream sourceStream)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
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

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [open()](../../com.aspose.zip/bzip2archive\#open--) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)
```


डिकम्प्रेशन के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है।

स्ट्रीम से एक अभिलेख खोलें और उसे `ByteArrayOutputStream` में निकालें

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
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

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

### Bzip2Archive(String path) {#Bzip2Archive-java.lang.String-}
```
public Bzip2Archive(String path)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
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

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [open()](../../com.aspose.zip/bzip2archive\#open--) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

### Bzip2Archive(String path, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(String path, Bzip2LoadOptions loadOptions)
```


डिकम्प्रेशन के लिए तैयार [Bzip2Archive](../../com.aspose.zip/bzip2archive) क्लास का नया उदाहरण प्रारंभ करता है।

फ़ाइल से पथ द्वारा एक अभिलेख खोलें और इसे `MemoryStream` में निकालें।

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
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

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

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

     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
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
|  | destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाली निर्देशिका का पथ। |

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा। |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है जो bzip2 अभिलेख बनाते हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ जो bzip2 अभिलेख बनाती हैं
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


निकालने के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है।


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
System.out.println(ex);
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

Write compressed data to an output stream.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | java.io.OutputStream | गंतव्य स्ट्रीम। |

### save(OutputStream outputStream, Bzip2SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(OutputStream outputStream, Bzip2SaveOptions saveOptions)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

संपीड़ित डेटा को आउटपुट स्ट्रीम में लिखें।

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream. |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

Writes compressed data to file.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bz2");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### save(String destinationFileName, Bzip2SaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(String destinationFileName, Bzip2SaveOptions saveOptions)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

संपीड़ित डेटा को फ़ाइल में लिखता है।

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### setSource(CpioArchive cpioArchive) {#setSource-com.aspose.zip.CpioArchive-}
```
public final void setSource(CpioArchive cpioArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (CpioArchive cpioArchive = new CpioArchive()) {
         cpioArchive.createEntry("first.bin", "data1.bin");
         cpioArchive.createEntry("second.bin", "data2.bin");
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(cpioArchive);
             bzippedArchive.save("archive.cpio.bz2");
         }
     }
 
```

इस विधि का उपयोग संयुक्त cpio.bz2 अभिलेख बनाने के लिए करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | संपीड़ित करने के लिए cpio अभिलेख |

### setSource(CpioArchive cpioArchive, CpioFormat format) {#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-}
```
public final void setSource(CpioArchive cpioArchive, CpioFormat format)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (CpioArchive cpioArchive = new CpioArchive()) {
cpioArchive.createEntry("first.bin", "data1.bin");
cpioArchive.createEntry("second.bin", "data2.bin");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(cpioArchive);
bzippedArchive.save("archive.cpio.bz2");
}
}
 
```

Use this method to compose joint cpio.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | cpio archive to be compressed |
| format | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(tarArchive);
             bzippedArchive.save("archive.tar.bz2");
         }
     }
 
```

इस विधि का उपयोग संयुक्त tar.bz2 अभिलेख बनाने के लिए करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | संपीड़ित करने के लिए tar अभिलेख |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(tarArchive);
bzippedArchive.save("archive.tar.bz2");
}
}
 
```

Use this method to compose joint tar.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | tar archive to be compressed |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.bz2");
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

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.bz2");
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

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | संपीड़ित करने के लिए फ़ाइल का पथ |

