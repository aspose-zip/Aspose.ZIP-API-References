---
title: "IArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Dieses Interface stellt ein Archiv dar."
type: docs
weight: 161
url: /de/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Dieses Interface stellt ein Archiv dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis. |
| [getFileEntries()](#getFileEntries--) | Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Extrahiert alle Dateien im Archiv in das angegebene Verzeichnis.

Wenn das Verzeichnis nicht existiert, wird es erstellt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Der Pfad zum Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Ruft Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) ab, die das Archiv bilden.

Archive ausschließlich zur Kompression, wie gzip, bzip2, lzip, lzma, lz4, xz, z, bestehen aus einem einzigen Datensatz – dem Archiv selbst.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das Archiv bilden.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Liefert das Archivformat.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
