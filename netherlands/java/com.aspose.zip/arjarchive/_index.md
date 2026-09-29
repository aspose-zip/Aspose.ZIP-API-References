---
title: "ArjArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een ARJ-archiefbestand."
type: docs
weight: 37
url: /nl/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een ARJ-archiefbestand.

Alleen de volgende compressiemethoden worden ondersteund:

| ------ | ------------------------------------------------------------ |
| Methode | Uitleg                                                  |
| 0      | Niet gecomprimeerd                                                 |
| 1      | Combinatie van LZ77 en adaptieve Huffman-codering. Beste verhouding. |
| 2      | Combinatie van LZ77 en adaptieve Huffman-codering.             |
| 3      | Combinatie van LZ77 en adaptieve Huffman-codering. Beste snelheid. |
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [ArjArchive](../../com.aspose.zip/arjarchive) klasse en maakt een lijst met items die uit het archief kunnen worden geëxtraheerd. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Initialiseert een nieuw exemplaar van de [ArjArchive](../../com.aspose.zip/arjarchive) klasse en maakt een lijst met items die uit het archief kunnen worden geëxtraheerd. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [ArjArchive](../../com.aspose.zip/arjarchive) klasse en maakt een lijst met items die uit het archief kunnen worden geëxtraheerd. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Initialiseert een nieuw exemplaar van de [ArjArchive](../../com.aspose.zip/arjarchive) klasse en maakt een lijst met items die uit het archief kunnen worden geëxtraheerd. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle items naar de opgegeven map. |
| [getCommentary()](#getCommentary--) | Haalt de commentaar op. |
| [getEntries()](#getEntries--) | Haalt items op van het type [ArjEntryPlain](../../com.aspose.zip/arjentryplain) die het ARJ-archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getName()](#getName--) | Haalt de oorspronkelijke naam op. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Initialiseert een nieuw exemplaar van de [ArjArchive](../../com.aspose.zip/arjarchive) klasse en maakt een lijst met items die uit het archief kunnen worden geëxtraheerd.

Deze constructor decompresseert geen enkel item. Zie de [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extractionSource | java.io.InputStream | de bron van het archief |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [ArjArchive](../../com.aspose.zip/arjarchive) klasse en maakt een lijst met items die uit het archief kunnen worden geëxtraheerd.

Deze constructor decompresseert geen enkel item. Zie de [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extractionSource | java.io.InputStream | de bron van het archief |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Opties om een bestaand archief mee te laden. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Initialiseert een nieuw exemplaar van de [ArjArchive](../../com.aspose.zip/arjarchive) klasse en maakt een lijst met items die uit het archief kunnen worden geëxtraheerd.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Deze constructor pakt geen enkel item uit. Zie de [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Opties om een bestaand archief mee te laden. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert alle items naar de opgegeven map.

Het volgende voorbeeld laat zien hoe alle items naar een map te extraheren:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
