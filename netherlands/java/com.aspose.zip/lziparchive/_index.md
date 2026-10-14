---
title: "LzipArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een Lzip-archiefbestand."
type: docs
weight: 83
url: /nl/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Deze klasse vertegenwoordigt een Lzip-archiefbestand. Gebruik het om Lzip-archieven samen te stellen of te extraheren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive). |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive) klasse, voorbereid op decompressie. |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive) klasse, voorbereid op decompressie. |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive) klasse, voorbereid op decompressie. |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive) klasse, voorbereid op decompressie. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extraheert lzip-archief naar een bestand. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert lzip-archief naar een stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert lzip-archief naar een bestand via pad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert de inhoud van het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt de items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het lzip-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getName()](#getName--) | De naam van het oorspronkelijke bestand. |
| [getSettings()](#getSettings--) | Haalt de instelling op van een specifiek lzip-archief. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de ongecomprimeerde grootte van de bestandsgegevens op in bytes. |
| [save(File destination)](#save-java.io.File-) | Slaat het lzip-archief op naar het opgegeven bestemmingsbestand. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Slaat het lzip-archief op naar de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het lzip-archief op naar het opgegeven bestemmingsbestand. |
| [setSource(File file)](#setSource-java.io.File-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(String path)](#setSource-java.lang.String-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive).

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive).

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | de instelling van een specifiek lzip-archief met definitie van de woordenboekgrootte |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive) klasse, voorbereid op decompressie.

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

Deze constructor decompresseert niet. Zie de [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Opties om het archief mee te laden. |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


Initialiseert een nieuw exemplaar van de [LzipArchive](../../com.aspose.zip/lziparchive) klasse, voorbereid op decompressie.

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

Deze constructor decompresseert niet. Zie de [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar de bron van het archief |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | Opties om het archief mee te laden. |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraheert lzip-archief naar een bestand.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | de stream voor het opslaan van gedecomprimeerde gegevens |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert lzip-archief naar een bestand via pad.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.File | het bestand dat als bestemmingsstream wordt geopend |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Slaat het lzip-archief op naar de opgegeven stream.

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de invoerstream voor het archief |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

