---
title: "AlzArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "एक ALZ अभिलेख फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

एक ALZ अभिलेख फ़ाइल का प्रतिनिधित्व करता है। इस वर्ग का उपयोग करके आप ALZ अभिलेखों की जाँच और निकासी कर सकते हैं।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | एक स्ट्रीम से ALZ अभिलेख को प्रारंभ करता है। |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | प्रदान किए गए लोड विकल्पों का उपयोग करके एक स्ट्रीम से ALZ अभिलेख को प्रारंभ करता है। |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | फ़ाइल पथ से ALZ अभिलेख को प्रारंभ करता है। |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | प्रदान किए गए लोड विकल्पों का उपयोग करके फ़ाइल पथ से ALZ अभिलेख को प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | इस अभिलेख द्वारा रखे गए संसाधनों को मुक्त करता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | सभी फ़ाइलों और निर्देशिकाओं को प्रदान की गई निर्देशिका में निकालता है। |
| [getEntries()](#getEntries--) | इस अभिलेख के घटक प्रविष्टियों को प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | सामान्य अभिलेख इंटरफ़ेस के माध्यम से प्रविष्टियों को प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


एक स्ट्रीम से ALZ अभिलेख को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | ALZ अभिलेख स्ट्रीम; इसे पढ़ने और खोजने का समर्थन करना चाहिए |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


प्रदान किए गए लोड विकल्पों का उपयोग करके एक स्ट्रीम से ALZ अभिलेख को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | java.io.InputStream | ALZ अभिलेख स्ट्रीम; इसे पढ़ने और खोजने का समर्थन करना चाहिए |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | अभिलेख को लोड करने के लिए उपयोग किए गए विकल्प |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


फ़ाइल पथ से ALZ अभिलेख को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | java.lang.String | ALZ अभिलेख का पथ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


प्रदान किए गए लोड विकल्पों का उपयोग करके फ़ाइल पथ से ALZ अभिलेख को प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | java.lang.String | ALZ अभिलेख का पथ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | अभिलेख को लोड करने के लिए उपयोग किए गए विकल्प |

### close() {#close--}
```
public void close()
```


इस अभिलेख द्वारा रखे गए संसाधनों को मुक्त करता है।

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


सभी फ़ाइलों और निर्देशिकाओं को प्रदान की गई निर्देशिका में निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | गंतव्य निर्देशिका; यह आवश्यक होने पर बनाई जाती है |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


इस अभिलेख के घटक प्रविष्टियों को प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - अपरिवर्तनीय ALZ प्रविष्टियों की सूची
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


सामान्य अभिलेख इंटरफ़ेस के माध्यम से प्रविष्टियों को प्राप्त करता है।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - अभिलेख प्रविष्टियाँ
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
