---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Xar arşivindeki dizin girişini temsil eder."
type: docs
weight: 139
url: /tr/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

Xar arşivindeki dizin girişini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mevcut dizindeki tüm dosyaları belirtilen dizine çıkarır. |
| [getAllEntries()](#getAllEntries--) | [XarEntry](../../com.aspose.zip/xarentry) tipindeki tüm girdileri, dizini oluşturacak şekilde, yinelemeli olarak alır. |
| [getDirectories()](#getDirectories--) | [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) tipindeki girdileri, dizini oluşturacak şekilde alır. |
| [getFiles()](#getFiles--) | [XarFileEntry](../../com.aspose.zip/xarfileentry) tipindeki girdileri, dizini oluşturacak şekilde alır. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | [XarEntry](../../com.aspose.zip/xarentry) tipindeki girdileri, dizini oluşturacak şekilde alır. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mevcut dizindeki tüm dosyaları belirtilen dizine çıkarır.

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
