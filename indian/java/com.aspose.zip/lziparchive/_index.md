---
title: "LzipArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक Lzip आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 83
url: /hi/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

यह क्लास एक Lzip आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग Lzip आर्काइव बनाने या निकालने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | नया उदाहरण प्रारंभ करता है [LzipArchive](../../com.aspose.zip/lziparchive) का। |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | नया उदाहरण प्रारंभ करता है [LzipArchive](../../com.aspose.zip/lziparchive) का। |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | डिकम्प्रेसिंग के लिए तैयार [LzipArchive](../../com.aspose.zip/lziparchive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | डिकम्प्रेसिंग के लिए तैयार [LzipArchive](../../com.aspose.zip/lziparchive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | डिकम्प्रेसिंग के लिए तैयार [LzipArchive](../../com.aspose.zip/lziparchive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | डिकम्प्रेसिंग के लिए तैयार [LzipArchive](../../com.aspose.zip/lziparchive) क्लास का नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | lzip अभिलेख को फ़ाइल में निकालता है। |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | lzip अभिलेख को स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा lzip अभिलेख को फ़ाइल में निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | lzip अभिलेख को बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getName()](#getName--) | मूल फ़ाइल का नाम। |
| [getSettings()](#getSettings--) | विशिष्ट lzip अभिलेख की सेटिंग प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | फ़ाइल डेटा का अनकम्प्रेस्ड आकार बाइट्स में प्राप्त करता है। |
| [save(File destination)](#save-java.io.File-) | प्रदान की गई गंतव्य फ़ाइल में lzip अभिलेख को सहेजता है। |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | प्रदान की गई स्ट्रीम में lzip अभिलेख को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | प्रदान की गई गंतव्य फ़ाइल में lzip अभिलेख को सहेजता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String path)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


नया उदाहरण प्रारंभ करता है [LzipArchive](../../com.aspose.zip/lziparchive) का।

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


नया उदाहरण प्रारंभ करता है [LzipArchive](../../com.aspose.zip/lziparchive) का।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | विशिष्ट lzip अभिलेख की सेटिंग, शब्दकोश आकार की परिभाषा के साथ |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


डिकम्प्रेसिंग के लिए तैयार [LzipArchive](../../com.aspose.zip/lziparchive) क्लास का नया उदाहरण प्रारंभ करता है।

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | आर्काइव लोड करने के विकल्प। |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


डिकम्प्रेसिंग के लिए तैयार [LzipArchive](../../com.aspose.zip/lziparchive) क्लास का नया उदाहरण प्रारंभ करता है।

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव के स्रोत का पथ |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | आर्काइव लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


lzip अभिलेख को फ़ाइल में निकालता है।

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
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


पथ द्वारा lzip अभिलेख को फ़ाइल में निकालता है।

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
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


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.File | फ़ाइल, जिसे गंतव्य स्ट्रीम के रूप में खोला जाएगा |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


प्रदान की गई स्ट्रीम में lzip अभिलेख को सहेजता है।

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव के लिए इनपुट स्ट्रीम |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

