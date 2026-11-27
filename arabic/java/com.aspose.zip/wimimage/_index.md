---
title: "WimImage"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل صورة واحدة داخل أرشيف wim."
type: docs
weight: 134
url: /ar/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

تمثل صورة واحدة داخل أرشيف wim.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات في الصورة إلى الدليل المحدد. |
| [getAllEntries()](#getAllEntries--) | يحصل على الإدخالات من نوع [WimEntry](../../com.aspose.zip/wimentry) التي تشكل الصورة بشكل متكرر. |
| [getEntry(String path)](#getEntry-java.lang.String-) | يحصل على الإدخال من نوع [WimEntry](../../com.aspose.zip/wimentry) لمسار معين. |
| [getParent()](#getParent--) | يحصل على الأرشيف الذي تنتمي إليه الصورة. |
| [getRootDirectory()](#getRootDirectory--) | يحصل على إدخال الدليل الجذر للصورة. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج جميع الملفات في الصورة إلى الدليل المحدد.

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
