---
title: "LhaArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक LHA .lzh आर्काइव फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 75
url: /hi/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

यह क्लास एक LHA (.lzh) आर्काइव फ़ाइल का प्रतिनिधित्व करती है।

केवल निम्नलिखित संपीड़न विधियों का समर्थन किया जाता है:

| ------ | --------------------------------------------- |
| Method | Explanation                                   |
| lh0    | असंपीड़ित                                  |
| lh4    | 8 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman   |
| lh5    | 16 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman  |
| lh6    | 64 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman  |
| lh7    | 128 KiB स्लाइडिंग डिक्शनरी और स्थिर Huffman |
| lhx    | 1 Mib स्लाइडिंग डिक्शनरी और स्थिर Huffman   |
| lhd    | डायरेक्टरी                                     |
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | नया उदाहरण प्रारंभ करता है [LhaArchive](../../com.aspose.zip/lhaarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | नया उदाहरण प्रारंभ करता है [LhaArchive](../../com.aspose.zip/lhaarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | नया उदाहरण प्रारंभ करता है [LhaArchive](../../com.aspose.zip/lhaarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | नया उदाहरण प्रारंभ करता है [LhaArchive](../../com.aspose.zip/lhaarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों और निर्देशिकाओं को प्रदान की गई निर्देशिका में निकालता है। |
| [getEntries()](#getEntries--) | आर्काइव बनाते हुए [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) प्रकार की फ़ाइल प्रविष्टियों को प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


नया उदाहरण प्रारंभ करता है [LhaArchive](../../com.aspose.zip/lhaarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

यह कंस्ट्रक्टर कोई भी प्रविष्टि डीकंप्रेस नहीं करता। डीकंप्रेस करने के लिए देखें [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


नया उदाहरण प्रारंभ करता है [LhaArchive](../../com.aspose.zip/lhaarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

यह कंस्ट्रक्टर कोई भी प्रविष्टि डीकंप्रेस नहीं करता। डीकंप्रेस करने के लिए देखें [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


नया उदाहरण प्रारंभ करता है [LhaArchive](../../com.aspose.zip/lhaarchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्नलिखित उदाहरण एक आर्काइव को निकालता है, फिर पहली प्रविष्टि को `MemoryStream` में डिकम्प्रेस करता है।

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता। डिकम्प्रेस करने के लिए देखें [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\\#extract-OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

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

try (LhaArchive archive = new LhaArchive(\"archive.lzh\")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
