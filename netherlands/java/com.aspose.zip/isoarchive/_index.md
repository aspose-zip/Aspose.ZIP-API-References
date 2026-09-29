---
title: "IsoArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Stelt een ISO‑archief ISO 9660 voor."
type: docs
weight: 71
url: /nl/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Vertegenwoordigt een ISO-archief (ISO 9660).
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en maakt een leeg ISO‑archief aan om nieuwe bestanden en mappen toe te voegen. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Voegt een map toe aan het ISO‑beeld. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Voegt een bestand toe aan het ISO‑beeld. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Voegt een bestand toe aan het ISO‑beeld. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Voegt een bestand toe aan het ISO‑beeld. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle items naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt items op van het type [IsoEntry](../../com.aspose.zip/isoentry) die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Slaat het ISO‑beeld op naar de opgegeven stream. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Slaat het ISO‑beeld op naar de opgegeven stream. |
| [save(String path)](#save-java.lang.String-) | Slaat het ISO‑beeld op naar het opgegeven pad. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Slaat het ISO‑beeld op naar het opgegeven pad. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en maakt een leeg ISO‑archief aan om nieuwe bestanden en mappen toe te voegen.

Het volgende voorbeeld toont hoe een nieuw leeg ISO‑archief te maken en er bestanden aan toe te voegen:

```

``````

// Maak een nieuw leeg ISO‑archief
try (IsoArchive isoArchive = new IsoArchive()) {
// Voeg bestanden toe aan het ISO‑archief
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Sla het ISO‑archief op naar een bestand
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Deze constructor pakt geen enkel item uit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Deze constructor pakt geen enkel item uit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [IsoArchive](../../com.aspose.zip/isoarchive)‑klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | java.lang.String | de map waarin de items moeten worden uitgepakt |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Haalt items op van het type [IsoEntry](../../com.aspose.zip/isoentry) die het archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - items van het type [IsoEntry](../../com.aspose.zip/isoentry) die het iso-archief vormen
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het iso-archief vormen
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Slaat het ISO‑beeld op naar de opgegeven stream.

Het volgende voorbeeld laat zien hoe een ISO-archief naar een geheugenstroom kan worden opgeslagen:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Maak een nieuw leeg ISO‑archief
try (IsoArchive isoArchive = new IsoArchive()) {
// Voeg bestanden toe aan het ISO‑archief
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Sla het ISO-archief op in een geheugenstroom
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | java.io.OutputStream | de stroom waarin het ISO-image wordt opgeslagen |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | de opties om het ISO-archief mee op te slaan |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Slaat het ISO‑beeld op naar het opgegeven pad.

Het volgende voorbeeld laat zien hoe een ISO-archief naar een bestand kan worden opgeslagen:

```

``````

// Maak een nieuw leeg ISO‑archief
try (IsoArchive isoArchive = new IsoArchive()) {
// Voeg bestanden toe aan het ISO‑archief
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Sla het ISO‑archief op naar een bestand
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad waar het ISO-image wordt opgeslagen |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | de opties om het ISO-archief mee op te slaan |

