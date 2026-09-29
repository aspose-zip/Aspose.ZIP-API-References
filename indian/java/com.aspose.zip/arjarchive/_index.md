---
title: "ArjArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक ARJ अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 37
url: /hi/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

यह क्लास एक ARJ अभिलेख फ़ाइल का प्रतिनिधित्व करती है।

केवल निम्नलिखित संपीड़न विधियों का समर्थन किया जाता है:

| ------ | ------------------------------------------------------------ |
| विधि | व्याख्या                                                  |
| 0      | असंपीड़ित                                                 |
| 1      | LZ77 और अनुकूली Huffman कोडिंग का संयोजन। सर्वोत्तम अनुपात। |
| 2      | LZ77 और अनुकूली Huffman कोडिंग का संयोजन।             |
| 3      | LZ77 और अनुकूली Huffman कोडिंग का संयोजन। सर्वोत्तम गति। |
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | एक नया उदाहरण प्रारंभ करता है [ArjArchive](../../com.aspose.zip/arjarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | एक नया उदाहरण प्रारंभ करता है [ArjArchive](../../com.aspose.zip/arjarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है [ArjArchive](../../com.aspose.zip/arjarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | एक नया उदाहरण प्रारंभ करता है [ArjArchive](../../com.aspose.zip/arjarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | सभी एंट्रीज़ को निर्दिष्ट डायरेक्टरी में निकालता है। |
| [getCommentary()](#getCommentary--) | टिप्पणी प्राप्त करता है। |
| [getEntries()](#getEntries--) | ARJ आर्काइव बनाते हुए [ArjEntryPlain](../../com.aspose.zip/arjentryplain) प्रकार की एंट्रीज़ प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getName()](#getName--) | मूल नाम प्राप्त करता है। |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


एक नया उदाहरण प्रारंभ करता है [ArjArchive](../../com.aspose.zip/arjarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

यह कंस्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| extractionSource | java.io.InputStream | आर्काइव का स्रोत |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


एक नया उदाहरण प्रारंभ करता है [ArjArchive](../../com.aspose.zip/arjarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

यह कंस्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| extractionSource | java.io.InputStream | आर्काइव का स्रोत |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


एक नया उदाहरण प्रारंभ करता है [ArjArchive](../../com.aspose.zip/arjarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को अनपैक नहीं करता है। डिकम्प्रेस करने के लिए देखें [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


सभी एंट्रीज़ को निर्दिष्ट डायरेक्टरी में निकालता है।

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
