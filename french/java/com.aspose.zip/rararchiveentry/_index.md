---
title: "RarArchiveEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier unique dans l'archive."
type: docs
weight: 98
url: /fr/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Représente un fichier unique dans l'archive.

Convertissez une instance de [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) en [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) pour déterminer si l'entrée est chiffrée ou non.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getCompressedSize()](#getCompressedSize--) | Obtient la taille du fichier compressé. |
| [getCreationTime()](#getCreationTime--) | Obtient la date et l'heure de création. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Obtient un événement qui est levé lorsqu'une partie du flux brut est extraite. |
| [getLastAccessTime()](#getLastAccessTime--) | Obtient la date et l'heure du dernier accès. |
| [getLength()](#getLength--) | Obtient la longueur. |
| [getModificationTime()](#getModificationTime--) | Obtient la date et l'heure de dernière modification. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille du fichier original. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si l'entrée représente un répertoire. |
| [open()](#open--) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu décompressé de l'entrée. |
| [open(String password)](#open-java.lang.String-) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu décompressé de l'entrée. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Définit un événement qui est levé lorsqu'une partie du flux brut est extraite. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.


Extrait une entrée d'une archive rar avec mot de passe.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(outputStream, "p@s$");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Flux de destination. Doit être accessible en écriture. |
| password | java.lang.String | Mot de passe optionnel pour le déchiffrement. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni.


Extrait deux entrées d'une archive rar.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |
| password | java.lang.String | Mot de passe optionnel pour le déchiffrement. |

**Returns:**
java.io.File - les informations du fichier extrait
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtient la taille du fichier compressé.

**Returns:**
long - la taille du fichier compressé
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Obtient la date et l'heure de création.

**Returns:**
java.util.Date - date et heure de création.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Obtient un événement qui est levé lorsqu'une partie du flux brut est extraite.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

Lisez le flux pour obtenir le contenu original du fichier. Voir la section des exemples.

**Returns:**
java.io.InputStream - Le flux qui représente le contenu de l'entrée.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu décompressé de l'entrée.


Utilisation :

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

L'expéditeur d'événement est une instance de [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un événement qui est déclenché lorsqu'une partie du flux brut est extraite. |

