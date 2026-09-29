---
title: "TarArchive"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "यह वर्ग एक tar संग्रह फ़ाइल का प्रतिनिधित्व करता है।"
type: docs
weight: 125
url: /hi/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

यह क्लास एक tar आर्काइव फ़ाइल का प्रतिनिधित्व करती है। इसका उपयोग tar आर्काइव को बनाने, निकालने या अपडेट करने के लिए करें।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [TarArchive()](#TarArchive--) | नए [TarArchive](../../com.aspose.zip/tararchive) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | नए [Archive](../../com.aspose.zip/archive) क्लास का एक नया उदाहरण आरंभ करता है और एक एंट्री सूची बनाता है जिसे आर्काइव से निकाला जा सकता है। |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | नए [TarArchive](../../com.aspose.zip/tararchive) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है। |
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
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | आर्काइव के भीतर एक एकल एंट्री बनाता है। |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | एंट्री सूची से एक विशिष्ट एंट्री की पहली घटना को हटाता है। |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | इंडेक्स द्वारा एंट्री सूची से एंट्री को हटाता है। |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | आर्काइव में सभी फ़ाइलों को प्रदान किए गए डायरेक्टरी में निकालता है। |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | प्रदान किए गए gzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | प्रदान किए गए gzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | प्रदान किए गए LZ4 आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | प्रदान किए गए LZ4 आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | प्रदान किए गए LZMA आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | प्रदान किए गए LZMA आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | प्रदान किए गए lzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | प्रदान किए गए lzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | प्रदान किए गए xz फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromXz(String path)](#fromXz-java.lang.String-) | प्रदान किए गए xz फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | प्रदान किए गए Z फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromZ(String path)](#fromZ-java.lang.String-) | प्रदान किए गए Z फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | प्रदान किए गए Zstandard आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | प्रदान किए गए Zstandard आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है। |
| [getEntries()](#getEntries--) | [TarEntry](../../com.aspose.zip/tarentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं। |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो tar आर्काइव बनाती हैं। |
| [getFormat()](#getFormat--) | अभिलेख प्रारूप को प्राप्त करता है। |
| [save(OutputStream output)](#save-java.io.OutputStream-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | आर्काइव को प्रदान किए गए स्ट्रीम में सहेजता है। |
| [save(String destinationFileName)](#save-java.lang.String-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है। |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | gzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | gzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | gzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | gzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | आर्काइव को LZ4 संपीड़न के साथ स्ट्रीम में सहेजता है। |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | आर्काइव को LZ4 संपीड़न के साथ स्ट्रीम में सहेजता है। |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | आर्काइव को पथ द्वारा फ़ाइल में LZ4 संपीड़न के साथ सहेजता है। |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | आर्काइव को पथ द्वारा फ़ाइल में LZ4 संपीड़न के साथ सहेजता है। |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | आर्काइव को LZMA संपीड़न के साथ स्ट्रीम में सहेजता है। |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | आर्काइव को LZMA संपीड़न के साथ स्ट्रीम में सहेजता है। |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | आर्काइव को पथ द्वारा फ़ाइल में lzma संपीड़न के साथ सहेजता है। |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | आर्काइव को पथ द्वारा फ़ाइल में lzma संपीड़न के साथ सहेजता है। |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | lzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | lzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | lzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | lzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Z संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Z संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Z संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Z संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Zstandard संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Zstandard संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है। |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Zstandard संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Zstandard संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है। |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


नए [TarArchive](../../com.aspose.zip/tararchive) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।

निम्नलिखित उदाहरण दिखाता है कि फ़ाइल को कैसे संपीड़ित किया जाए।

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

यह कंस्ट्रक्टर किसी भी एंट्री को अनपैक नहीं करता। अनपैक करने के लिए देखें [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) मेथड।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | java.io.InputStream | आर्काइव का स्रोत |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


नए [TarArchive](../../com.aspose.zip/tararchive) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और एक एंट्री सूची बनाता है जिसे संग्रह से निकाला जा सकता है।

निम्न उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे निकाला जाए।

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

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
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| डायरेक्टरी | java.io.File | संपीड़न के लिए निर्देशिका |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | java.lang.String | संपीड़न के लिए निर्देशिका |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

एंट्री का नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है। `file` पैरामीटर में दिया गया फ़ाइल नाम एंट्री के नाम को प्रभावित नहीं करता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| फ़ाइल | java.io.File | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

एंट्री का नाम केवल `name` पैरामीटर के भीतर सेट किया जाता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| source | java.io.InputStream | एंट्री के लिए इनपुट स्ट्रीम |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

एंट्री नाम केवल `name` पैरामीटर में सेट किया जाता है। `path` पैरामीटर में दिया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String | एंट्री का नाम |
| path | java.lang.String | संपीड़ित करने के लिए फ़ाइल का पथ |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


आर्काइव के भीतर एक एकल एंट्री बनाता है।

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | एंट्री को एंट्रीज़ सूची से हटाने के लिए |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


इंडेक्स द्वारा एंट्री सूची से एंट्री को हटाता है।

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

यदि निर्देशिका मौजूद नहीं है, तो इसे बनाया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationDirectory | java.lang.String | निकाले गए फ़ाइलों को रखने वाली डायरेक्टरी का पथ |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


प्रदान किए गए gzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: gzip आर्काइव इस मेथड के भीतर पूरी तरह से एक्सट्रैक्ट किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

कम्प्रेशन एल्गोरिदम की प्रकृति के कारण GZip एक्सट्रैक्शन स्ट्रीम सर्चेबल नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को एक्सट्रैक्ट करने की सुविधा प्रदान करता है, इसलिए इसे अंतर्निहित रूप से सर्चेबल स्ट्रीम पर काम करना पड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत। |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


प्रदान किए गए gzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: gzip आर्काइव इस मेथड के भीतर पूरी तरह से एक्सट्रैक्ट किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

कम्प्रेशन एल्गोरिदम की प्रकृति के कारण GZip एक्सट्रैक्शन स्ट्रीम सर्चेबल नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को एक्सट्रैक्ट करने की सुविधा प्रदान करता है, इसलिए इसे अंतर्निहित रूप से सर्चेबल स्ट्रीम पर काम करना पड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ। |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


प्रदान किए गए LZ4 आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: LZ4 आर्काइव इस मेथड के भीतर पूरी तरह से एक्सट्रैक्ट किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | source | java.io.InputStream | आर्काइव का स्रोत। |

LZ4 निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है। |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


प्रदान किए गए LZ4 आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: LZ4 आर्काइव इस मेथड के भीतर पूरी तरह से एक्सट्रैक्ट किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | आर्काइव फ़ाइल का पथ। |

LZ4 निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है। |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


प्रदान किए गए LZMA आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: LZMA आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

LZMA निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


प्रदान किए गए LZMA आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: LZMA आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

LZMA निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


प्रदान किए गए lzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: lzip आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

Lzip निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत। |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


प्रदान किए गए lzip आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: lzip आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

Lzip निष्कर्षण स्ट्रीम संपीड़न एल्गोरिदम की प्रकृति के कारण खोज योग्य नहीं है। Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ। |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


प्रदान किए गए xz फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: xz आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


प्रदान किए गए xz फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: xz आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

Tar आर्काइव मनमाने रिकॉर्ड को निकालने की सुविधा प्रदान करता है, इसलिए इसे आंतरिक रूप से खोज योग्य स्ट्रीम पर काम करना पड़ता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


प्रदान किए गए Z फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: Z आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


प्रदान किए गए Z फ़ॉर्मेट आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: Z आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


प्रदान किए गए Zstandard आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: Zstandard आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | java.io.InputStream | आर्काइव का स्रोत |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


प्रदान किए गए Zstandard आर्काइव को निकालता है और निकाले गए डेटा से [TarArchive](../../com.aspose.zip/tararchive) बनाता है।

महत्वपूर्ण: Zstandard आर्काइव इस विधि के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | आर्काइव फ़ाइल का पथ |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


[TarEntry](../../com.aspose.zip/tarentry) प्रकार की एंट्रीज़ प्राप्त करता है जो आर्काइव बनाती हैं।

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - आर्काइव बनाते हुए [TarEntry](../../com.aspose.zip/tarentry) प्रकार की प्रविष्टियाँ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की एंट्रीज़ प्राप्त करता है जो tar आर्काइव बनाती हैं।

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - टार आर्काइव बनाते हुए [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) प्रकार की प्रविष्टियाँ
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

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


आर्काइव को प्रदान किए गए गंतव्य फ़ाइल में सहेजता है।

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

एक आर्काइव को उसी पथ पर सहेजना संभव है जिससे इसे लोड किया गया था। हालांकि, यह अनुशंसित नहीं है क्योंकि यह तरीका अस्थायी फ़ाइल में कॉपी करने का उपयोग करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | java.lang.String | निर्मित किए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे ओवरराइट किया जाएगा। |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


gzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


gzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


आर्काइव को LZ4 संपीड़न के साथ स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


आर्काइव को पथ द्वारा फ़ाइल में LZ4 संपीड़न के साथ सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | निर्माण किए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित किया जाएगा। |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


आर्काइव को LZMA संपीड़न के साथ स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

महत्वपूर्ण: इस विधि में टार आर्काइव को पहले बनाया जाता है और फिर संकुचित किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम। |

`output` लिखने योग्य होना चाहिए |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


आर्काइव को पथ द्वारा फ़ाइल में lzma संपीड़न के साथ सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

महत्वपूर्ण: इस विधि में टार आर्काइव को पहले बनाया जाता है और फिर संकुचित किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग के प्रति सावधान रहें।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


lzip संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


lzip संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


xz संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


xz संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | विशिष्ट xz आर्काइव की सेटिंग्स का सेट: शब्दकोश आकार, ब्लॉक आकार, जांच प्रकार |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Z संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| आउटपुट | java.io.OutputStream | गंतव्य स्ट्रीम |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Z संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Zstandard संपीड़न के साथ संग्रह को स्ट्रीम में सहेजता है।

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Zstandard संपीड़न के साथ संग्रह को पथ द्वारा फ़ाइल में सहेजता है।

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | java.lang.String | बनाए जाने वाले आर्काइव का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर इशारा करता है, तो उसे अधिलेखित किया जाएगा |
| format | [TarFormat](../../com.aspose.zip/tarformat) | टार हेडर फ़ॉर्मेट को परिभाषित करता है। शून्य मान को संभव होने पर USTar के रूप में माना जाएगा। |

