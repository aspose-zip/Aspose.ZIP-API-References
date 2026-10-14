---
title: "CpioArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास cpio अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 57
url: /hi/java/com.aspose.zip/cpioarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class CpioArchive implements IArchive, AutoCloseable
```

यह क्लास cpio अभिलेख फ़ाइल का प्रतिनिधित्व करती है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [CpioArchive()](#CpioArchive--) | एक नया उदाहरण प्रारंभ करता है [CpioArchive](../../com.aspose.zip/cpioarchive) क्लास का। |
| [CpioArchive(InputStream sourceStream)](#CpioArchive-java.io.InputStream-) | एक नया उदाहरण प्रारंभ करता है [CpioArchive](../../com.aspose.zip/cpioarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [CpioArchive(String path)](#CpioArchive-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है [CpioArchive](../../com.aspose.zip/cpioarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [deleteEntry(CpioEntry entry)](#deleteEntry-com.aspose.zip.CpioEntry-) | एंट्री सूची से एक विशिष्ट एंट्री की पहली घटना को हटाता है। |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | इंडेक्स द्वारा एंट्री सूची से एंट्री को हटाता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getEntries()](#getEntries--) | [CpioEntry](../../com.aspose.zip/cpioentry) प्रकार की एंट्री प्राप्त करता है जो cpio आर्काइव बनाती हैं। |
| [getFileEntries()](#getFileEntries--) | cpio संग्रह बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream output, CpioFormat cpioFormat)](#save-java.io.OutputStream-com.aspose.zip.CpioFormat-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, CpioFormat cpioFormat)](#save-java.lang.String-com.aspose.zip.CpioFormat-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | gzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveGzipped(OutputStream output, CpioFormat cpioFormat)](#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | gzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | gzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveGzipped(String path, CpioFormat cpioFormat)](#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-) | gzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | LZMA संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | LZMA संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | lzma संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveLZMACompressed(String path, CpioFormat cpioFormat)](#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-) | lzma संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | lzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveLzipped(OutputStream output, CpioFormat cpioFormat)](#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | lzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | lzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveLzipped(String path, CpioFormat cpioFormat)](#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-) | lzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveXzCompressed(String path, CpioFormat cpioFormat)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Z संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZCompressed(OutputStream output, CpioFormat cpioFormat)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Z संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Z संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZCompressed(String path, CpioFormat cpioFormat)](#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Z संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Zstandard संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZstandard(OutputStream output, CpioFormat cpioFormat)](#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Zstandard संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Zstandard संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZstandard(String path, CpioFormat cpioFormat)](#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-) | Zstandard संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
### CpioArchive() {#CpioArchive--}
```
public CpioArchive()
```


एक नया उदाहरण प्रारंभ करता है [CpioArchive](../../com.aspose.zip/cpioarchive) क्लास का।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```



### CpioArchive(InputStream sourceStream) {#CpioArchive-java.io.InputStream-}
```
public CpioArchive(InputStream sourceStream)
```


Initializes a new instance of the [CpioArchive](../../com.aspose.zip/cpioarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CpioArchive archive = new CpioArchive(new FileInputStream("archive.cpio"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर कोई भी प्रविष्टि अनपैक नहीं करता है। अनपैकिंग के लिए देखें [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### CpioArchive(String path) {#CpioArchive-java.lang.String-}
```
public CpioArchive(String path)
```


एक नया उदाहरण प्रारंभ करता है [CpioArchive](../../com.aspose.zip/cpioarchive) क्लास का और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CpioArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संपीड़न के लिए निर्देशिका |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CpioArchive createEntries(File directory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CpioArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | संपीड़न के लिए निर्देशिका |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CpioArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final CpioEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new File("data.bin");
     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| फ़ाइल | java.io.File | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final CpioEntry createEntry(String name, File file, boolean openImmediately)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

java.io.File file = new File(\"data.bin\");
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry(\"test.bin\", file);
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CpioEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.cpio");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final CpioEntry createEntry(String name, String sourcePath)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | path to file to be compressed. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final CpioEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.cpio");
     }
 
```

एंट्री नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `sourcePath` पैरामीटर में प्रदान किया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता है

`openImmediately` पैरामीटर के साथ फ़ाइल को तुरंत खोलने पर यह तब तक ब्लॉक हो जाता है जब तक आर्काइव को नष्ट नहीं किया जाता

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| sourcePath | java.lang.String | संपीड़ित की जाने वाली फ़ाइल का पथ। |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलें, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें। |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### deleteEntry(CpioEntry entry) {#deleteEntry-com.aspose.zip.CpioEntry-}
```
public final CpioArchive deleteEntry(CpioEntry entry)
```


एंट्री सूची से एक विशिष्ट एंट्री की पहली घटना को हटाता है।

यहाँ बताया गया है कि आप अंतिम एंट्री को छोड़कर सभी एंट्रीज़ को कैसे हटा सकते हैं:

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save(\"outputCpioFile.cpio\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [CpioEntry](../../com.aspose.zip/cpioentry) | the entry to remove from the entries list |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final CpioArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (CpioArchive archive = new CpioArchive("two_files.cpio")) {
         archive.deleteEntry(0);
         archive.save("single_file.cpio");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entryIndex | int | हटाने के लिए एंट्री का शून्य-आधारित सूचकांक |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है।

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<CpioEntry> getEntries()
```


Gets entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.

**Returns:**
java.util.List&lt;com.aspose.zip.CpioEntry&gt; - entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |

### save(OutputStream output, CpioFormat cpioFormat) {#save-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void save(OutputStream output, CpioFormat cpioFormat)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | निर्मित किए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे ओवरराइट किया जाएगा। |

एक आर्काइव को उसी पथ पर सहेजना संभव है जिससे इसे लोड किया गया था। हालांकि, यह अनुशंसित नहीं है क्योंकि यह विधि अस्थायी फ़ाइल में कॉपी करने का उपयोग करती है |

### save(String destinationFileName, CpioFormat cpioFormat) {#save-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void save(String destinationFileName, CpioFormat cpioFormat)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |

### saveGzipped(OutputStream output, CpioFormat cpioFormat) {#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(OutputStream output, CpioFormat cpioFormat)
```


gzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.cpio.gz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### saveGzipped(String path, CpioFormat cpioFormat) {#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(String path, CpioFormat cpioFormat)
```


gzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.cpio.gz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Saves the archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

महत्वपूर्ण: cpio आर्काइव इस मेथड के भीतर निर्मित और फिर संकुचित किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |

### saveLZMACompressed(OutputStream output, CpioFormat cpioFormat) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)
```


LZMA संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Saves the archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.cpio.lzma");
         }
     } catch (IOException ex) {
     }
 
```

महत्वपूर्ण: cpio आर्काइव इस मेथड के भीतर निर्मित और फिर संकुचित किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### saveLZMACompressed(String path, CpioFormat cpioFormat) {#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(String path, CpioFormat cpioFormat)
```


lzma संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.cpio.lzma");
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |

### saveLzipped(OutputStream output, CpioFormat cpioFormat) {#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(OutputStream output, CpioFormat cpioFormat)
```


lzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.cpio.lz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### saveLzipped(String path, CpioFormat cpioFormat) {#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(String path, CpioFormat cpioFormat)
```


lzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.cpio.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output`स्ट्रीम लिखने योग्य होना चाहिए |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat)
```


xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output`स्ट्रीम लिखने योग्य होना चाहिए। |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | cpio हेडर फ़ॉर्मेट को परिभाषित करता है |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | विशिष्ट xz आर्काइव की सेटिंग्स का सेट: शब्दकोश आकार, ब्लॉक आकार, जांच प्रकार |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveXzCompressed(String path, CpioFormat cpioFormat) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.cpio.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | cpio हेडर फ़ॉर्मेट को परिभाषित करता है |

### saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)
```


xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |

### saveZCompressed(OutputStream output, CpioFormat cpioFormat) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(OutputStream output, CpioFormat cpioFormat)
```


Z संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.cpio.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### saveZCompressed(String path, CpioFormat cpioFormat) {#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(String path, CpioFormat cpioFormat)
```


Z संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.cpio.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | d cpio header format |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |

### saveZstandard(OutputStream output, CpioFormat cpioFormat) {#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(OutputStream output, CpioFormat cpioFormat)
```


Zstandard संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.cpio.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### saveZstandard(String path, CpioFormat cpioFormat) {#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(String path, CpioFormat cpioFormat)
```


Zstandard संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.cpio.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

