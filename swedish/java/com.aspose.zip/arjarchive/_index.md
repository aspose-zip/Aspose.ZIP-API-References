---
title: "ArjArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en ARJ-arkivfil."
type: docs
weight: 37
url: /sv/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Denna klass representerar en ARJ-arkivfil.

Endast följande komprimeringsmetoder stöds:

| ------ | ------------------------------------------------------------ |
| Metod | Förklaring                                                  |
| 0      | Okomprimerad                                                 |
| 1      | Kombination av LZ77 och adaptiv Huffman‑kodning. Bästa förhållandet. |
| 2      | Kombination av LZ77 och adaptiv Huffman‑kodning.             |
| 3      | Kombination av LZ77 och adaptiv Huffman‑kodning. Bästa hastigheten. |
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Initierar en ny instans av klassen [ArjArchive](../../com.aspose.zip/arjarchive) och skapar en postlista som kan extraheras från arkivet. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Initierar en ny instans av klassen [ArjArchive](../../com.aspose.zip/arjarchive) och skapar en postlista som kan extraheras från arkivet. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Initierar en ny instans av klassen [ArjArchive](../../com.aspose.zip/arjarchive) och skapar en postlista som kan extraheras från arkivet. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Initierar en ny instans av klassen [ArjArchive](../../com.aspose.zip/arjarchive) och skapar en postlista som kan extraheras från arkivet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar alla poster till den angivna katalogen. |
| [getCommentary()](#getCommentary--) | Hämtar kommentaren. |
| [getEntries()](#getEntries--) | Hämtar poster av typen [ArjEntryPlain](../../com.aspose.zip/arjentryplain) som utgör ARJ‑arkivet. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getName()](#getName--) | Hämtar det ursprungliga namnet. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Initierar en ny instans av klassen [ArjArchive](../../com.aspose.zip/arjarchive) och skapar en postlista som kan extraheras från arkivet.

Den här konstruktorn dekomprimerar inte någon post. Se metoden [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| extractionSource | java.io.InputStream | källan till arkivet |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Initierar en ny instans av klassen [ArjArchive](../../com.aspose.zip/arjarchive) och skapar en postlista som kan extraheras från arkivet.

Den här konstruktorn dekomprimerar inte någon post. Se metoden [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| extractionSource | java.io.InputStream | källan till arkivet |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Initierar en ny instans av klassen [ArjArchive](../../com.aspose.zip/arjarchive) och skapar en postlista som kan extraheras från arkivet.

Följande exempel visar hur man extraherar alla poster till en katalog.

```

``````

try (ArjArchive archive = new ArjArchive(\"archive.arj\")) {
archive.extractToDirectory(\"C:\\\\extracted\");
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

Den här konstruktorn packar inte upp någon post. Se metoden [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till arkivfilen |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraherar alla poster till den angivna katalogen.

Följande exempel visar hur man extraherar alla poster till en katalog:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream(\"archive.arj\"))) {
archive.extractToDirectory(\"C:\\\\extracted\");
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
