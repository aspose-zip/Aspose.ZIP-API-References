---
title: "LzxArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een LZX .lzx-archiefbestand."
type: docs
weight: 89
url: /nl/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een LZX (.lzx) archiefbestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Initialiseert een nieuwe instantie van de [LzxArchive](../../com.aspose.zip/lzxarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Initialiseert een nieuwe instantie van de [LzxArchive](../../com.aspose.zip/lzxarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Initialiseert een nieuwe instantie van de [LzxArchive](../../com.aspose.zip/lzxarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Initialiseert een nieuwe instantie van de [LzxArchive](../../com.aspose.zip/lzxarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden en mappen in het archief naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt bestandsitems op van het type [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Initialiseert een nieuwe instantie van de [LzxArchive](../../com.aspose.zip/lzxarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Deze constructor decompresseert geen enkel item. Zie de methode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extractionSource | java.io.InputStream | De bron van het archief. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Initialiseert een nieuwe instantie van de [LzxArchive](../../com.aspose.zip/lzxarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Deze constructor decompresseert geen enkel item. Zie de methode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extractionSource | java.io.InputStream | De bron van het archief. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opties om een bestaand archief mee te laden. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Initialiseert een nieuwe instantie van de [LzxArchive](../../com.aspose.zip/lzxarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Het volgende voorbeeld extraheert een archief en decompresseert vervolgens het eerste item naar een `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Deze constructor decompresseert geen enkel item. Zie de methode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Het volledig gekwalificeerde of het relatieve pad naar het archiefbestand. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opties om een bestaand archief mee te laden. |

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

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
