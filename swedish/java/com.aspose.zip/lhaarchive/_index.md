---
title: "LhaArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en LHA .lzh-arkivfil."
type: docs
weight: 75
url: /sv/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Denna klass representerar en LHA (.lzh)-arkivfil.

Endast följande komprimeringsmetoder stöds:

| ------ | --------------------------------------------- |
| Metod | Förklaring                                   |
| lh0    | Okomprimerad                                  |
| lh4    | 8 KiB glidande ordbok och statisk Huffman   |
| lh5    | 16 KiB glidande ordbok och statisk Huffman  |
| lh6    | 64 KiB glidande ordbok och statisk Huffman  |
| lh7    | 128 KiB glidande ordbok och statisk Huffman |
| lhx    | 1 Mib glidande ordbok och statisk Huffman   |
| lhd    | Katalog                                     |
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Initierar en ny instans av klassen [LhaArchive](../../com.aspose.zip/lhaarchive) och skapar en postlista som kan extraheras från arkivet. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Initierar en ny instans av klassen [LhaArchive](../../com.aspose.zip/lhaarchive) och skapar en postlista som kan extraheras från arkivet. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Initierar en ny instans av klassen [LhaArchive](../../com.aspose.zip/lhaarchive) och skapar en postlista som kan extraheras från arkivet. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Initierar en ny instans av klassen [LhaArchive](../../com.aspose.zip/lhaarchive) och skapar en postlista som kan extraheras från arkivet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar alla filer och kataloger i arkivet till den angivna katalogen. |
| [getEntries()](#getEntries--) | Hämtar filposter av typen [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) som utgör arkivet. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Initierar en ny instans av klassen [LhaArchive](../../com.aspose.zip/lhaarchive) och skapar en postlista som kan extraheras från arkivet.

Denna konstruktor dekomprimerar inte någon post. Se metoden [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | källan till arkivet |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Initierar en ny instans av klassen [LhaArchive](../../com.aspose.zip/lhaarchive) och skapar en postlista som kan extraheras från arkivet.

Denna konstruktor dekomprimerar inte någon post. Se metoden [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | källan till arkivet |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Initierar en ny instans av klassen [LhaArchive](../../com.aspose.zip/lhaarchive) och skapar en postlista som kan extraheras från arkivet.

Följande exempel extraherar ett arkiv och dekomprimerar sedan den första posten till en `MemoryStream`.

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

Den här konstruktorn dekomprimerar inte någon post. Se [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) metod för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | den fullständiga eller relativa sökvägen till arkivfilen |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraherar alla filer och kataloger i arkivet till den angivna katalogen.

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
