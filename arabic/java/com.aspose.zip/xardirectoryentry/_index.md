---
title: "XarDirectoryEntry"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "تمثل إدخال دليل داخل أرشيف xar."
type: docs
weight: 139
url: /ar/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

تمثل إدخال دليل داخل أرشيف xar.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | يستخرج جميع الملفات في الدليل الحالي إلى الدليل المحدد. |
| [getAllEntries()](#getAllEntries--) | يحصل على جميع الإدخالات من نوع [XarEntry](../../com.aspose.zip/xarentry) التي تشكل الدليل بشكل متكرر. |
| [getDirectories()](#getDirectories--) | يحصل على الإدخالات من نوع [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) التي تشكل الدليل. |
| [getFiles()](#getFiles--) | يحصل على الإدخالات من نوع [XarFileEntry](../../com.aspose.zip/xarfileentry) التي تشكل الدليل. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | يحصل على الإدخالات من نوع [XarEntry](../../com.aspose.zip/xarentry) التي تشكل الدليل. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


يستخرج جميع الملفات في الدليل الحالي إلى الدليل المحدد.

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
public final Iterable<XarEntry> getAllEntries()
```


Gets all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final Iterable<XarDirectoryEntry> getDirectories()
```


Gets entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarDirectoryEntry&gt; - entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final Iterable<XarFileEntry> getFiles()
```


Gets entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarFileEntry&gt; - entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<XarEntry> getFilesAndDirectories()
```


Gets entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory
