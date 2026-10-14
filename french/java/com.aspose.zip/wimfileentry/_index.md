---
title: "WimFileEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un seul fichier dans une archive wim."
type: docs
weight: 133
url: /fr/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

Représente un seul fichier dans une archive wim.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [open()](#open--) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

Extrait une entrée d'une archive wim.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

**Returns:**
java.io.File - les informations du fichier extrait
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtient la longueur de l'entrée en octets.

**Returns:**
java.lang.Long - la longueur de l'entrée en octets
### open() {#open--}
```
public final InputStream open()
```


Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée.

Utilisation :

```

``````

try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
