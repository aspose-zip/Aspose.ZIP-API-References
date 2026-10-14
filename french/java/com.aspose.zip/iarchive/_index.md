---
title: "IArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette interface représente une archive."
type: docs
weight: 161
url: /fr/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Cette interface représente une archive.
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Extrait tous les fichiers de l'archive vers le répertoire fourni.

Si le répertoire n'existe pas, il sera créé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Le chemin du répertoire où placer les fichiers extraits. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive.

Les archives uniquement destinées à la compression, telles que gzip, bzip2, lzip, lzma, lz4, xz, z, se composent d'un seul enregistrement - l'archive elle‑même.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Obtient le format de l'archive.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
