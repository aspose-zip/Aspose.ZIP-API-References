---
title: "ArchiveEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "अभिलेख के भीतर एकल फ़ाइल को प्रतिनिधित्व करता है।"
type: docs
weight: 27
url: /hi/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

अभिलेख के भीतर एकल फ़ाइल को प्रतिनिधित्व करता है।

[ArchiveEntry](../../com.aspose.zip/archiveentry) इंस्टेंस को [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) में कास्ट करें ताकि यह निर्धारित किया जा सके कि प्रविष्टि एन्क्रिप्टेड है या नहीं।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getComment()](#getComment--) | आर्काइव के भीतर प्रविष्टि की टिप्पणी प्राप्त करता है। |
| [getCompressedSize()](#getCompressedSize--) | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [getCompressionProgressed()](#getCompressionProgressed--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [getCompressionSettings()](#getCompressionSettings--) | संपीड़न या डीकंप्रेशन के लिए सेटिंग्स प्राप्त करता है। |
| [getDataSource()](#getDataSource--) | यदि प्रविष्टि को आर्काइव में जोड़ा गया था, न कि निकाला गया, तो प्रविष्टि का स्रोत। |
| [getExtractionProgressed()](#getExtractionProgressed--) | कच्ची स्ट्रीम के एक भाग के निकाले जाने पर उठाया गया इवेंट प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | अंतिम संशोधित तिथि और समय प्राप्त करता है। |
| [getName()](#getName--) | अभिलेख के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | मूल फ़ाइल का आकार प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं। |
| [open()](#open--) | निकालने के लिए प्रविष्टि खोलता है और डिकम्प्रेस्ड प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [open(String password)](#open-java.lang.String-) | निकालने के लिए प्रविष्टि खोलता है और डिकम्प्रेस्ड प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को सेट करता है। |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | कच्ची स्ट्रीम के एक भाग के निकाले जाने पर उठाया गया इवेंट सेट करता है। |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | अंतिम संशोधित तिथि और समय सेट करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।

पासवर्ड के साथ zip अभिलेख की एक प्रविष्टि निकालें।

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| गंतव्य | java.io.OutputStream | गंतव्य स्ट्रीम। लिखने योग्य होना चाहिए। |
| पासवर्ड | java.lang.String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है।

ZIP अभिलेख के दो प्रविष्टियों को निकालें, प्रत्येक का अपना पासवर्ड हो।

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | गंतव्य फ़ाइल का पथ। यदि फ़ाइल पहले से मौजूद है, तो उसे अधिलेखित किया जाएगा। |
| पासवर्ड | java.lang.String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। |

**Returns:**
java.io.File - निकाली गई फ़ाइल की फ़ाइल जानकारी
### getComment() {#getComment--}
```
public final String getComment()
```


आर्काइव के भीतर प्रविष्टि की टिप्पणी प्राप्त करता है।

**Returns:**
java.lang.String - अभिलेख के भीतर प्रविष्टि की टिप्पणी
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


संपीड़ित फ़ाइल का आकार प्राप्त करता है।

**Returns:**
long - संकुचित फ़ाइल का आकार
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

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

इस नमूने में इवेंट हैंडलर का उपयोग प्रविष्टि के पहले सौ मेगाबाइट निकाले जाने के बाद रद्द करने के लिए किया जाता है।

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
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


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

फ़ाइल की मूल सामग्री प्राप्त करने के लिए स्ट्रीम से पढ़ें।

**Returns:**
java.io.InputStream - वह स्ट्रीम जो प्रविष्टि की सामग्री को दर्शाती है।
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


निकालने के लिए प्रविष्टि खोलता है और डिकम्प्रेस्ड प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है।


उपयोग:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
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

इवेंट प्रेषक एक [ArchiveEntry](../../com.aspose.zip/archiveentry) उदाहरण है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है। |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


कच्ची स्ट्रीम के एक भाग के निकाले जाने पर उठाया गया इवेंट सेट करता है।

इस नमूने में इवेंट हैंडलर का उपयोग प्रतिशत में प्रोसेस किए गए आकार के हिस्से की गणना के लिए किया जाता है।

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

इवेंट प्रेषक एक [ArchiveEntry](../../com.aspose.zip/archiveentry) उदाहरण है। निष्कर्षण को रद्द करना संभव है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब कच्ची स्ट्रीम का एक भाग निकाला जाता है। |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


अंतिम संशोधित तिथि और समय सेट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | java.util.Date | अंतिम संशोधित तिथि और समय |

