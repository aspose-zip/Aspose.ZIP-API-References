---
title: "WimImage"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt ein einzelnes Image innerhalb eines Wim-Archivs dar."
type: docs
weight: 134
url: /de/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

Stellt ein einzelnes Image innerhalb eines Wim-Archivs dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im Image in das angegebene Verzeichnis. |
| [getAllEntries()](#getAllEntries--) | Liefert Einträge des Typs [WimEntry](../../com.aspose.zip/wimentry) zurück, die das Image rekursiv bilden. |
| [getEntry(String path)](#getEntry-java.lang.String-) | Liefert den Eintrag des Typs [WimEntry](../../com.aspose.zip/wimentry) für einen angegebenen Pfad. |
| [getParent()](#getParent--) | Liefert das Archiv, zu dem das Image gehört. |
| [getRootDirectory()](#getRootDirectory--) | Liefert den Wurzelverzeichnis-Eintrag des Images. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien im Image in das angegebene Verzeichnis.

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
