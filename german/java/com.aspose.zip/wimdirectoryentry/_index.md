---
title: "WimDirectoryEntry"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt ein einzelnes Verzeichnis innerhalb eines Wim-Archivs dar."
type: docs
weight: 131
url: /de/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

Stellt ein einzelnes Verzeichnis innerhalb eines Wim-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im aktuellen Verzeichnis in das angegebene Verzeichnis. |
| [getAllEntries()](#getAllEntries--) | Liefert alle Einträge des Typs [WimEntry](../../com.aspose.zip/wimentry), die das Verzeichnis rekursiv bilden. |
| [getDirectories()](#getDirectories--) | Liefert Einträge des Typs [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry), die das Verzeichnis bilden. |
| [getFiles()](#getFiles--) | Liefert Einträge des Typs [WimFileEntry](../../com.aspose.zip/wimfileentry), die das Verzeichnis bilden. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Liefert Einträge des Typs [WimEntry](../../com.aspose.zip/wimentry), die das Verzeichnis bilden. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien im aktuellen Verzeichnis in das angegebene Verzeichnis.

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
