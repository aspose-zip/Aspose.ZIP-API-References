---
title: "SevenZipArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह क्लास 7z अभिलेख फ़ाइल का प्रतिनिधित्व करती है।"
type: docs
weight: 104
url: /hi/java/com.aspose.zip/sevenziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class SevenZipArchive implements IArchive, AutoCloseable
```

यह क्लास 7z आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग 7z आर्काइव बनाने और निकालने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipArchive()](#SevenZipArchive--) | एंट्रीज़ के वैकल्पिक सेटिंग्स के साथ [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [SevenZipArchive(SevenZipEntrySettings newEntrySettings)](#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-) | एंट्रीज़ के वैकल्पिक सेटिंग्स के साथ [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [SevenZipArchive(InputStream sourceStream)](#SevenZipArchive-java.io.InputStream-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive(InputStream sourceStream, String password)](#SevenZipArchive-java.io.InputStream-java.lang.String-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive(String path)](#SevenZipArchive-java.lang.String-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive(String path, String password)](#SevenZipArchive-java.lang.String-java.lang.String-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)](#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive(String path, SevenZipLoadOptions options)](#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive(String[] parts)](#SevenZipArchive-java.lang.String---) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस मल्टी-वॉल्यूम 7z आर्काइव से इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [SevenZipArchive(String[] parts, String password)](#SevenZipArchive-java.lang.String---java.lang.String-) | [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस मल्टी-वॉल्यूम 7z आर्काइव से इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है। |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-) | आर्काइव के भीतर एक सिंगल एंट्री बनाएं। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [extractToDirectory(String destinationDirectory, String password)](#extractToDirectory-java.lang.String-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [getEntries()](#getEntries--) | [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो 7z आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [getNewEntrySettings()](#getNewEntrySettings--) | नए जोड़े गए [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) आइटम्स के लिए उपयोग किए जाने वाले कंप्रेशन और एन्क्रिप्शन सेटिंग्स। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | प्रदान किए गए स्ट्रीम में 7z आर्काइव को सहेजता है। |
| [save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-) | प्रदान किए गए स्ट्रीम में 7z आर्काइव को सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | संग्रह को प्रदान की गई गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-) | संग्रह को प्रदान की गई गंतव्य फ़ाइल में सहेजता है। |
| [saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-) | प्रदान किए गए गंतव्य डायरेक्टरी में मल्टी-वॉल्यूम आर्काइव को सहेजता है। |
### SevenZipArchive() {#SevenZipArchive--}
```
public SevenZipArchive()
```


एंट्रीज़ के वैकल्पिक सेटिंग्स के साथ [SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

निम्न उदाहरण दिखाता है कि डिफ़ॉल्ट सेटिंग्स के साथ एक सिंगल फ़ाइल को कैसे कंप्रेस करें: एन्क्रिप्शन के बिना LZMA कंप्रेशन।

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

LZMA compression without encryption would be used.

### SevenZipArchive(SevenZipEntrySettings newEntrySettings) {#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-}
```
public SevenZipArchive(SevenZipEntrySettings newEntrySettings)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class with optional settings for its entries.

The following example shows how to compress a single file with default settings: LZMA compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | नए जोड़े गए [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) आइटमों के लिए उपयोग किए जाने वाले संपीड़न और एन्क्रिप्शन सेटिंग्स। यदि निर्दिष्ट नहीं किया गया, तो एन्क्रिप्शन के बिना LZMA संपीड़न उपयोग किया जाएगा |

### SevenZipArchive(InputStream sourceStream) {#SevenZipArchive-java.io.InputStream-}
```
public SevenZipArchive(InputStream sourceStream)
```


[SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream(\"archive.7z\"))) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### SevenZipArchive(InputStream sourceStream, String password) {#SevenZipArchive-java.io.InputStream-java.lang.String-}
```
public SevenZipArchive(InputStream sourceStream, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\\#extractToDirectory-String--String-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |
| पासवर्ड | java.lang.String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। यदि फ़ाइल नाम एन्क्रिप्टेड हैं, तो यह मौजूद होना चाहिए |

### SevenZipArchive(String path) {#SevenZipArchive-java.lang.String-}
```
public SevenZipArchive(String path)
```


[SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(\"archive.7z\")) {
archive.extractToDirectory("C:\\extracted");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### SevenZipArchive(String path, String password) {#SevenZipArchive-java.lang.String-java.lang.String-}
```
public SevenZipArchive(String path, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\\#extractToDirectory-String--String-) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ |
| पासवर्ड | java.lang.String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। यदि फ़ाइल नाम एन्क्रिप्टेड हैं, तो यह मौजूद होना चाहिए |

### SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options) {#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)
```


[SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

एक एन्क्रिप्टेड आर्काइव निकालें। आगे बढ़ने के लिए अधिकतम 60 सेकंड की अनुमति दें, उस अवधि के बाद रद्द करें।

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword(\"Top$ecr3t\");
options.setCancellationFlag(cf);
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
try (SevenZipArchive a = new SevenZipArchive(new FileInputStream(\"archive.7z\"), options)) {
a.extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Options to load existing archive with.

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing. |

### SevenZipArchive(String path, SevenZipLoadOptions options) {#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(String path, SevenZipLoadOptions options)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

Extract an encrypted archive. Allow up to 60 seconds to proceed, cancel after that period.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setDecryptionPassword("Top$ecr3t");
         options.setCancellationFlag(cf);
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
             a.extractToDirectory("C:\\extracted");
         } catch (IOException ex) {
         }
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पूर्ण योग्य या सापेक्ष पथ। |
|  | options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | मौजूदा आर्काइव को लोड करने के विकल्प। |

यह कंस्ट्रक्टर किसी भी एंट्री को डिकम्प्रेस नहीं करता है। डिकम्प्रेस करने के लिए देखें [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\\#extractToDirectory-String--String-) मेथड। |

### SevenZipArchive(String[] parts) {#SevenZipArchive-java.lang.String---}
```
public SevenZipArchive(String[] parts)
```


[SevenZipArchive](../../com.aspose.zip/sevenziparchive) क्लास का नया इंस्टेंस मल्टी-वॉल्यूम 7z आर्काइव से इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new String[] { \"multi.7z.001\", \"multi.7z.002\", \"multi.7z.003\" } )) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parts | java.lang.String[] | paths to each segment of multi-volume 7z archive respecting order |

### SevenZipArchive(String[] parts, String password) {#SevenZipArchive-java.lang.String---java.lang.String-}
```
public SevenZipArchive(String[] parts, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class from multi-volume 7z archive and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| parts | java.lang.String[] | बहु-आयतन 7z आर्काइव के प्रत्येक खंड के पथ, क्रम का सम्मान करते हुए |
| पासवर्ड | java.lang.String | डिक्रिप्शन के लिए वैकल्पिक पासवर्ड। यदि फ़ाइल नाम एन्क्रिप्टेड हैं, तो यह मौजूद होना चाहिए |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SevenZipArchive createEntries(File directory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive()) {
File folder = new File(\"C:\\\\folder\");
archive.createEntries(folder);
archive.save(\"folder.7z\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SevenZipArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         File folder = new File("C:\\folder");
         archive.createEntries(folder);
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संपीड़न के लिए निर्देशिका |
| includeRootDirectory | बूलियन | यह दर्शाता है कि रूट डायरेक्टरी को स्वयं शामिल किया जाए या नहीं |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SevenZipArchive createEntries(String sourceDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

LZMA संपीड़न के साथ 7z आर्काइव बनाएं।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntries("C:\\folder");
archive.save(\"folder.7z\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SevenZipArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

Compose 7z archive with LZMA compression.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
         archive.createEntries("C:\\folder");
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | संपीड़न के लिए निर्देशिका |
| includeRootDirectory | बूलियन | यह दर्शाता है कि रूट डायरेक्टरी को स्वयं शामिल किया जाए या नहीं |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, File file)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

विभिन्न पासवर्ड के साथ एन्क्रिप्ट किए गए प्रविष्टियों के साथ आर्काइव बनाएं।

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different passwords each.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         File fi1 = new File("data1.bin");
         File fi2 = new File("data2.bin");
         File fi3 = new File("data3.bin");

         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
             archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
             archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

एंट्री का नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `file` पैरामीटर में दिया गया फ़ाइल नाम एंट्री के नाम को प्रभावित नहीं करता।

यदि फ़ाइल को `openImmediately` पैरामीटर के साथ तुरंत खोला जाता है तो यह आर्काइव सहेजे जाने तक अवरुद्ध रहती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| फ़ाइल | java.io.File | संपीड़ित की जाने वाली फ़ाइल का मेटाडेटा |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

विभिन्न पासवर्ड के साथ एन्क्रिप्ट किए गए प्रविष्टियों के साथ आर्काइव बनाएं।

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

Compose 7z archive with LZMA compression and encryption of all entries.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.7z");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

सभी प्रविष्टियों के LZMA संपीड़न और एन्क्रिप्शन के साथ 7z आर्काइव बनाएं।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
archive.save("archive.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with LZMA compressed encrypted entry.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF}), new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new File("data1.bin"));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

एंट्री का नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `file` पैरामीटर में दिया गया फ़ाइल नाम एंट्री के नाम को प्रभावित नहीं करता।

`file` निर्देशिका को संदर्भित कर सकता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | जोड़े गए [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) आइटम के लिए उपयोग किए गए संपीड़न और एन्क्रिप्शन सेटिंग्स। व्यक्तिगत संपीड़न सेटिंग्स सॉलिड संपीड़न के मामले में अनदेखी की जाती हैं, देखें `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |
| फ़ाइल | java.io.File | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final SevenZipArchiveEntry createEntry(String name, String path)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

एंट्री नाम केवल `name` पैरामीटर में सेट किया जाता है। `path` पैरामीटर में दिया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

यदि फ़ाइल को `openImmediately` पैरामीटर के साथ तुरंत खोला जाता है तो यह आर्काइव सहेजे जाने तक अवरुद्ध रहती है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| path | java.lang.String | नई फ़ाइल का पूर्ण योग्य नाम, या संपीड़ित की जाने वाली सापेक्ष फ़ाइल नाम। |
| openImmediately | बूलियन | सही, यदि फ़ाइल को तुरंत खोलना हो, अन्यथा आर्काइव सहेजते समय फ़ाइल खोलें |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

Compose archive with LZMA2 compressed encrypted entry.

```

``````

 System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
 using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
 {
     using (var archive = new SevenZipArchive())
     {
         archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
         archive.Save(sevenZipFile);
     }
 }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम। |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | प्रविष्टि के लिए इनपुट स्ट्रीम प्रदान करने वाली विधि। |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, SevenZipEntrySettings newEntrySettings)
```


आर्काइव के भीतर एक सिंगल एंट्री बनाएं।

LZMA2 संपीड़ित एन्क्रिप्टेड प्रविष्टि के साथ आर्काइव बनाएं।

```

``````

System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
using (var archive = new SevenZipArchive())
{
archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.Save(sevenZipFile);
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | Compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाले डायरेक्टरी का पथ। |

यदि डायरेक्टरी मौजूद नहीं है, तो इसे बनाया जाएगा |

### extractToDirectory(String destinationDirectory, String password) {#extractToDirectory-java.lang.String-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory, String password)
```


आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(\"archive.7z\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |
| password | java.lang.String | optional password for content decryption.

`password` is used for content decryption only. If file names are encrypted provide password in [SevenZipArchive(String, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-String--String-) or [SevenZipArchive(java.io.InputStream, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-java.io.InputStream--String-) constructor. |

### getEntries() {#getEntries--}
```
public final List<SevenZipArchiveEntry> getEntries()
```


Gets entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.SevenZipArchiveEntry&gt; - entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final SevenZipEntrySettings getNewEntrySettings()
```


Compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items.

**Returns:**
[SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) - compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves 7z archive to the stream provided.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (SevenZipArchive archive = new SevenZipArchive()) {
                 archive.createEntry("data", source);
                 archive.save(sevenZipFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम |

### save(OutputStream output, SevenZipArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)
```


प्रदान किए गए स्ट्रीम में 7z आर्काइव को सहेजता है।

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("data", source);
archive.save(sevenZipFile);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to a destination file provided.

```

``````

  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
     using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
     {
        archive.CreateEntry("data", source);
        archive.Save("archive.7z");
     }
  }
  
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | निर्माण किए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित किया जाएगा। |

एक संग्रह को उसी पथ पर सहेजना संभव है जिससे इसे लोड किया गया था। हालांकि, यह अनुशंसित नहीं है क्योंकि यह विधि अस्थायी फ़ाइल में कॉपी करने का उपयोग करती है। |

### save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)
```


संग्रह को प्रदान की गई गंतव्य फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data", source);
archive.save("archive.7z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```


Saves multi-volume archive to destination directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         archive.createEntry("entry.bin", "data.bin");
         archive.saveSplit("C:\\Folder", new SplitSevenZipArchiveSaveOptions("volume", 65536));
     }
 
```

यह विधि कई `(n)` फ़ाइलें बनाती है filename.7z.001, filename.7z.002, ..., filename.7z.(n).

मौजूदा संग्रह को मल्टी-वॉल्यूम नहीं बनाया जा सकता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | आर्काइव खंडों को बनाने के लिए निर्देशिका का पथ |
| options | [SplitSevenZipArchiveSaveOptions](../../com.aspose.zip/splitsevenziparchivesaveoptions) | आर्काइव सहेजने के विकल्प, जिसमें फ़ाइल नाम शामिल है |

