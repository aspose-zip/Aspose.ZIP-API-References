---
title: "आर्काइव"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक ज़िप अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 26
url: /hi/java/com.aspose.zip/archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class Archive implements IArchive, AutoCloseable
```

यह क्लास एक ज़िप आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग ज़िप आर्काइव को बनाने, निकालने या अपडेट करने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [Archive()](#Archive--) | वैकल्पिक सेटिंग्स के साथ उसके एंट्रीज़ के लिए नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है। |
| [Archive(ArchiveEntrySettings newEntrySettings)](#Archive-com.aspose.zip.ArchiveEntrySettings-) | वैकल्पिक सेटिंग्स के साथ उसके एंट्रीज़ के लिए नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है। |
| [Archive(InputStream sourceStream)](#Archive-java.io.InputStream-) | नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-) | नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [Archive(String path)](#Archive-java.lang.String-) | नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [Archive(String path, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-) | नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [Archive(String mainSegment, String[] segmentsInOrder)](#Archive-java.lang.String-java.lang.String---) | मल्टी-वॉल्यूम ज़िप आर्काइव से नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-) | मल्टी-वॉल्यूम ज़िप आर्काइव से नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | दिए गए डायरेक्टरी में सभी फ़ाइलों और डायरेक्टरीज़ को पुनरावृत्त रूप से आर्काइव में जोड़ें। |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | दिए गए डायरेक्टरी में सभी फ़ाइलों और डायरेक्टरीज़ को पुनरावृत्त रूप से आर्काइव में जोड़ें। |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | दिए गए डायरेक्टरी में सभी फ़ाइलों और डायरेक्टरीज़ को पुनरावृत्त रूप से आर्काइव में जोड़ें। |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | दिए गए डायरेक्टरी में सभी फ़ाइलों और डायरेक्टरीज़ को पुनरावृत्त रूप से आर्काइव में जोड़ें। |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [deleteEntry(ArchiveEntry entry)](#deleteEntry-com.aspose.zip.ArchiveEntry-) | एंट्री सूची से विशिष्ट एंट्री की पहली उपस्थिति को हटाता है। |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | इंडेक्स द्वारा एंट्री सूची से एंट्री को हटाता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getComment()](#getComment--) | पूरे आर्काइव के लिए टिप्पणी प्राप्त करता है। |
| [getEntries()](#getEntries--) | [ArchiveEntry](../../com.aspose.zip/archiveentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | आर्काइव फ़ॉर्मेट (Zip) प्राप्त करता है। |
| [getNewEntrySettings()](#getNewEntrySettings--) | नए जोड़े गए [ArchiveEntry](../../com.aspose.zip/archiveentry) आइटम्स के लिए उपयोग किए गए संपीड़न और एन्क्रिप्शन सेटिंग्स। |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream outputStream, ArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, ArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-) | मल्टी-वॉल्यूम आर्काइव को प्रदान किए गए गंतव्य डायरेक्टरी में सहेजता है। |
### Archive() {#Archive--}
```
public Archive()
```


वैकल्पिक सेटिंग्स के साथ उसके एंट्रीज़ के लिए नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है।


निम्न उदाहरण दिखाता है कि डिफ़ॉल्ट सेटिंग्स के साथ एक फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```



### Archive(ArchiveEntrySettings newEntrySettings) {#Archive-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries.


The following example shows how to compress a single file with default settings.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | नए जोड़े गए [ArchiveEntry](../../com.aspose.zip/archiveentry) आइटमों के लिए उपयोग किए जाने वाले संपीड़न और एन्क्रिप्शन सेटिंग्स। यदि निर्दिष्ट नहीं किया गया, तो सबसे सामान्य Deflate संपीड़न बिना एन्क्रिप्शन के उपयोग किया जाएगा। |

### Archive(InputStream sourceStream) {#Archive-java.io.InputStream-}
```
public Archive(InputStream sourceStream)
```


नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्नलिखित उदाहरण एक एन्क्रिप्टेड आर्काइव को निकालता है, फिर पहले एंट्री को `ByteArrayOutputStream` में डीकम्प्रेस करता है।

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
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

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
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

यह कंस्ट्रक्टर किसी भी एंट्री को डीकम्प्रेस नहीं करता है। डीकम्प्रेस करने के लिए देखें [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत। |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्नलिखित उदाहरण एक एन्क्रिप्टेड आर्काइव को निकालता है, फिर पहले एंट्री को `ByteArrayOutputStream` में डीकम्प्रेस करता है।

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
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

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, the most common Deflate compression without encryption would be used. |

### Archive(String path) {#Archive-java.lang.String-}
```
public Archive(String path)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को डीकम्प्रेस नहीं करता है। डीकम्प्रेस करने के लिए देखें [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |

### Archive(String path, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String path, ArchiveLoadOptions loadOptions)
```


नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्नलिखित उदाहरण एक एन्क्रिप्टेड आर्काइव को निकालता है, फिर पहले एंट्री को `ByteArrayOutputStream` में डीकम्प्रेस करता है।

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive("encrypted.zip", options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |

### Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को डीकम्प्रेस नहीं करता है। डीकम्प्रेस करने के लिए देखें [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | नए जोड़े गए [ArchiveEntry](../../com.aspose.zip/archiveentry) आइटमों के लिए उपयोग किए जाने वाले संपीड़न और एन्क्रिप्शन सेटिंग्स। यदि निर्दिष्ट नहीं किया गया, तो सबसे सामान्य Deflate संपीड़न बिना एन्क्रिप्शन के उपयोग किया जाएगा। |

### Archive(String mainSegment, String[] segmentsInOrder) {#Archive-java.lang.String-java.lang.String---}
```
public Archive(String mainSegment, String[] segmentsInOrder)
```


मल्टी-वॉल्यूम ज़िप आर्काइव से नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```

``````

try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
a.extractToDirectory("destination");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mainSegment | java.lang.String | Path to the last segment of multi-volume archive with the central directory.

Usually this segment has \*.zip extension and smaller than others. |
| segmentsInOrder | java.lang.String[] | Paths to each segment but the last of multi-volume zip archive respecting order.

Usually they named filename.z01, filename.z02, ..., filename.z(n-1). |

### Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class from multi-volume ZIP archive and composes an entry list can be extracted from the archive.

This sample extract to a directory an archive of three segments.

```

``````

     try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
         a.extractToDirectory("destination");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | mainSegment | java.lang.String | केंद्रीय निर्देशिका वाले मल्टी-वॉल्यूम आर्काइव के अंतिम सेगमेंट का पथ। |

आमतौर पर इस सेगमेंट का \*.zip एक्सटेंशन होता है और यह अन्य से छोटे होते हैं। |
|  | segmentsInOrder | java.lang.String[] | मल्टी-वॉल्यूम ज़िप आर्काइव के प्रत्येक सेगमेंट (अंतिम को छोड़कर) के पथ, क्रम का सम्मान करते हुए। |

आमतौर पर उनका नाम filename.z01, filename.z02, ..., filename.z(n-1) होता है। |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final Archive createEntries(File directory)
```


दिए गए डायरेक्टरी में सभी फ़ाइलों और डायरेक्टरीज़ को पुनरावृत्त रूप से आर्काइव में जोड़ें।

```

``````

try (Archive archive = new Archive()) {
java.io.File folder = new java.io.File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final Archive createEntries(File directory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        java.io.File folder = new java.io.File("C:\\folder");
        archive.createEntries(folder);
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संकुचित करने के लिए डायरेक्टरी। |
| includeRootDirectory | बूलियन | यह दर्शाता है कि रूट डायरेक्टरी को स्वयं शामिल करना है या नहीं। |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final Archive createEntries(String sourceDirectory)
```


दिए गए डायरेक्टरी में सभी फ़ाइलों और डायरेक्टरीज़ को पुनरावृत्त रूप से आर्काइव में जोड़ें।

```

``````

try (Archive archive = new Archive()) {
archive.createEntries("C:\\folder");
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final Archive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntries("C:\\folder");
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | संकुचित करने के लिए डायरेक्टरी। |
| includeRootDirectory | बूलियन | यह दर्शाता है कि रूट डायरेक्टरी को स्वयं शामिल करना है या नहीं। |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final ArchiveEntry createEntry(String name, File file)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

विभिन्न एन्क्रिप्शन विधियों और पासवर्ड के साथ प्रत्येक एंट्री को एन्क्रिप्ट करके आर्काइव बनाएं।

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different encryption methods and passwords each.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

एंट्री का नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `file` पैरामीटर में दिया गया फ़ाइल नाम एंट्री के नाम को प्रभावित नहीं करता।

यदि फ़ाइल को `openImmediately` पैरामीटर के साथ तुरंत खोला जाता है तो यह आर्काइव सहेजे जाने तक अवरुद्ध रहती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| फ़ाइल | java.io.File | संकुचित की जाने वाली फ़ाइल का मेटाडेटा। |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें। |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

विभिन्न एन्क्रिप्शन विधियों और पासवर्ड के साथ प्रत्येक एंट्री को एन्क्रिप्ट करके आर्काइव बनाएं।

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final ArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.zip");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम। |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save("archive.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {
                    0x00,
                    (byte) 0xFF
            }), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new java.io.File("data1.bin"));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

एंट्री का नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `file` पैरामीटर में दिया गया फ़ाइल नाम एंट्री के नाम को प्रभावित नहीं करता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम। |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | जोड़े गए [ArchiveEntry](../../com.aspose.zip/archiveentry) आइटम के लिए उपयोग किए गए संपीड़न और एन्क्रिप्शन सेटिंग्स। |
| फ़ाइल | java.io.File | संपीड़ित किए जाने वाले फ़ाइल या फ़ोल्डर की मेटाडेटा। |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final ArchiveEntry createEntry(String name, String path)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

एंट्री नाम केवल `name` पैरामीटर में सेट किया जाता है। `path` पैरामीटर में दिया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

यदि फ़ाइल को `openImmediately` पैरामीटर के साथ तुरंत खोला जाता है तो यह आर्काइव सहेजे जाने तक अवरुद्ध रहती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| path | java.lang.String | नए फ़ाइल का पूर्ण योग्य नाम, या संपीड़ित किए जाने वाला सापेक्ष फ़ाइल नाम। |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें। |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

     Supplier<InputStream> provider = new Supplier<InputStream>() {
         public InputStream get() {
             return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
         }
     };
     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
             archive.save(zipFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | एंट्री के लिए इनपुट स्ट्रीम प्रदान करने वाला मेथड |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, ArchiveEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

एन्क्रिप्टेड एंट्री के साथ आर्काइव बनाएं।

```

``````

Supplier<InputStream> provider = new Supplier<InputStream>() {
public InputStream get() {
return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
}
};
try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.save(zipFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | the method providing input stream for the entry |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### deleteEntry(ArchiveEntry entry) {#deleteEntry-com.aspose.zip.ArchiveEntry-}
```
public final Archive deleteEntry(ArchiveEntry entry)
```


Removes the first occurrence of the specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        while (archive.getEntries().size() > 1)
            archive.deleteEntry(archive.getEntries().get(0));
        archive.save("last_entry.zip");
    }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | सूची में से हटाने के लिए प्रविष्टि। |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final Archive deleteEntry(int entryIndex)
```


इंडेक्स द्वारा एंट्री सूची से एंट्री को हटाता है।

```

``````

try (Archive archive = new Archive("two_files.zip")) {
archive.deleteEntry(0);
archive.save("single_file.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | The zero-based index of the entry to remove. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        archive.extractToDirectory("C:\\extracted");
    }
 
```

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाली निर्देशिका का पथ। |

### getComment() {#getComment--}
```
public final String getComment()
```


पूरे आर्काइव के लिए टिप्पणी प्राप्त करता है।

यदि `ArchiveLoadOptions.Encoding`([ArchiveLoadOptions.getEncoding](../../com.aspose.zip/archiveloadoptions\#getEncoding)/[ArchiveLoadOptions.setEncoding](../../com.aspose.zip/archiveloadoptions\#setEncoding)) प्रदान किया गया है, तो इसे उपयोग करके डिकोड किया जाता है। अन्यथा, UTF-8 का उपयोग किया जाता है।

**Returns:**
java.lang.String - संपूर्ण अभिलेख के लिए टिप्पणी।
### getEntries() {#getEntries--}
```
public final List<ArchiveEntry> getEntries()
```


[ArchiveEntry](../../com.aspose.zip/archiveentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं।

**Returns:**
java.util.List&lt;com.aspose.zip.ArchiveEntry&gt; - अभिलेख बनाते हुए [ArchiveEntry](../../com.aspose.zip/archiveentry) प्रकार की प्रविष्टियाँ।
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - अभिलेख बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ।
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


आर्काइव फ़ॉर्मेट (Zip) प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - Zip archive format.
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final ArchiveEntrySettings getNewEntrySettings()
```


नए जोड़े गए [ArchiveEntry](../../com.aspose.zip/archiveentry) आइटम्स के लिए उपयोग किए गए संपीड़न और एन्क्रिप्शन सेटिंग्स।

**Returns:**
[ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) - the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) instance
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

`outputStream` must be writable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream. |

### save(OutputStream outputStream, ArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(OutputStream outputStream, ArchiveSaveOptions saveOptions)
```


Saves archive to the stream provided.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry.bin", "data.bin");
            archive.save(zipFile);
        }
    } catch (IOException ex) {
    }
 
```

`outputStream` लिखने योग्य होना चाहिए।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | java.io.OutputStream | गंतव्य स्ट्रीम। |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | अभिलेख सहेजने के विकल्प। |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncoding(StandardCharsets.US_ASCII);
archive.save("archive.zip", options);
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, ArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(String destinationFileName, ArchiveSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncoding(StandardCharsets.US_ASCII);
        archive.save("archive.zip", options);
    }
 
```

एक अभिलेख को उसी पथ पर सहेजना संभव है जिससे इसे लोड किया गया था। हालांकि, यह अनुशंसित नहीं है क्योंकि यह तरीका अस्थायी फ़ाइल में कॉपी करने का उपयोग करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | निर्माण किए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित किया जाएगा। |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | अभिलेख सहेजने के विकल्प। |

### saveSplit(String destinationDirectory, SplitArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)
```


मल्टी-वॉल्यूम आर्काइव को प्रदान किए गए गंतव्य डायरेक्टरी में सहेजता है।

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.saveSplit( "C:\\Folder", new SplitArchiveSaveOptions("volume", 65536));
}
 
```

This method composes several (n) files filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Cannot make existing archive multi-volume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory where archive segments to be created. |
| options | [SplitArchiveSaveOptions](../../com.aspose.zip/splitarchivesaveoptions) | Options for archive saving, including file name. |

