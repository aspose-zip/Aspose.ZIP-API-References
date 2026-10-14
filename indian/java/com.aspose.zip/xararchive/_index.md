---
title: "XarArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह वर्ग एक xar संग्रह फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 136
url: /hi/java/com.aspose.zip/xararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XarArchive implements IArchive, AutoCloseable
```

यह वर्ग एक xar संग्रह फ़ाइल का प्रतिनिधित्व करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [XarArchive()](#XarArchive--) | [XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [XarArchive(XarCompressionSettings defaultCompressionSettings)](#XarArchive-com.aspose.zip.XarCompressionSettings-) | [XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है। |
| [XarArchive(InputStream sourceStream)](#XarArchive-java.io.InputStream-) | [XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)](#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-) | [XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [XarArchive(String path)](#XarArchive-java.lang.String-) | [XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
| [XarArchive(String path, XarLoadOptions loadOptions)](#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-) | [XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [deleteEntry(XarEntry entry)](#deleteEntry-com.aspose.zip.XarEntry-) | एंट्री सूची से एक विशिष्ट एंट्री की पहली घटना को हटाता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getEntries()](#getEntries--) | आर्काइव बनाते हुए [XarEntry](../../com.aspose.zip/xarentry) प्रकार के प्रविष्टियों को प्राप्त करता है। |
| [getFileEntries()](#getFileEntries--) | xar आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream output, XarSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, XarSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.XarSaveOptions-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
### XarArchive() {#XarArchive--}
```
public XarArchive()
```


[XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```



### XarArchive(XarCompressionSettings defaultCompressionSettings) {#XarArchive-com.aspose.zip.XarCompressionSettings-}
```
public XarArchive(XarCompressionSettings defaultCompressionSettings)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class.

The following example shows how to compress a file.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| defaultCompressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | डिफ़ॉल्ट संपीड़न सेटिंग्स, जो आर्काइव की सभी प्रविष्टियों पर लागू होती हैं। |

### XarArchive(InputStream sourceStream) {#XarArchive-java.io.InputStream-}
```
public XarArchive(InputStream sourceStream)
```


[XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### XarArchive(InputStream sourceStream, XarLoadOptions loadOptions) {#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर कोई भी प्रविष्टि अनपैक नहीं करता है। अनपैक करने के लिए देखें [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | आर्काइव लोड करने के विकल्प। |

### XarArchive(String path) {#XarArchive-java.lang.String-}
```
public XarArchive(String path)
```


[XarArchive](../../com.aspose.zip/xararchive) क्लास का नया उदाहरण प्रारंभ करता है और एक प्रविष्टि सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### XarArchive(String path, XarLoadOptions loadOptions) {#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(String path, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

यह कंस्ट्रक्टर कोई भी प्रविष्टि अनपैक नहीं करता है। अनपैक करने के लिए देखें [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | आर्काइव लोड करने के विकल्प। |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final XarArchive createEntries(File directory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संपीड़न के लिए निर्देशिका |
| includeRootDirectory | बूलियन | यह दर्शाता है कि रूट डायरेक्टरी को स्वयं शामिल किया जाए या नहीं |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final XarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | संपीड़न के लिए निर्देशिका |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(xarFile);
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
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | संपीड़न के लिए निर्देशिका |
| includeRootDirectory | बूलियन | यह दर्शाता है कि रूट डायरेक्टरी को स्वयं शामिल किया जाए या नहीं |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | जोड़े गए [XarEntry](../../com.aspose.zip/xarentry) आइटमों के लिए उपयोग किए गए संपीड़न सेटिंग्स |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final XarEntry createEntry(String name, File file)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry(\"test.bin\", file);
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.xar");
     }
 
```

`openImmediately` पैरामीटर के साथ फ़ाइल को तुरंत खोलने पर यह तब तक ब्लॉक हो जाता है जब तक आर्काइव को नष्ट नहीं किया जाता

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| फ़ाइल | java.io.File | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा |
| openImmediately | बूलियन | यदि फ़ाइल को तुरंत खोलें तो true, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें। |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry(\"test.bin\", file);
archive.save("archive.xar");
}
 
```

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final XarEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.xar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", new FileInputStream("data.bin"));
archive.save("archive.xar");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final XarEntry createEntry(String name, String sourcePath)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

एंट्री नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `sourcePath` पैरामीटर में प्रदान किया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| sourcePath | java.lang.String | संपीड़ित की जाने वाली फ़ाइल का पथ |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

एंट्री नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `sourcePath` पैरामीटर में प्रदान किया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

यदि फ़ाइल को `openImmediately` पैरामीटर के साथ तुरंत खोल दिया जाता है तो यह आर्काइव समाप्त होने तक ब्लॉक हो जाती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| sourcePath | java.lang.String | संपीड़ित की जाने वाली फ़ाइल का पथ |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | जोड़े गए [XarEntry](../../com.aspose.zip/xarentry) आइटम के लिए उपयोग किए गए संपीड़न सेटिंग्स |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### deleteEntry(XarEntry entry) {#deleteEntry-com.aspose.zip.XarEntry-}
```
public final XarArchive deleteEntry(XarEntry entry)
```


एंट्री सूची से एक विशिष्ट एंट्री की पहली घटना को हटाता है।

यहाँ बताया गया है कि आप अंतिम एंट्री को छोड़कर सभी एंट्रीज़ को कैसे हटा सकते हैं:

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputXarFile.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | the entry to remove from the entries list |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाले डायरेक्टरी का पथ। |

यदि डायरेक्टरी मौजूद नहीं है, तो इसे बनाया जाएगा |

### getEntries() {#getEntries--}
```
public final List<XarEntry> getEntries()
```


आर्काइव बनाते हुए [XarEntry](../../com.aspose.zip/xarentry) प्रकार के प्रविष्टियों को प्राप्त करता है।

**Returns:**
java.util.List&lt;com.aspose.zip.XarEntry&gt; - आर्काइव बनाते हुए [XarEntry](../../com.aspose.zip/xarentry) प्रकार के एंट्रीज़
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


xar आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के प्रविष्टियों को प्राप्त करता है।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - xar आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार के एंट्रीज़
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

बड़े आर्काइव के लिए java.io.FileOutputStream में सहेजने के बजाय [save(String)](../../com.aspose.zip/xararchive\#save-String-) का उपयोग करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम |

### save(OutputStream output, XarSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-}
```
public final void save(OutputStream output, XarSaveOptions saveOptions)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

बड़े आर्काइव के लिए java.io.FileOutputStream में सहेजने के बजाय [save(String)](../../com.aspose.zip/xararchive\#save-String-) का उपयोग करें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | xar आर्काइव को सहेजने के विकल्प |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### save(String destinationFileName, XarSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.XarSaveOptions-}
```
public final void save(String destinationFileName, XarSaveOptions saveOptions)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | xar आर्काइव को सहेजने के विकल्प |

