---
title: "LzmaArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास LZMA आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 86
url: /hi/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

यह क्लास LZMA आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग LZMA आर्काइव बनाने या निकालने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और lzma प्रारूप में आर्काइव बनाता है। |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और lzma प्रारूप में आर्काइव बनाता है। |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और डिकम्प्रेसन के लिए तैयार करता है। |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और डिकम्प्रेसन के लिए तैयार करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | lzma आर्काइव को फ़ाइल में निकालता है। |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | lzma आर्काइव को स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा lzma आर्काइव को फ़ाइल में निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो lzma आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getName()](#getName--) | मूल फ़ाइल का नाम। |
| [save(File destination)](#save-java.io.File-) | प्रदान किए गए गंतव्य फ़ाइल में lzma आर्काइव सहेजता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में lzma आर्काइव को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | प्रदान किए गए गंतव्य फ़ाइल में lzma आर्काइव सहेजता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और lzma प्रारूप में आर्काइव बनाता है।

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और lzma प्रारूप में आर्काइव बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | विशिष्ट lzma आर्काइव की सेटिंग का सेट |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और डिकम्प्रेसन के लिए तैयार करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


डिफ़ॉल्ट पैरामीटरों के साथ [LzmaArchive](../../com.aspose.zip/lzmaarchive) क्लास का नया उदाहरण प्रारंभ करता है और डिकम्प्रेसन के लिए तैयार करता है।

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइल | java.io.File | डिकम्प्रेस्ड डेटा को संग्रहीत करने के लिए फ़ाइल |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


lzma आर्काइव को स्ट्रीम में निकालता है।

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | फ़ाइल का पथ जहाँ डिकम्प्रेस्ड डेटा संग्रहीत होगा |

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


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो lzma आर्काइव बनाती हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियाँ जो lzma आर्काइव बनाती हैं।
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
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


प्रदान किए गए गंतव्य फ़ाइल में lzma आर्काइव सहेजता है।

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lzma\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


प्रदान किए गए गंतव्य फ़ाइल में lzma आर्काइव सहेजता है।

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइल | java.io.File | फ़ाइल, जिसे इनपुट स्ट्रीम के रूप में खोला जाएगा |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save(\"archive.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourcePath | java.lang.String | फ़ाइल का पथ, जिसे इनपुट स्ट्रीम के रूप में खोला जाएगा |

