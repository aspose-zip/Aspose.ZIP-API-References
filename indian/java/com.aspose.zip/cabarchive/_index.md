---
title: "CabArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास एक CAB अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 44
url: /hi/java/com.aspose.zip/cabarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.zip.ICompressionArchive, java.lang.AutoCloseable
```
public class CabArchive implements ICompressionArchive, AutoCloseable
```

यह क्लास एक CAB अभिलेख फ़ाइल का प्रतिनिधित्व करती है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [CabArchive(CabEntrySettings settings)](#CabArchive-com.aspose.zip.CabEntrySettings-) | कम्प्रेस करने के लिए तैयार [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [CabArchive(InputStream sourceStream)](#CabArchive-java.io.InputStream-) | आर्काइव से निकाली जा सकने वाली प्रविष्टियों की सूची बनाता हुआ [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)](#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-) | आर्काइव से निकाली जा सकने वाली प्रविष्टियों की सूची बनाता हुआ [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [CabArchive(String path)](#CabArchive-java.lang.String-) | आर्काइव से निकाली जा सकने वाली प्रविष्टियों की सूची बनाता हुआ [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [CabArchive(String path, CabLoadOptions loadOptions)](#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-) | आर्काइव से निकाली जा सकने वाली प्रविष्टियों की सूची बनाता हुआ [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | निर्दिष्ट डायरेक्टरी से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | निर्दिष्ट डायरेक्टरी से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | निर्दिष्ट डायरेक्टरी पाथ से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | निर्दिष्ट डायरेक्टरी पाथ से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है। |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-) | आर्काइव के भीतर एक एकल प्रविष्टि और विशिष्ट सेटिंग्स बनाएं। |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, String path, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getEntries()](#getEntries--) | [CabEntry](../../com.aspose.zip/cabentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो कैब आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream outputStream, CabSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-) | विशिष्ट विकल्पों के साथ प्रदान किए गए स्ट्रीम में आर्काइव को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, CabSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.CabSaveOptions-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
### CabArchive(CabEntrySettings settings) {#CabArchive-com.aspose.zip.CabEntrySettings-}
```
public CabArchive(CabEntrySettings settings)
```


कम्प्रेस करने के लिए तैयार [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

विशिष्ट संपीड़न सेटिंग्स का उपयोग करके फ़ाइल को संपीड़ित करें।

```

``````

CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings()));
try (CabArchive archive = new CabArchive(settings))
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | the source of the archive |

### CabArchive(InputStream sourceStream) {#CabArchive-java.io.InputStream-}
```
public CabArchive(InputStream sourceStream)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को अनपैक नहीं करता। अनपैकिंग के लिए देखें [CabEntry.open()](../../com.aspose.zip/cabentry\\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### CabArchive(InputStream sourceStream, CabLoadOptions loadOptions) {#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)
```


आर्काइव से निकाली जा सकने वाली प्रविष्टियों की सूची बनाता हुआ [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### CabArchive(String path) {#CabArchive-java.lang.String-}
```
public CabArchive(String path)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को अनपैक नहीं करता। अनपैकिंग के लिए देखें [CabEntry.open()](../../com.aspose.zip/cabentry\\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

### CabArchive(String path, CabLoadOptions loadOptions) {#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(String path, CabLoadOptions loadOptions)
```


आर्काइव से निकाली जा सकने वाली प्रविष्टियों की सूची बनाता हुआ [CabArchive](../../com.aspose.zip/cabarchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CabArchive createEntries(File directory)
```


Adds to the archive all files, recursively, from the specified directory.

```

``````

 try (var archive = new CabArchive())
 {
     File directory = new File("C:/Logs");
     archive.createEntries(directory);
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संकुचित करने के लिए डायरेक्टरी। |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CabArchive createEntries(File directory, boolean includeRootDirectory)
```


निर्दिष्ट डायरेक्टरी से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (var archive = new CabArchive())
{
File directory = new File("C:/Logs");
archive.createEntries(directory, false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CabArchive createEntries(String sourceDirectory)
```


Adds to the archive all files recursively from the specified directory path.

```

``````

 try (var archive = new CabArchive())
 {
     archive.createEntries("C:/Logs");
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | कम्प्रेस करने के लिए डायरेक्टरी पाथ। |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CabArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


निर्दिष्ट डायरेक्टरी पाथ से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (var archive = new CabArchive())
{
archive.createEntries("C:/Logs", false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory path to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final CabEntry createEntry(String name, File fileInfo)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     var sourceFile = new java.io.File("logs\\log.txt");
     archive.createEntry("log.txt", sourceFile);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
|  | fileInfo | java.io.File | संकुचित की जाने वाली फ़ाइल का मेटाडेटा। |

एंट्री नाम केवल `name` पैरामीटर में सेट किया जाता है। `fileInfo` पैरामीटर में प्रदान किया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता। |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
File sourceFile = new File("logs\\log.txt");
archive.createEntry("log.txt", sourceFile, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| fileInfo | java.io.File | The metadata of file to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `fileInfo` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CabEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
 {
     archive.createEntry("stream-entry.bin", stream);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम। |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, InputStream source, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल प्रविष्टि और विशिष्ट सेटिंग्स बनाएं।

```

``````

try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
{
CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings());
archive.createEntry("stream-entry.bin", stream, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final CabEntry createEntry(String name, String path)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("entry.bin", "data.bin");
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
|  | path | java.lang.String | नए फ़ाइल का पूर्ण योग्य नाम, या संपीड़ित किए जाने वाला सापेक्ष फ़ाइल नाम। |

एंट्री का नाम केवल `name` पैरामीटर में सेट किया जाता है। `path` पैरामीटर में प्रदान किया गया फ़ाइल नाम एंट्री के नाम को प्रभावित नहीं करता। |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, String path, CabEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry(\"entry.bin\", \"data.bin\", settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("log.txt", () -> new FileInputStream("log.txt"));
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | प्रविष्टि के लिए इनपुट स्ट्रीम प्रदान करने वाली विधि। |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider, CabEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry(\"log.txt\", () -> new FileInputStream(\"log.txt\"), settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाले डायरेक्टरी का पथ। |

यदि डायरेक्टरी मौजूद नहीं है, तो इसे बनाया जाएगा |

### getEntries() {#getEntries--}
```
public final List<CabEntry> getEntries()
```


[CabEntry](../../com.aspose.zip/cabentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो आर्काइव बनाती हैं।

**Returns:**
java.util.List&lt;com.aspose.zip.CabEntry&gt; - आर्काइव बनाते हुए [CabEntry](../../com.aspose.zip/cabentry) प्रकार के प्रविष्टियाँ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियों को प्राप्त करता है जो कैब आर्काइव बनाती हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - cab आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


अभिलेख प्रारूप को प्राप्त करता है।

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है।

```

``````

try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream(\"archive.cab\"))
{
archive.createEntry("entry.bin", "data.bin");
archive.save(cabFile);
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream.

`outputStream` must be writable. |

### save(OutputStream outputStream, CabSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-}
```
public final void save(OutputStream outputStream, CabSaveOptions saveOptions)
```


Saves archive to the stream provided with specific options.

```

``````

  try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream("archive.cab"))
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save(cabFile, options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | java.io.OutputStream | गंतव्य स्ट्रीम। |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | अभिलेख सहेजने के विकल्प। |

`outputStream` लिखने योग्य होना चाहिए। |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (CabArchive archive = new CabArchive())
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### save(String destinationFileName, CabSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.CabSaveOptions-}
```
public final void save(String destinationFileName, CabSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

  try (CabArchive archive = new CabArchive())
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save("archive.cab", options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | निर्माण किए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित किया जाएगा। |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | अभिलेख सहेजने के विकल्प। |

एक संग्रह को उसी पथ पर सहेजना संभव है जिससे इसे लोड किया गया था। हालांकि, यह अनुशंसित नहीं है क्योंकि यह विधि अस्थायी फ़ाइल में कॉपी करने का उपयोग करती है। |

