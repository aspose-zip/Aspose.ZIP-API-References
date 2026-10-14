---
title: "LhaArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een LHA .lzh archiefbestand."
type: docs
weight: 75
url: /nl/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een LHA (.lzh) archiefbestand.

Alleen de volgende compressiemethoden worden ondersteund:

| ------ | --------------------------------------------- |
| Methode | Uitleg                                   |
| lh0    | Niet gecomprimeerd                                  |
| lh4    | 8 KiB glijdend woordenboek en statische Huffman   |
| lh5    | 16 KiB glijdend woordenboek en statische Huffman  |
| lh6    | 64 KiB glijdend woordenboek en statische Huffman  |
| lh7    | 128 KiB glijdend woordenboek en statische Huffman |
| lhx    | 1 Mib glijdend woordenboek en statische Huffman   |
| lhd    | Map                                     |
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de klasse [LhaArchive](../../com.aspose.zip/lhaarchive) en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [LhaArchive](../../com.aspose.zip/lhaarchive) en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [LhaArchive](../../com.aspose.zip/lhaarchive) en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [LhaArchive](../../com.aspose.zip/lhaarchive) en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden en mappen in het archief naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt bestandsitems op van het type [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Initialiseert een nieuw exemplaar van de klasse [LhaArchive](../../com.aspose.zip/lhaarchive) en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Deze constructor decompresseert geen enkel item. Zie de methode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de klasse [LhaArchive](../../com.aspose.zip/lhaarchive) en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Deze constructor decompresseert geen enkel item. Zie de methode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opties om een bestaand archief mee te laden. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Initialiseert een nieuw exemplaar van de klasse [LhaArchive](../../com.aspose.zip/lhaarchive) en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Het volgende voorbeeld extraheert een archief en decompresseert vervolgens het eerste item naar een `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Deze constructor decompresseert geen enkele entry. Zie de [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het volledig gekwalificeerde of het relatieve pad naar het archiefbestand |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opties om een bestaand archief mee te laden. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert alle bestanden en mappen in het archief naar de opgegeven map.

```

``````

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
