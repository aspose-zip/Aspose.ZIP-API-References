---
title: "SnappyArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह वर्ग एक snappy संग्रह फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 121
url: /hi/java/com.aspose.zip/snappyarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class SnappyArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

यह क्लास एक स्नैपी अभिलेख फ़ाइल का प्रतिनिधित्व करती है। स्नैपी अभिलेखों को बनाने या निकालने के लिए इसका उपयोग करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SnappyArchive()](#SnappyArchive--) | [SnappyArchive](../../com.aspose.zip/snappyarchive) क्लास का नया उदाहरण प्रारंभ करता है जो संपीड़न के लिए तैयार है। |
| [SnappyArchive(InputStream source)](#SnappyArchive-java.io.InputStream-) | [SnappyArchive](../../com.aspose.zip/snappyarchive) क्लास का नया उदाहरण प्रारंभ करता है जो डीकंप्रेसन के लिए तैयार है। |
| [SnappyArchive(String path)](#SnappyArchive-java.lang.String-) | [SnappyArchive](../../com.aspose.zip/snappyarchive) क्लास का नया उदाहरण प्रारंभ करता है जो डीकंप्रेसन के लिए तैयार है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | स्नैपी अभिलेख को फ़ाइल में निकालता है। |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | स्नैपी अभिलेख को स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | स्नैपी अभिलेख को पथ द्वारा फ़ाइल में निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो स्नैपी अभिलेख बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getName()](#getName--) | मूल फ़ाइल का नाम। |
| [save(File destination)](#save-java.io.File-) | प्रदान की गई लक्ष्य फ़ाइल में स्नैपी अभिलेख को सहेजता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | प्रदान की गई स्ट्रीम में स्नैपी अभिलेख को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | प्रदान की गई लक्ष्य फ़ाइल में स्नैपी अभिलेख को सहेजता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### SnappyArchive() {#SnappyArchive--}
```
public SnappyArchive()
```


[SnappyArchive](../../com.aspose.zip/snappyarchive) क्लास का नया उदाहरण प्रारंभ करता है जो संपीड़न के लिए तैयार है।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



### SnappyArchive(InputStream source) {#SnappyArchive-java.io.InputStream-}
```
public SnappyArchive(InputStream source)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The source of the archive. |

### SnappyArchive(String path) {#SnappyArchive-java.lang.String-}
```
public SnappyArchive(String path)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

```

``````

      try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
          try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
              try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                  archive.extract(extractedFile);
              }
          }
      } catch (IOException ex) {
      }
 
```

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। See [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) डिकम्प्रेस करने के लिए मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव के स्रोत का पथ |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


स्नैपी अभिलेख को फ़ाइल में निकालता है।

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
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


Extracts snappy archive to a stream.

```

``````

     try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
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


स्नैपी अभिलेख को पथ द्वारा फ़ाइल में निकालता है।

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
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

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive
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
java.lang.Long - length.
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.snappy"));
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.File | फ़ाइल, जिसे गंतव्य स्ट्रीम के रूप में खोला जाएगा |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


प्रदान की गई स्ट्रीम में स्नैपी अभिलेख को सहेजता है।

```

``````

try (FileOutputStream snappyFile = new FileOutputStream("archive.snappy")) {
try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save(snappyFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.snappy");
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

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as an input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.snappy");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव के लिए इनपुट स्ट्रीम |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | the path to the file which will be opened as an input stream |

