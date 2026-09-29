---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt einen Verzeichniseintrag innerhalb eines XAR-Archivs dar."
type: docs
weight: 139
url: /de/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

Stellt einen Verzeichniseintrag innerhalb eines XAR-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im aktuellen Verzeichnis in das angegebene Verzeichnis. |
| [getAllEntries()](#getAllEntries--) | Ermittelt alle Einträge des Typs [XarEntry](../../com.aspose.zip/xarentry), die das Verzeichnis rekursiv bilden. |
| [getDirectories()](#getDirectories--) | Liefert Einträge des Typs [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry), die das Verzeichnis bilden. |
| [getFiles()](#getFiles--) | Liefert Einträge des Typs [XarFileEntry](../../com.aspose.zip/xarfileentry), die das Verzeichnis bilden. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Liefert Einträge des Typs [XarEntry](../../com.aspose.zip/xarentry), die das Verzeichnis bilden. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien im aktuellen Verzeichnis in das angegebene Verzeichnis.

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
