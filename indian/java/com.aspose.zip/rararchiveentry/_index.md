---
title: "RarArchiveEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "अभिलेख के भीतर एकल फ़ाइल को प्रतिनिधित्व करता है।"
type: docs
weight: 98
url: /hi/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

अभिलेख के भीतर एकल फ़ाइल को प्रतिनिधित्व करता है।

एक [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) उदाहरण को [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) में कास्ट करें यह निर्धारित करने के लिए कि एंट्री एन्क्रिप्टेड है या नहीं।
## Methods

| Method | विवरण |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है। |
| [extract(String path)](#extract-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | प्रदान किए गए पथ द्वारा फ़ाइल सिस्टम में प्रविष्टि को निकालता है। |
| [getCompressedSize()](#getCompressedSize--) | संपीड़ित फ़ाइल का आकार प्राप्त करता है। |
| [getCreationTime()](#getCreationTime--) | निर्माण तिथि और समय प्राप्त करता है। |
| [getExtractionProgressed()](#getExtractionProgressed--) | कच्ची स्ट्रीम के एक भाग के निकाले जाने पर उठाया गया इवेंट प्राप्त करता है। |
| [getLastAccessTime()](#getLastAccessTime--) | अंतिम पहुँच तिथि और समय प्राप्त करता है। |
| [getLength()](#getLength--) | लंबाई प्राप्त करता है। |
| [getModificationTime()](#getModificationTime--) | अंतिम संशोधित तिथि और समय प्राप्त करता है। |
| [getName()](#getName--) | आर्काइव के भीतर प्रविष्टि का नाम प्राप्त करता है। |
| [getUncompressedSize()](#getUncompressedSize--) | मूल फ़ाइल का आकार प्राप्त करता है। |
| [isDirectory()](#isDirectory--) | यह दर्शाने वाला मान प्राप्त करता है कि प्रविष्टि एक निर्देशिका है या नहीं। |
| [open()](#open--) | निकालने के लिए प्रविष्टि खोलता है और डिकम्प्रेस्ड प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [open(String password)](#open-java.lang.String-) | निकालने के लिए प्रविष्टि खोलता है और डिकम्प्रेस्ड प्रविष्टि सामग्री के साथ एक स्ट्रीम प्रदान करता है। |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | कच्ची स्ट्रीम के एक भाग के निकाले जाने पर उठाया गया इवेंट सेट करता है। |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


प्रदान किए गए स्ट्रीम में प्रविष्टि को निकालता है।


पासवर्ड के साथ rar अभिलेख के एक प्रविष्टि को निकालें।

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
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


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
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


rar अभिलेख की दो प्रविष्टियों को निकालें।

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
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


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
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
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


संपीड़ित फ़ाइल का आकार प्राप्त करता है।

**Returns:**
long - संपीड़ित फ़ाइल का आकार
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


निर्माण तिथि और समय प्राप्त करता है।

**Returns:**
java.util.Date - निर्माण तिथि और समय।
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


कच्ची स्ट्रीम के एक भाग के निकाले जाने पर उठाया गया इवेंट प्राप्त करता है।

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
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
long - the size of the original file.
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

स्ट्रीम से पढ़ें ताकि फ़ाइल की मूल सामग्री प्राप्त हो सके। उदाहरण अनुभाग देखें।

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
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

इवेंट प्रेषक एक [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) उदाहरण है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब कच्ची स्ट्रीम का एक भाग निकाला जाता है। |

