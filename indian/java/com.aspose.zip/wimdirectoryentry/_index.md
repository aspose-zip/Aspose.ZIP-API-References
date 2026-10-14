---
title: "WimDirectoryEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "wim संग्रह के भीतर एकल निर्देशिका का प्रतिनिधित्व करता है।"
type: docs
weight: 131
url: /hi/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

wim संग्रह के भीतर एकल निर्देशिका का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | वर्तमान निर्देशिका की सभी फ़ाइलों को प्रदान किए गए निर्देशिका में निकालता है। |
| [getAllEntries()](#getAllEntries--) | डायरेक्टरी बनाते हुए [WimEntry](../../com.aspose.zip/wimentry) प्रकार की सभी प्रविष्टियों को पुनरावर्ती रूप से प्राप्त करता है। |
| [getDirectories()](#getDirectories--) | डायरेक्टरी बनाते हुए [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) प्रकार की प्रविष्टियों को प्राप्त करता है। |
| [getFiles()](#getFiles--) | डायरेक्टरी बनाते हुए [WimFileEntry](../../com.aspose.zip/wimfileentry) प्रकार की प्रविष्टियों को प्राप्त करता है। |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | डायरेक्टरी बनाते हुए [WimEntry](../../com.aspose.zip/wimentry) प्रकार की प्रविष्टियों को प्राप्त करता है। |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


वर्तमान निर्देशिका की सभी फ़ाइलों को प्रदान किए गए निर्देशिका में निकालता है।

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getAllEntries() {#getAllEntries--}
```
public final Iterable<WimEntry> getAllEntries()
```


Gets all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final List<WimDirectoryEntry> getDirectories()
```


Gets entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimDirectoryEntry&gt; - entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final List<WimFileEntry> getFiles()
```


Gets entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimFileEntry&gt; - entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<WimEntry> getFilesAndDirectories()
```


Gets entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory
