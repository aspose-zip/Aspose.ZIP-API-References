---
title: "LzxArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक LZX .lzx आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 89
url: /hi/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

यह क्लास एक LZX (.lzx) आर्काइव फ़ाइल का प्रतिनिधित्व करती है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | एक नया इंस्टेंस प्रारंभ करता है [LzxArchive](../../com.aspose.zip/lzxarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | एक नया इंस्टेंस प्रारंभ करता है [LzxArchive](../../com.aspose.zip/lzxarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | एक नया इंस्टेंस प्रारंभ करता है [LzxArchive](../../com.aspose.zip/lzxarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | एक नया इंस्टेंस प्रारंभ करता है [LzxArchive](../../com.aspose.zip/lzxarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों और निर्देशिकाओं को प्रदान की गई निर्देशिका में निकालता है। |
| [getEntries()](#getEntries--) | आर्काइव को बनाते हुए [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) प्रकार की फ़ाइल प्रविष्टियों को प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


एक नया इंस्टेंस प्रारंभ करता है [LzxArchive](../../com.aspose.zip/lzxarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

यह कंस्ट्रक्टर किसी भी प्रविष्टि को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| extractionSource | java.io.InputStream | आर्काइव का स्रोत। |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


एक नया इंस्टेंस प्रारंभ करता है [LzxArchive](../../com.aspose.zip/lzxarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

यह कंस्ट्रक्टर किसी भी प्रविष्टि को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| extractionSource | java.io.InputStream | आर्काइव का स्रोत। |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


एक नया इंस्टेंस प्रारंभ करता है [LzxArchive](../../com.aspose.zip/lzxarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्नलिखित उदाहरण एक आर्काइव को निकालता है, फिर पहली प्रविष्टि को `MemoryStream` में डिकम्प्रेस करता है।

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

यह कंस्ट्रक्टर किसी भी प्रविष्टि को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


आर्काइव में सभी फ़ाइलों और निर्देशिकाओं को प्रदान की गई निर्देशिका में निकालता है।

```

``````

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
