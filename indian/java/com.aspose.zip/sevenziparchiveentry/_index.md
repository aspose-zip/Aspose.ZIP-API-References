---
title: "SevenZipArchiveEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7z अभिलेख में एकल फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 105
url: /hi/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

7z अभिलेख में एकल फ़ाइल का प्रतिनिधित्व करता है।

एक [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) उदाहरण को [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) में कास्ट करें ताकि यह निर्धारित किया जा सके कि प्रविष्टि एन्क्रिप्टेड है या नहीं।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getCompressedSize()](#getCompressedSize--) | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [getCompressionProgressed()](#getCompressionProgressed--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [getCompressionSettings()](#getCompressionSettings--) | संपीड़न या डीकंप्रेशन के लिए सेटिंग्स प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | अंतिम संशोधित तिथि और समय प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | मूल फ़ाइल का आकार प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं। |
| [open()](#open--) | निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [open(String password)](#open-java.lang.String-) | निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को सेट करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

पासवर्ड के साथ zip अभिलेख की एक प्रविष्टि निकालें।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(\"archive.7z\")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम। लिखने योग्य होना चाहिए |
| पासवर्ड | java.lang.String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(\"archive.7z\")) {
archive.getEntries().get(0).extract("data.bin");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो इसे अधिलेखित किया जाएगा। |
| पासवर्ड | java.lang.String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड |

**Returns:**
java.io.File - निकाली गई फ़ाइल की फ़ाइल जानकारी
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


संपीड़ित फ़ाइल का आकार प्राप्त करता है।

**Returns:**
long - संपीड़ित फ़ाइल का आकार
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है।

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

स्ट्रीम से पढ़ें ताकि फ़ाइल की मूल सामग्री प्राप्त हो सके। उदाहरण अनुभाग देखें।

**Returns:**
java.io.InputStream - वह स्ट्रीम जो प्रविष्टि की सामग्री का प्रतिनिधित्व करता है
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


निकालने के लिए प्रविष्टि को खोलता है और प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है।

उपयोग:

```

``````

SevenZipArchive archive = new SevenZipArchive("archive.7z");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

इवेंट प्रेषक एक [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) इंस्टेंस है।

LZMA2 प्रविष्टियों के लिए सॉलिड मोड और मल्टीथ्रेडेड मोड में यह नहीं बुलाया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है। |

