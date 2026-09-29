---
title: "IArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह इंटरफ़ेस एक अभिलेख का प्रतिनिधित्व करता है।"
type: docs
weight: 161
url: /hi/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

यह इंटरफ़ेस एक अभिलेख का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है।

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाली निर्देशिका का पथ। |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं।

केवल संपीड़न के लिए आर्काइव, जैसे gzip, bzip2, lzip, lzma, lz4, xz, z, एकल रिकॉर्ड - स्वयं आर्काइव - से बनते हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - अभिलेख बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ।
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
