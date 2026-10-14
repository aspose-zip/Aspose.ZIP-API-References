---
title: "WimImage"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente une seule image dans une archive wim."
type: docs
weight: 134
url: /fr/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

Représente une seule image dans une archive wim.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'image vers le répertoire fourni. |
| [getAllEntries()](#getAllEntries--) | Obtient les entrées de type [WimEntry](../../com.aspose.zip/wimentry) constituant l'image de manière récursive. |
| [getEntry(String path)](#getEntry-java.lang.String-) | Obtient l'entrée de type [WimEntry](../../com.aspose.zip/wimentry) pour un chemin donné. |
| [getParent()](#getParent--) | Obtient l'archive à laquelle l'image appartient. |
| [getRootDirectory()](#getRootDirectory--) | Obtient l'entrée du répertoire racine de l'image. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait tous les fichiers de l'image vers le répertoire fourni.

```

``````

try (WimArchive archive = new WimArchive("install.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
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
