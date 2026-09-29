---
title: "ZArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास Z संपीड़न आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 153
url: /hi/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

यह क्लास Z (compress) आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग Z आर्काइव को बनाने या निकालने के लिए करें।

देखें [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ZArchive()](#ZArchive--) | कम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है। |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है। |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है। |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है। |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Z आर्काइव को फ़ाइल में निकालता है। |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Z आर्काइव को स्ट्रीम में निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | Z आर्काइव को पथ द्वारा फ़ाइल में निकालता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव की सामग्री को प्रदान किए गए निर्देशिका में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो Z आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getLength()](#getLength--) | प्रविष्टि की लंबाई बाइट्स में प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर एंट्री का नाम प्राप्त करता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | प्रदान की गई स्ट्रीम में Z आर्काइव को सहेजता है। |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | प्रदान की गई स्ट्रीम में Z आर्काइव को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | प्रदान की गई लक्ष्य फ़ाइल में Z आर्काइव को सहेजता है। |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | प्रदान की गई लक्ष्य फ़ाइल में Z आर्काइव को सहेजता है। |
| [setSource(File file)](#setSource-java.io.File-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है। |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


कम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है।

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | आर्काइव लोड करने के विकल्प। |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव के स्रोत का पथ |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


डिकम्प्रेस करने के लिए तैयार [ZArchive](../../com.aspose.zip/zarchive) क्लास का नया उदाहरण आरंभ करता है।

यह कंस्ट्रक्टर डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव के स्रोत का पथ |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | आर्काइव लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Z आर्काइव को फ़ाइल में निकालता है।

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
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


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


Z आर्काइव को पथ द्वारा फ़ाइल में निकालता है।

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

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
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


प्रदान की गई स्ट्रीम में Z आर्काइव को सहेजता है।

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


प्रदान की गई लक्ष्य फ़ाइल में Z आर्काइव को सहेजता है।

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| फ़ाइल | java.io.File | फ़ाइल जानकारी जो इनपुट स्ट्रीम के रूप में खोली जाएगी |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


आर्काइव के भीतर संकुचित की जाने वाली सामग्री को सेट करता है।

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourcePath | java.lang.String | फ़ाइल का पथ जो इनपुट स्ट्रीम के रूप में खोला जाएगा |

