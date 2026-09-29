---
title: "RarArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास RAR अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 97
url: /hi/java/com.aspose.zip/rararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class RarArchive implements IArchive, AutoCloseable
```

यह क्लास RAR आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग RAR आर्काइव निकालने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [RarArchive(String path)](#RarArchive-java.lang.String-) | नया उदाहरण प्रारंभ करता है [RarArchive](../../com.aspose.zip/rararchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [RarArchive(String path, RarArchiveLoadOptions loadOptions)](#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-) | नया उदाहरण प्रारंभ करता है [RarArchive](../../com.aspose.zip/rararchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [RarArchive(InputStream sourceStream)](#RarArchive-java.io.InputStream-) | नया उदाहरण प्रारंभ करता है [RarArchive](../../com.aspose.zip/rararchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)](#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-) | नया उदाहरण प्रारंभ करता है [RarArchive](../../com.aspose.zip/rararchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getEntries()](#getEntries--) | RAR आर्काइव बनाते हुए [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) प्रकार की प्रविष्टियों को प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | RAR आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
### RarArchive(String path) {#RarArchive-java.lang.String-}
```
public RarArchive(String path)
```


नया उदाहरण प्रारंभ करता है [RarArchive](../../com.aspose.zip/rararchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्नलिखित उदाहरण एक आर्काइव को निकालता है, फिर पहली प्रविष्टि को `MemoryStream` में डिकम्प्रेस करता है।

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (RarArchive archive = new RarArchive("data.rar")) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### RarArchive(String path, RarArchiveLoadOptions loadOptions) {#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(String path, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (RarArchive archive = new RarArchive("data.rar")) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

यह कंस्ट्रक्टर कोई भी प्रविष्टि डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### RarArchive(InputStream sourceStream) {#RarArchive-java.io.InputStream-}
```
public RarArchive(InputStream sourceStream)
```


नया उदाहरण प्रारंभ करता है [RarArchive](../../com.aspose.zip/rararchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।


निम्नलिखित उदाहरण पहले प्रविष्टि को डिकोड और डिकम्प्रेस करके `MemoryStream` में रखता है।

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions) {#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.


The following example decipher and decompress first entry to a `MemoryStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (RarArchive archive = new RarArchive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर कोई भी प्रविष्टि डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत। |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है।

```

``````

try (RarArchive archive = new RarArchive("archive.rar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<RarArchiveEntry> getEntries()
```


Gets entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.

**Returns:**
java.util.List&lt;com.aspose.zip.RarArchiveEntry&gt; - entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
