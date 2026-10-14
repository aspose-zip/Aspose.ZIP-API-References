---
title: "ArchiveFactory"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "आर्काइव फ़ॉर्मेट का पता लगाता है और आर्काइव के प्रकार के अनुसार उपयुक्त ऑब्जेक्ट बनाता है।"
type: docs
weight: 31
url: /hi/java/com.aspose.zip/archivefactory/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFactory
```

आर्काइव फ़ॉर्मेट का पता लगाता है और आर्काइव के प्रकार के अनुसार उपयुक्त [IArchive](../../com.aspose.zip/iarchive) ऑब्जेक्ट बनाता है।
## Methods

| Method | विवरण |
| --- | --- |
| [compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)](#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-) | प्रदान किए गए आर्काइव फ़ॉर्मेट का उपयोग करके निर्दिष्ट डायरेक्टरी को एक आर्काइव फ़ाइल में संपीड़ित करता है। |
| [getArchive(InputStream stream)](#getArchive-java.io.InputStream-) | दिए गए स्ट्रीम द्वारा निर्दिष्ट आर्काइव प्रकार के अनुसार आर्काइव फ़ॉर्मेट का पता लगाता है और उपयुक्त [IArchive](../../com.aspose.zip/iarchive) ऑब्जेक्ट बनाता है। |
| [getArchive(InputStream stream, String password)](#getArchive-java.io.InputStream-java.lang.String-) | दिए गए स्ट्रीम द्वारा निर्दिष्ट एन्क्रिप्टेड आर्काइव प्रकार के अनुसार आर्काइव फ़ॉर्मेट का पता लगाता है और उपयुक्त [IArchive](../../com.aspose.zip/iarchive) ऑब्जेक्ट बनाता है। |
| [getArchive(String path)](#getArchive-java.lang.String-) | दिए गए पाथ द्वारा निर्दिष्ट आर्काइव प्रकार के अनुसार आर्काइव फ़ॉर्मेट का पता लगाता है और उपयुक्त [IArchive](../../com.aspose.zip/iarchive) ऑब्जेक्ट बनाता है। |
### compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat) {#compressDirectory-java.lang.String-java.lang.String-com.aspose.zip.ArchiveFormat-}
```
public static void compressDirectory(String path, String outputFileName, ArchiveFormat archiveFormat)
```


प्रदान किए गए आर्काइव फ़ॉर्मेट का उपयोग करके निर्दिष्ट डायरेक्टरी को एक आर्काइव फ़ाइल में संपीड़ित करता है।

यहाँ CompressDirectory मेथड का उपयोग करने का एक उदाहरण दिया गया है:

```

``````

String directoryPath = "C:\\path\\to\\your\\directory";
ArchiveFormat format = ArchiveFormat.Zip;
ArchiveFactory.compressDirectory(directoryPath, "result", format);
// यह निर्दिष्ट पाथ पर डायरेक्टरी की सामग्री के साथ एक ZIP फ़ाइल बनाएगा।
 
```

This method will create an archive file at the location specified by the `path` parameter. The name of the archive file will typically be the directory name followed by the appropriate file extension based on the `archiveFormat`. The directory itself is not modified or deleted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the directory that will be compressed |
| outputFileName | java.lang.String | destination file name |
| archiveFormat | [ArchiveFormat](../../com.aspose.zip/archiveformat) | the format of the archive to create (e.g., zip, rar, tar, etc.) |

### getArchive(InputStream stream) {#getArchive-java.io.InputStream-}
```
public static IArchive getArchive(InputStream stream)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(InputStream stream, String password) {#getArchive-java.io.InputStream-java.lang.String-}
```
public static IArchive getArchive(InputStream stream, String password)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of encrypted archive specified by the given stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | the stream containing the archive data |
| password | java.lang.String | password to decrypt an encrypted archive |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
### getArchive(String path) {#getArchive-java.lang.String-}
```
public static IArchive getArchive(String path)
```


Detects the archive format and creates the appropriate [IArchive](../../com.aspose.zip/iarchive) object according to the type of archive specified by the given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive to be analyzed |

**Returns:**
[IArchive](../../com.aspose.zip/iarchive) - an [IArchive](../../com.aspose.zip/iarchive) object representing the archive
