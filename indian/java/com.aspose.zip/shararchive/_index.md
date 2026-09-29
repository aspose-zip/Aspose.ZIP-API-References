---
title: "SharArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह वर्ग एक shar संग्रह फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 119
url: /hi/java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

यह वर्ग एक shar संग्रह फ़ाइल का प्रतिनिधित्व करता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SharArchive()](#SharArchive--) | नया [SharArchive](../../com.aspose.zip/shararchive) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है। |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | डिकम्प्रेसिंग के लिए तैयार नया [SharArchive](../../com.aspose.zip/shararchive) क्लास का इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | एंट्री सूची से एक विशिष्ट एंट्री की पहली घटना को हटाता है। |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | इंडेक्स द्वारा एंट्री सूची से एंट्री को हटाता है। |
| [getEntries()](#getEntries--) | [SharEntry](../../com.aspose.zip/sharentry) प्रकार के एंट्रीज़ प्राप्त करता है जो आर्काइव बनाते हैं। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


नया [SharArchive](../../com.aspose.zip/shararchive) क्लास का एक इंस्टेंस इनिशियलाइज़ करता है।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संकुचित करने के लिए निर्देशिका |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | संकुचित करने के लिए निर्देशिका |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| फ़ाइल | java.io.File | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

java.io.File file = new java.io.File("data.bin");
try (SharArchive archive = new SharArchive()) {
archive.createEntry(\"test.bin\", file);
archive.save("archive.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

एंट्री नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `sourcePath` पैरामीटर में प्रदान किया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

यदि फ़ाइल को `openImmediately` पैरामीटर के साथ तुरंत खोल दिया जाता है तो यह आर्काइव समाप्त होने तक ब्लॉक हो जाती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| sourcePath | java.lang.String | संकुचित की जाने वाली फ़ाइल का पथ |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


एंट्री सूची से एक विशिष्ट एंट्री की पहली घटना को हटाता है।

यहाँ बताया गया है कि आप अंतिम एंट्री को छोड़कर सभी एंट्रीज़ को कैसे हटा सकते हैं:

```

``````

try (SharArchive archive = new SharArchive("archive.shar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputSharFile.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entryIndex | int | हटाने के लिए एंट्री का शून्य-आधारित सूचकांक |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


[SharEntry](../../com.aspose.zip/sharentry) प्रकार के एंट्रीज़ प्राप्त करता है जो आर्काइव बनाते हैं।

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - आर्काइव बनाते हुए [SharEntry](../../com.aspose.zip/sharentry) प्रकार की प्रविष्टियाँ
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | निर्मित किए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे ओवरराइट किया जाएगा। |

एक आर्काइव को उसी पथ पर सहेजना संभव है जिससे इसे लोड किया गया था। हालांकि, यह अनुशंसित नहीं है क्योंकि यह विधि अस्थायी फ़ाइल में कॉपी करने का उपयोग करती है |

