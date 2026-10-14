---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Vertegenwoordigt mapvermelding binnen xar-archief."
type: docs
weight: 139
url: /nl/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

Vertegenwoordigt mapvermelding binnen xar-archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden in de huidige map naar de opgegeven map. |
| [getAllEntries()](#getAllEntries--) | Haalt alle items op van het type [XarEntry](../../com.aspose.zip/xarentry) die de map recursief vormen. |
| [getDirectories()](#getDirectories--) | Haalt items op van het type [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) die de map vormen. |
| [getFiles()](#getFiles--) | Haalt items op van het type [XarFileEntry](../../com.aspose.zip/xarfileentry) die de map vormen. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Haalt items op van het type [XarEntry](../../com.aspose.zip/xarentry) die de map vormen. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert alle bestanden in de huidige map naar de opgegeven map.

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
