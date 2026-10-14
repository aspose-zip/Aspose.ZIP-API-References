---
title: "WimDirectoryEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un seul répertoire dans une archive wim."
type: docs
weight: 131
url: /fr/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

Représente un seul répertoire dans une archive wim.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers du répertoire actuel vers le répertoire fourni. |
| [getAllEntries()](#getAllEntries--) | Obtient toutes les entrées de type [WimEntry](../../com.aspose.zip/wimentry) constituant le répertoire de manière récursive. |
| [getDirectories()](#getDirectories--) | Obtient les entrées de type [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) constituant le répertoire. |
| [getFiles()](#getFiles--) | Obtient les entrées de type [WimFileEntry](../../com.aspose.zip/wimfileentry) constituant le répertoire. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Obtient les entrées de type [WimEntry](../../com.aspose.zip/wimentry) constituant le répertoire. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait tous les fichiers du répertoire actuel vers le répertoire fourni.

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
