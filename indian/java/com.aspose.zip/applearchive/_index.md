---
title: "AppleArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक Apple Archive .aar फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 16
url: /hi/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

यह क्लास एक Apple Archive (.aar) फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग Apple Archive फ़ाइलें बनाने के लिए करें।

Apple और Apple Archive, Apple Inc. के ट्रेडमार्क हैं।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का, जो निर्मित प्रविष्टियों के लिए उपयोग की गई सेटिंग्स के साथ है। |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का, जो निर्मित प्रविष्टियों के लिए उपयोग की गई सेटिंग्स के साथ है। |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [dispose()](#dispose--) | ऐप्लिकेशन-परिभाषित कार्यों को निष्पादित करता है जो अनमैनेज्ड संसाधनों को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित हैं। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getEntries()](#getEntries--) | संग्रह को बनाते हुए प्रविष्टियों को प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getNewEntrySettings()](#getNewEntrySettings--) | नव निर्मित प्रविष्टियों के लिए उपयोग की गई सेटिंग्स को प्राप्त करता है। |
| [isSolid()](#isSolid--) | एक मान प्राप्त करता है जो दर्शाता है कि संग्रह सॉलिड संपीड़न का उपयोग करता है या नहीं। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | संग्रह को प्रदान की गई गंतव्य फ़ाइल में सहेजता है। |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का, जो निर्मित प्रविष्टियों के लिए उपयोग की गई सेटिंग्स के साथ है।

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का, जो निर्मित प्रविष्टियों के लिए उपयोग की गई सेटिंग्स के साथ है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | नए Apple Archive को बनाते समय उपयोग की गई सेटिंग्स। |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | आर्काइव का स्रोत। |

यह कंस्ट्रक्टर किसी भी प्रविष्टि को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) और [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) मेथड्स। |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत। |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

यह कंस्ट्रक्टर किसी भी प्रविष्टि को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) और [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) मेथड्स। |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |

यह कंस्ट्रक्टर किसी भी प्रविष्टि को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) और [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) मेथड्स। |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


एक नया उदाहरण प्रारंभ करता है [AppleArchive](../../com.aspose.zip/applearchive) क्लास का और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

यह कंस्ट्रक्टर किसी भी प्रविष्टि को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) और [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) मेथड्स। |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संकुचित करने के लिए डायरेक्टरी। |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संकुचित करने के लिए डायरेक्टरी। |
| includeRootDirectory | बूलियन | यह दर्शाता है कि रूट डायरेक्टरी को स्वयं शामिल करना है या नहीं। |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| fileInfo | java.io.File | संकुचित की जाने वाली फ़ाइल का मेटाडेटा। |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| fileInfo | java.io.File | संकुचित की जाने वाली फ़ाइल का मेटाडेटा। |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें। |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम। |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| path | java.lang.String | फ़ाइल को संपीड़ित करने का पथ। |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| path | java.lang.String | फ़ाइल को संपीड़ित करने का पथ। |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें। |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


ऐप्लिकेशन-परिभाषित कार्यों को निष्पादित करता है जो अनमैनेज्ड संसाधनों को मुक्त करने, रिलीज़ करने या रीसेट करने से संबंधित हैं।

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाली निर्देशिका का पथ। |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


संग्रह को बनाते हुए प्रविष्टियों को प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - संग्रह को बनाते हुए प्रविष्टियाँ।
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ जो संग्रह को बनाती हैं
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


नव निर्मित प्रविष्टियों के लिए उपयोग की गई सेटिंग्स को प्राप्त करता है।

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


एक मान प्राप्त करता है जो दर्शाता है कि संग्रह सॉलिड संपीड़न का उपयोग करता है या नहीं। सॉलिड मोड में, सभी प्रविष्टि डेटा एक ही स्ट्रीम के रूप में संपीड़ित होता है और व्यक्तिगत प्रविष्टि निष्कर्षण उपलब्ध नहीं है। इसके बजाय उपयोग करें [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--)।

**Returns:**
boolean - एक मान जो दर्शाता है कि संग्रह सॉलिड संपीड़न का उपयोग करता है या नहीं।
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए। कुछ संपीड़न सेटिंग्स, जैसे LZ4, को एक सीक करने योग्य स्ट्रीम की भी आवश्यकता होती है। |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


संग्रह को प्रदान की गई गंतव्य फ़ाइल में सहेजता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले संग्रह का पथ। |

