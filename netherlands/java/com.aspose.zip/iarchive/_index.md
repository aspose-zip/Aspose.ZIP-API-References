---
title: "IArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze interface vertegenwoordigt een archief."
type: docs
weight: 161
url: /nl/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Deze interface vertegenwoordigt een archief.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden in het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Extraheert alle bestanden in het archief naar de opgegeven map.

Als de map niet bestaat, wordt deze aangemaakt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Het pad naar de map waarin de uitgepakte bestanden worden geplaatst. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen.

Archieven alleen voor compressie, zoals gzip, bzip2, lzip, lzma, lz4, xz, z bestaan uit één enkel record - het archief zelf.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
