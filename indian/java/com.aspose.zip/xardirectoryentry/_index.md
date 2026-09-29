---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "xar संग्रह के भीतर निर्देशिका प्रविष्टि का प्रतिनिधित्व करता है।"
type: docs
weight: 139
url: /hi/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

xar संग्रह के भीतर निर्देशिका प्रविष्टि का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | वर्तमान निर्देशिका की सभी फ़ाइलों को प्रदान किए गए निर्देशिका में निकालता है। |
| [getAllEntries()](#getAllEntries--) | डायरेक्टरी को पुनरावर्ती रूप से बनाते हुए [XarEntry](../../com.aspose.zip/xarentry) प्रकार के सभी प्रविष्टियों को प्राप्त करता है। |
| [getDirectories()](#getDirectories--) | डायरेक्टरी बनाते हुए [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) प्रकार के प्रविष्टियों को प्राप्त करता है। |
| [getFiles()](#getFiles--) | डायरेक्टरी बनाते हुए [XarFileEntry](../../com.aspose.zip/xarfileentry) प्रकार के प्रविष्टियों को प्राप्त करता है। |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | डायरेक्टरी बनाते हुए [XarEntry](../../com.aspose.zip/xarentry) प्रकार के प्रविष्टियों को प्राप्त करता है। |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


वर्तमान निर्देशिका की सभी फ़ाइलों को प्रदान किए गए निर्देशिका में निकालता है।

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
((XarDirectoryEntry)archive.getEntries().get(0)).extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getAllEntries() {#getAllEntries--}
```
public final Iterable<XarEntry> getAllEntries
```


Gets all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final Iterable<XarDirectoryEntry> getDirectories
```


Gets entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarDirectoryEntry&gt; - entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final Iterable<XarFileEntry> getFiles
```


Gets entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarFileEntry&gt; - entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<XarEntry> getFilesAndDirectories
```


Gets entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory
