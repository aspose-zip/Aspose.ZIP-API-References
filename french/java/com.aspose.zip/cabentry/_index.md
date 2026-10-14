---
title: "CabEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier unique dans une archive cab."
type: docs
weight: 46
url: /fr/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Représente un fichier unique dans une archive cab.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getModificationTime()](#getModificationTime--) | Obtient la date et l'heure de dernière modification. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [open()](#open--) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée. |
| [toString()](#toString--) | Renvoie la représentation sous forme de chaîne de caractères de l'instance de la classe [CabEntry](../../com.aspose.zip/cabentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

Extrait une entrée d'une archive CAB.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.getEntries().get(0).extract(httpResponseStream);
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

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

**Returns:**
java.io.File - les informations du fichier d'un fichier composé
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtient la longueur de l'entrée en octets.

**Returns:**
java.lang.Long - la longueur de l'entrée en octets
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtient la date et l'heure de dernière modification.

**Returns:**
java.util.Date - date et heure de la dernière modification.
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée dans l'archive.

**Returns:**
java.lang.String - le nom de l'entrée dans l'archive
### open() {#open--}
```
public final InputStream open()
```


Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée.

Utilisation :

```

``````

CabArchive archive = new CabArchive(\"archive.cab\");
CabEntry entry = archive.getEntries().get(0);
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
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
