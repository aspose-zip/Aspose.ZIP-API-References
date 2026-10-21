---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar katalogpost i xar-arkivet."
type: docs
weight: 139
url: /sv/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

Representerar katalogpost i xar-arkivet.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar alla filer i den aktuella katalogen till den angivna katalogen. |
| [getAllEntries()](#getAllEntries--) | Hämtar alla poster av typen [XarEntry](../../com.aspose.zip/xarentry) som utgör katalogen rekursivt. |
| [getDirectories()](#getDirectories--) | Hämtar poster av typen [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) som utgör katalogen. |
| [getFiles()](#getFiles--) | Hämtar poster av typen [XarFileEntry](../../com.aspose.zip/xarfileentry) som utgör katalogen. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Hämtar poster av typen [XarEntry](../../com.aspose.zip/xarentry) som utgör katalogen. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraherar alla filer i den aktuella katalogen till den angivna katalogen.

```

``````

try (XarArchive archive = new XarArchive(\"archive.xar\")) {
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
