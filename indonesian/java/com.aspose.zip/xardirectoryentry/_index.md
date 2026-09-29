---
title: "XarDirectoryEntry"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Mewakili entri direktori dalam arsip xar."
type: docs
weight: 139
url: /id/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

Mewakili entri direktori dalam arsip xar.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mengekstrak semua file di direktori saat ini ke direktori yang diberikan. |
| [getAllEntries()](#getAllEntries--) | Mendapatkan semua entri tipe [XarEntry](../../com.aspose.zip/xarentry) yang membentuk direktori secara rekursif. |
| [getDirectories()](#getDirectories--) | Mendapatkan entri tipe [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) yang membentuk direktori. |
| [getFiles()](#getFiles--) | Mendapatkan entri tipe [XarFileEntry](../../com.aspose.zip/xarfileentry) yang membentuk direktori. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Mendapatkan entri tipe [XarEntry](../../com.aspose.zip/xarentry) yang membentuk direktori. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mengekstrak semua file di direktori saat ini ke direktori yang diberikan.

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
