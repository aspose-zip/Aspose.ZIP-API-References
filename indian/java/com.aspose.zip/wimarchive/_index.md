---
title: "WimArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह वर्ग एक wim संग्रह फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 130
url: /hi/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

यह वर्ग एक wim संग्रह फ़ाइल का प्रतिनिधित्व करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | एक नया उदाहरण प्रारंभ करता है [WimArchive](../../com.aspose.zip/wimarchive) क्लास का और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | एक नया उदाहरण प्रारंभ करता है [WimArchive](../../com.aspose.zip/wimarchive) क्लास का और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है [WimArchive](../../com.aspose.zip/wimarchive) क्लास का और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | एक नया उदाहरण प्रारंभ करता है [WimArchive](../../com.aspose.zip/wimarchive) क्लास का और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | पथ द्वारा फ़ाइल में संग्रह को निकालता है। |
| [getBootImageIndex()](#getBootImageIndex--) | (शून्य-आधारित) बूटेबल इमेज का सूचकांक प्राप्त करता है। |
| [getEntries()](#getEntries--) | संग्रह बनाती हुई [WimEntry](../../com.aspose.zip/wimentry) प्रकार की एंट्रीज़ प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | wim संग्रह बनाती हुई [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है। |
| [getFileFormatVersion()](#getFileFormatVersion--) | फ़ाइल फ़ॉर्मेट का संस्करण प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getGuid()](#getGuid--) | संग्रह के लिए पहचानात्मक UUID प्राप्त करता है। |
| [getImages()](#getImages--) | संग्रह बनाती हुई [WimImage](../../com.aspose.zip/wimimage) प्रकार की एंट्रीज़ प्राप्त करता है। |
| [getManifest()](#getManifest--) | फ़ाइल और उसमें मौजूद इमेजेज़ का वर्णन करने वाला एम्बेडेड मैनिफेस्ट प्राप्त करता है। |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


एक नया उदाहरण प्रारंभ करता है [WimArchive](../../com.aspose.zip/wimarchive) क्लास का और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर कोई भी एंट्री अनपैक नहीं करता है। अनपैक करने के लिए देखें [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


एक नया उदाहरण प्रारंभ करता है [WimArchive](../../com.aspose.zip/wimarchive) क्लास का और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

यह कंस्ट्रक्टर कोई भी एंट्री अनपैक नहीं करता है। अनपैक करने के लिए देखें [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


पथ द्वारा फ़ाइल में संग्रह को निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाली डायरेक्टरी का पथ |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


(शून्य-आधारित) बूटेबल इमेज का सूचकांक प्राप्त करता है।

**Returns:**
int - (शून्य-आधारित) बूटेबल इमेज का सूचकांक
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


संग्रह बनाती हुई [WimEntry](../../com.aspose.zip/wimentry) प्रकार की एंट्रीज़ प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - एंट्रीज़ जो संग्रह बनाती हैं
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


wim संग्रह बनाती हुई [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - एंट्रीज़ जो wim संग्रह बनाती हैं, [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


फ़ाइल फ़ॉर्मेट का संस्करण प्राप्त करता है।

**Returns:**
int - फ़ाइल फ़ॉर्मेट का संस्करण
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


संग्रह के लिए पहचानात्मक UUID प्राप्त करता है।

**Returns:**
java.util.UUID - अभिलेख के लिए पहचानकर्ता UUID
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


संग्रह बनाती हुई [WimImage](../../com.aspose.zip/wimimage) प्रकार की एंट्रीज़ प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - अभिलेख को बनाते हुए [WimImage](../../com.aspose.zip/wimimage) प्रकार के प्रविष्टियाँ
### getManifest() {#getManifest--}
```
public final String getManifest()
```


फ़ाइल और उसमें मौजूद इमेजेज़ का वर्णन करने वाला एम्बेडेड मैनिफेस्ट प्राप्त करता है।

**Returns:**
java.lang.String - फ़ाइल और सम्मिलित छवियों का वर्णन करने वाला एम्बेडेड मैनिफेस्ट
