---
title: "Lz4Archive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास LZ4 आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 80
url: /hi/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

यह क्लास LZ4 आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग LZ4 आर्काइव को निकालने या बनाने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | डिकम्प्रेस करने के लिए तैयार [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | डिकम्प्रेस करने के लिए तैयार [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Lz4Archive()](#Lz4Archive--) | कम्प्रेस करने के लिए तैयार [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | कम्प्रेस करने के लिए तैयार [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | पथ द्वारा फ़ाइल में संग्रह को निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getName()](#getName--) | मूल नाम प्राप्त करता है। |
| [open()](#open--) | निकालने के लिए आर्काइव खोलता है और आर्काइव सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [save(File destination)](#save-java.io.File-) | प्रदान किए गए लक्ष्य फ़ाइल में lz4 आर्काइव को सहेजता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में lz4 आर्काइव को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(File fileInfo)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String path)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


डिकम्प्रेस करने के लिए तैयार [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

स्ट्रीम से एक आर्काइव खोलें और उसे `MemoryStream` में निकालें।

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream(\"archive.lz4\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

यह कन्स्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [open()](../../com.aspose.zip/lz4archive\#open--) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | आर्काइव लोड करने के विकल्प। |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


[Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

फ़ाइल से पथ द्वारा एक अभिलेख खोलें और इसे `MemoryStream` में निकालें।

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

यह कन्स्ट्रक्टर डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए [open()](../../com.aspose.zip/lz4archive\#open--) मेथड देखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | आर्काइव लोड करने के विकल्प। |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


कम्प्रेस करने के लिए तैयार [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


कम्प्रेस करने के लिए तैयार [Lz4Archive](../../com.aspose.zip/lz4archive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | संयुक्त आर्काइव की सेटिंग। |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


आर्काइव को प्रदान किए गए स्ट्रीम में निकालता है।

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
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


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

फ़ाइल की मूल सामग्री प्राप्त करने के लिए स्ट्रीम से पढ़ें। उदाहरण अनुभाग देखें।

**Returns:**
java.io.InputStream - वह स्ट्रीम जो आर्काइव की सामग्री को दर्शाता है।
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


प्रदान किए गए लक्ष्य फ़ाइल में lz4 आर्काइव को सहेजता है।

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lz4\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource("data.bin");
archive.save(\"archive.lz4\");
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
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

संधि tar.lz4 आर्काइव बनाने के लिए इस मेथड का उपयोग करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | कम्प्रेस करने के लिए टार आर्काइव। |

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
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileInfo | java.io.File | कम्प्रेस की जाने वाली फ़ाइल का संदर्भ। |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save(\"archive.lz4\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | कम्प्रेस की जाने वाली फ़ाइल का पथ। |

