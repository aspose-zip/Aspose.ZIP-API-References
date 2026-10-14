---
title: "GzipArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक gzip आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 69
url: /hi/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

यह क्लास एक gzip आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग gzip आर्काइव बनाने या निकालने के लिए करें।

Gzip संपीड़न एल्गोरिद्म DEFLATE एल्गोरिद्म पर आधारित है, जो LZ77 और Huffman कोडिंग का संयोजन है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | संपीड़न के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | डिकम्प्रेसिंग के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | डिकम्प्रेसिंग के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | डिकम्प्रेसिंग के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | डिकम्प्रेसिंग के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है। |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा फ़ाइल में संग्रह को निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | gzip आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | मूल फ़ाइल का आकार प्राप्त करता है। |
| [getName()](#getName--) | मूल फ़ाइल का नाम। |
| [getUncompressedSize()](#getUncompressedSize--) | मूल फ़ाइल का आकार प्राप्त करता है। |
| [open()](#open--) | निकालने के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String path)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


संपीड़न के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [open()](../../com.aspose.zip/gziparchive\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत। |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


डिकम्प्रेसिंग के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है।

स्ट्रीम से एक अभिलेख खोलें और उसे `ByteArrayOutputStream` में निकालें

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [open()](../../com.aspose.zip/gziparchive\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत। |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | आर्काइव लोड करने के विकल्प। |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


डिकम्प्रेसिंग के लिए तैयार [GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है।

फ़ाइल से पथ द्वारा एक अभिलेख खोलें और इसे `MemoryStream` में निकालें।

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [open()](../../com.aspose.zip/gziparchive\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ। |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


[GzipArchive](../../com.aspose.zip/gziparchive) क्लास का एक नया उदाहरण प्रारंभ करता है।

फ़ाइल से पथ द्वारा एक अभिलेख खोलें और इसे `MemoryStream` में निकालें।

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

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

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम। लिखने योग्य होना चाहिए। |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


पथ द्वारा फ़ाइल में संग्रह को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो उसे अधिलेखित किया जाएगा। |

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


gzip आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - gzip आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ।
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


मूल फ़ाइल का आकार प्राप्त करता है।

डिकम्प्रेशन के दौरान, इस प्रॉपर्टी में आकार गलत हो सकता है। यदि अनकम्प्रेस्ड फ़ाइल का आकार 4GB से अधिक हो जाता है, तो हेडर में 32-बिट सीमा के कारण यह प्रॉपर्टी गलत मान देगी।

**Returns:**
java.lang.Long - मूल फ़ाइल का आकार
### getName() {#getName--}
```
public final String getName()
```


मूल फ़ाइल का नाम।

**Returns:**
java.lang.String - मूल फ़ाइल का नाम
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


मूल फ़ाइल का आकार प्राप्त करता है।

डिकम्प्रेशन के दौरान, इस प्रॉपर्टी में आकार गलत हो सकता है। यदि अनकम्प्रेस्ड फ़ाइल का आकार 4GB से अधिक हो जाता है, तो हेडर में 32-बिट सीमा के कारण यह प्रॉपर्टी गलत मान देगी।

**Returns:**
long - मूल फ़ाइल का आकार।
### open() {#open--}
```
public final InputStream open()
```


निकालने के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है।

अभिलेख को निकालता है और निकाले गए सामग्री को फ़ाइल स्ट्रीम में कॉपी करता है।

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | गंतव्य स्ट्रीम। |

`outputStream` लिखने योग्य होना चाहिए। |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

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
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

इस मेथड का उपयोग संयुक्त tar.gz आर्काइव बनाने के लिए करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | कम्प्रेस करने के लिए टार आर्काइव। |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव के लिए इनपुट स्ट्रीम। |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

फ़ाइल से पथ द्वारा एक अभिलेख खोलें और इसे `MemoryStream` में निकालें।

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

