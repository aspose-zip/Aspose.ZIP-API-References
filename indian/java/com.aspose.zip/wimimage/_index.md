---
title: "WimImage"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "wim संग्रह के भीतर एकल इमेज का प्रतिनिधित्व करता है।"
type: docs
weight: 134
url: /hi/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

wim संग्रह के भीतर एकल इमेज का प्रतिनिधित्व करता है।
## Methods

| Method | विवरण |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | छवि में सभी फ़ाइलों को प्रदान किए गए निर्देशिका में निकालता है। |
| [getAllEntries()](#getAllEntries--) | छवि को बनाते हुए [WimEntry](../../com.aspose.zip/wimentry) प्रकार की प्रविष्टियों को पुनरावर्ती रूप से प्राप्त करता है। |
| [getEntry(String path)](#getEntry-java.lang.String-) | दिए गए पथ के लिए [WimEntry](../../com.aspose.zip/wimentry) प्रकार की प्रविष्टि प्राप्त करता है। |
| [getParent()](#getParent--) | छवि से संबंधित अभिलेख प्राप्त करता है। |
| [getRootDirectory()](#getRootDirectory--) | छवि की मूल निर्देशिका प्रविष्टि प्राप्त करता है। |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


छवि में सभी फ़ाइलों को प्रदान किए गए निर्देशिका में निकालता है।

```

``````

try (WimArchive archive = new WimArchive("install.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
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


Gets entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the image recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the image recursively
### getEntry(String path) {#getEntry-java.lang.String-}
```
public final WimEntry getEntry(String path)
```


Gets the entry of [WimEntry](../../com.aspose.zip/wimentry) type for a given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of file or directory |

**Returns:**
[WimEntry](../../com.aspose.zip/wimentry) - the entry of [WimEntry](../../com.aspose.zip/wimentry) type
### getParent() {#getParent--}
```
public final WimArchive getParent()
```


Gets the archive the image belongs to.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the image belongs to
### getRootDirectory() {#getRootDirectory--}
```
public final WimDirectoryEntry getRootDirectory()
```


Gets the root directory entry of the image.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the root directory entry of the image
