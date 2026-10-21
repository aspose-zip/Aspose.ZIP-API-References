---
title: "IArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Detta gränssnitt representerar ett arkiv."
type: docs
weight: 161
url: /sv/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Detta gränssnitt representerar ett arkiv.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar alla filer i arkivet till den angivna katalogen. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Extraherar alla filer i arkivet till den angivna katalogen.

Om katalogen inte finns kommer den att skapas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Sökvägen till katalogen där de extraherade filerna ska placeras. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet.

Arkiv för endast komprimering, såsom gzip, bzip2, lzip, lzma, lz4, xz, z, består av en enda post – själva arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Hämtar arkivformatet.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
