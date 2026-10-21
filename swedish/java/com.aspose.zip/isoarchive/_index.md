---
title: "IsoArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Representerar ett ISO-arkiv ISO 9660."
type: docs
weight: 71
url: /sv/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Representerar ett ISO-arkiv (ISO 9660).
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och skapar ett tomt ISO-arkiv för att lägga till nya filer och kataloger. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och sammansätter en postlista som kan extraheras från arkivet. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och sammansätter en postlista som kan extraheras från arkivet. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och sammansätter en postlista som kan extraheras från arkivet. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och sammansätter en postlista som kan extraheras från arkivet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Lägger till en katalog i ISO-avbilden. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Lägger till en fil i ISO-avbilden. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Lägger till en fil i ISO-avbilden. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Lägger till en fil i ISO-avbilden. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar alla poster till den angivna katalogen. |
| [getEntries()](#getEntries--) | Hämtar poster av typen [IsoEntry](../../com.aspose.zip/isoentry) som utgör arkivet. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Sparar ISO-avbilden till den angivna strömmen. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Sparar ISO-avbilden till den angivna strömmen. |
| [save(String path)](#save-java.lang.String-) | Sparar ISO-avbilden till den angivna sökvägen. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Sparar ISO-avbilden till den angivna sökvägen. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och skapar ett tomt ISO-arkiv för att lägga till nya filer och kataloger.

Följande exempel visar hur man skapar ett nytt tomt ISO-arkiv och lägger till filer i det:

```

``````

// Skapa ett nytt tomt ISO-arkiv
try (IsoArchive isoArchive = new IsoArchive()) {
// Lägg till filer i ISO-arkivet
isoArchive.createEntry(\"example_file.txt\", \"path_to_file.txt\");
// Spara ISO-arkivet till en fil
isoArchive.save(\"new_archive.iso\");
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

Denna konstruktor packar inte upp någon post.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | källan till arkivet |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och sammansätter en postlista som kan extraheras från arkivet.

Följande exempel visar hur man extraherar alla poster till en katalog.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream(\"archive.iso\"))) {
archive.extractToDirectory(\"C:\\\\extracted\");
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

Denna konstruktor packar inte upp någon post.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till arkivfilen |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Initierar en ny instans av klassen [IsoArchive](../../com.aspose.zip/isoarchive) och sammansätter en postlista som kan extraheras från arkivet.

Följande exempel visar hur man extraherar alla poster till en katalog.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory(\"C:\\\\extracted\");
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | java.lang.String | katalogen att extrahera posterna till |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Hämtar poster av typen [IsoEntry](../../com.aspose.zip/isoentry) som utgör arkivet.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - poster av typen [IsoEntry](../../com.aspose.zip/isoentry) som utgör iso-arkivet
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör iso-arkivet
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Hämtar arkivformatet.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Sparar ISO-avbilden till den angivna strömmen.

Följande exempel visar hur man sparar ett ISO-arkiv till en minnesström:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Skapa ett nytt tomt ISO-arkiv
try (IsoArchive isoArchive = new IsoArchive()) {
// Lägg till filer i ISO-arkivet
isoArchive.createEntry(\"example_file.txt\", \"path_to_file.txt\");
// Spara ISO-arkivet till en minnesström
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | java.io.OutputStream | strömmen där ISO-avbilden kommer att sparas |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | alternativen för att spara ISO-arkivet med |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Sparar ISO-avbilden till den angivna sökvägen.

Följande exempel visar hur man sparar ett ISO-arkiv till en fil:

```

``````

// Skapa ett nytt tomt ISO-arkiv
try (IsoArchive isoArchive = new IsoArchive()) {
// Lägg till filer i ISO-arkivet
isoArchive.createEntry(\"example_file.txt\", \"path_to_file.txt\");
// Spara ISO-arkivet till en fil
isoArchive.save(\"new_archive.iso\");
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen där ISO-avbilden kommer att sparas |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | alternativen för att spara ISO-arkivet med |

