---
title: "WimImage"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta una singola immagine all'interno di un archivio wim."
type: docs
weight: 134
url: /it/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

Rappresenta una singola immagine all'interno di un archivio wim.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file nell'immagine nella directory fornita. |
| [getAllEntries()](#getAllEntries--) | Ottiene le voci di tipo [WimEntry](../../com.aspose.zip/wimentry) che costituiscono l'immagine in modo ricorsivo. |
| [getEntry(String path)](#getEntry-java.lang.String-) | Ottiene la voce di tipo [WimEntry](../../com.aspose.zip/wimentry) per un percorso specificato. |
| [getParent()](#getParent--) | Ottiene l'archivio a cui appartiene l'immagine. |
| [getRootDirectory()](#getRootDirectory--) | Ottiene la voce della directory radice dell'immagine. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae tutti i file nell'immagine nella directory fornita.

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
