---
title: "IsoArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "ISO 9660 आर्काइव का प्रतिनिधित्व करता है।"
type: docs
weight: 71
url: /hi/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

एक ISO आर्काइव (ISO 9660) का प्रतिनिधित्व करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और नई फाइलों और डायरेक्टरीज़ को जोड़ने के लिए एक खाली ISO आर्काइव बनाता है। |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | ISO इमेज में एक डायरेक्टरी जोड़ता है। |
| [createEntry(String name)](#createEntry-java.lang.String-) | ISO इमेज में एक फाइल जोड़ता है। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | ISO इमेज में एक फाइल जोड़ता है। |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | ISO इमेज में एक फाइल जोड़ता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | सभी एंट्रीज़ को निर्दिष्ट डायरेक्टरी में निकालता है। |
| [getEntries()](#getEntries--) | [IsoEntry](../../com.aspose.zip/isoentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | ISO इमेज को निर्दिष्ट स्ट्रीम में सहेजता है। |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | ISO इमेज को निर्दिष्ट स्ट्रीम में सहेजता है। |
| [save(String path)](#save-java.lang.String-) | ISO इमेज को निर्दिष्ट पथ पर सहेजता है। |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | ISO इमेज को निर्दिष्ट पथ पर सहेजता है। |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और नई फाइलों और डायरेक्टरीज़ को जोड़ने के लिए एक खाली ISO आर्काइव बनाता है।

निम्न उदाहरण दिखाता है कि कैसे एक नया खाली ISO आर्काइव बनाया जाए और उसमें फाइलें जोड़ी जाएँ:

```

``````

// एक नया खाली ISO आर्काइव बनाएं
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO आर्काइव में फाइलें जोड़ें
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO आर्काइव को फ़ाइल में सहेजें
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर कोई भी एंट्री अनपैक नहीं करता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

यह कंस्ट्रक्टर कोई भी एंट्री अनपैक नहीं करता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


नया उदाहरण प्रारंभ करता है [IsoArchive](../../com.aspose.zip/isoarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | एंट्रीज़ को निकालने के लिए निर्देशिका |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


[IsoEntry](../../com.aspose.zip/isoentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं।

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - आइसो आर्काइव बनाते हुए [IsoEntry](../../com.aspose.zip/isoentry) प्रकार की प्रविष्टियाँ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - आइसो आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


ISO इमेज को निर्दिष्ट स्ट्रीम में सहेजता है।

निम्न उदाहरण दिखाता है कि ISO आर्काइव को मेमोरी स्ट्रीम में कैसे सहेजा जाए:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// एक नया खाली ISO आर्काइव बनाएं
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO आर्काइव में फाइलें जोड़ें
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO आर्काइव को मेमोरी स्ट्रीम में सहेजें
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.OutputStream | स्ट्रीम जहाँ ISO इमेज सहेजा जाएगा |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | ISO आर्काइव को सहेजने के विकल्प |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


ISO इमेज को निर्दिष्ट पथ पर सहेजता है।

निम्न उदाहरण दिखाता है कि ISO आर्काइव को फ़ाइल में कैसे सहेजा जाए:

```

``````

// एक नया खाली ISO आर्काइव बनाएं
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO आर्काइव में फाइलें जोड़ें
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO आर्काइव को फ़ाइल में सहेजें
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | पथ जहाँ ISO इमेज सहेजा जाएगा |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | ISO आर्काइव को सहेजने के विकल्प |

