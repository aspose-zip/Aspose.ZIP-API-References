---
title: "ArchiveEntry"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier unique dans l'archive."
type: docs
weight: 27
url: /fr/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Représente un fichier unique dans l'archive.

Convertissez une instance [ArchiveEntry](../../com.aspose.zip/archiveentry) en [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) pour déterminer si l'entrée est chiffrée ou non.
## Méthodes

| Méthode | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'entrée vers le flux fourni. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrait l'entrée vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni. |
| [getComment()](#getComment--) | Obtient le commentaire de l'entrée dans l'archive. |
| [getCompressedSize()](#getCompressedSize--) | Obtient la taille du fichier compressé. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtient un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
| [getCompressionSettings()](#getCompressionSettings--) | Obtient les paramètres de compression ou de décompression. |
| [getDataSource()](#getDataSource--) | Source de l'entrée si l'entrée a été ajoutée à l'archive, pas extraite. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Obtient un événement qui est levé lorsqu'une partie du flux brut est extraite. |
| [getLength()](#getLength--) | Obtient la longueur. |
| [getModificationTime()](#getModificationTime--) | Obtient la date et l'heure de dernière modification. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille du fichier original. |
| [isDirectory()](#isDirectory--) | Obtient une valeur indiquant si l'entrée représente un répertoire. |
| [open()](#open--) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu décompressé de l'entrée. |
| [open(String password)](#open-java.lang.String-) | Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu décompressé de l'entrée. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Définit un événement qui est déclenché lorsqu'une partie du flux brut est compressée. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Définit un événement qui est levé lorsqu'une partie du flux brut est extraite. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Définit la date et l'heure de dernière modification. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrait l'entrée vers le flux fourni.

Extrait une entrée d'une archive zip avec un mot de passe.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
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

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
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

Extrait deux entrées d'une archive ZIP, chacune avec son propre mot de passe.

```

``````

try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract("first.bin", "first_pass");
archive.getEntries().get(1).extract("second.bin", "second_pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
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
### getComment() {#getComment--}
```
public final String getComment()
```


Obtient le commentaire de l'entrée dans l'archive.

**Returns:**
java.lang.String - commentaire de l'entrée dans l'archive
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtient la taille du fichier compressé.

**Returns:**
long - taille du fichier compressé
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Obtient un événement qui est déclenché lorsqu'une partie du flux brut est compressée.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Dans cet exemple, le gestionnaire d'événement est utilisé pour l'annulation après les premiers cent Mo de l'entrée ont été extraits.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
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

Lisez le flux pour obtenir le contenu original du fichier.

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
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

L'expéditeur d'événement est une instance de [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un événement qui est déclenché lorsqu'une partie du flux brut est compressée |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Définit un événement qui est levé lorsqu'une partie du flux brut est extraite.

Dans cet exemple, le gestionnaire d'événement est utilisé pour calculer la part de la taille traitée en pourcentage.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

L'expéditeur d'événement est une instance de [ArchiveEntry](../../com.aspose.zip/archiveentry). Il est possible d'annuler l'extraction.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | un événement qui est déclenché lorsqu'une partie du flux brut est extraite. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Définit la date et l'heure de dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | date et heure de dernière modification |

