---
title: "XzArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास xz अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 146
url: /hi/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

यह क्लास xz आर्काइव फ़ाइल का प्रतिनिधित्व करती है। xz आर्काइव को बनाने और निकालने के लिए इसका उपयोग करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [XzArchive()](#XzArchive--) | नया इंस्टेंस [XzArchive](../../com.aspose.zip/xzarchive) क्लास का प्रारंभ करता है और आर्काइव को xz फ़ॉर्मेट में बनाता है। |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | नया इंस्टेंस [XzArchive](../../com.aspose.zip/xzarchive) क्लास का प्रारंभ करता है और आर्काइव को xz फ़ॉर्मेट में बनाता है। |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है। |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | xz आर्काइव को फ़ाइल में निकालता है। |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | xz आर्काइव को स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा xz आर्काइव को फ़ाइल में निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | xz अभिलेख बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर एंट्री का नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | फ़ाइल डेटा का अनकम्प्रेस्ड आकार बाइट्स में प्राप्त करता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में xz अभिलेख को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | प्रदान की गई गंतव्य फ़ाइल में xz अभिलेख को सहेजता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


नया इंस्टेंस [XzArchive](../../com.aspose.zip/xzarchive) क्लास का प्रारंभ करता है और आर्काइव को xz फ़ॉर्मेट में बनाता है।

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


नया इंस्टेंस [XzArchive](../../com.aspose.zip/xzarchive) क्लास का प्रारंभ करता है और आर्काइव को xz फ़ॉर्मेट में बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | विशिष्ट xz आर्काइव की सेटिंग्स का सेट: शब्दकोश आकार, ब्लॉक आकार, जांच प्रकार |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | आर्काइव लोड करने के विकल्प। |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | अभिलेख के स्रोत का पथ |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


डिकम्प्रेस करने के लिए तैयार [XzArchive](../../com.aspose.zip/xzarchive) क्लास का नया इंस्टेंस प्रारंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | अभिलेख के स्रोत का पथ |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


xz आर्काइव को फ़ाइल में निकालता है।

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | डिकम्प्रेस्ड डेटा को संग्रहीत करने के लिए स्ट्रीम |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


पथ द्वारा xz आर्काइव को फ़ाइल में निकालता है।

```

``````

try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


प्रदान की गई गंतव्य फ़ाइल में xz अभिलेख को सहेजता है।

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("result.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
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

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourcePath | java.lang.String | फ़ाइल का पथ जिसे इनपुट स्ट्रीम के रूप में खोला जाएगा |

