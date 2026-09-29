---
title: "SnappyArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een snappy-archiefbestand."
type: docs
weight: 121
url: /nl/java/com.aspose.zip/snappyarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class SnappyArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Deze klasse vertegenwoordigt een snappy-archiefbestand. Gebruik deze om snappy-archieven samen te stellen of te extraheren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SnappyArchive()](#SnappyArchive--) | Initialiseert een nieuw exemplaar van de [SnappyArchive](../../com.aspose.zip/snappyarchive) klasse, voorbereid voor compressie. |
| [SnappyArchive(InputStream source)](#SnappyArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [SnappyArchive](../../com.aspose.zip/snappyarchive) klasse, voorbereid voor decompressie. |
| [SnappyArchive(String path)](#SnappyArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [SnappyArchive](../../com.aspose.zip/snappyarchive) klasse, voorbereid voor decompressie. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extraheert een snappy-archief naar een bestand. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert een snappy-archief naar een stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert een snappy-archief naar een bestand via pad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert de inhoud van het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het snappy-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getName()](#getName--) | De naam van het oorspronkelijke bestand. |
| [save(File destination)](#save-java.io.File-) | Slaat het snappy-archief op in het opgegeven bestemmingsbestand. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat het snappy-archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het snappy-archief op in het opgegeven bestemmingsbestand. |
| [setSource(File file)](#setSource-java.io.File-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
### SnappyArchive() {#SnappyArchive--}
```
public SnappyArchive()
```


Initialiseert een nieuw exemplaar van de [SnappyArchive](../../com.aspose.zip/snappyarchive) klasse, voorbereid voor compressie.

Het volgende voorbeeld laat zien hoe een bestand te comprimeren.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



### SnappyArchive(InputStream source) {#SnappyArchive-java.io.InputStream-}
```
public SnappyArchive(InputStream source)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The source of the archive. |

### SnappyArchive(String path) {#SnappyArchive-java.lang.String-}
```
public SnappyArchive(String path)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

```

``````

      try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
          try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
              try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                  archive.extract(extractedFile);
              }
          }
      } catch (IOException ex) {
      }
 
```

Deze constructor decompresseert niet. Zie [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar de bron van het archief |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraheert een snappy-archief naar een bestand.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
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


Extracts snappy archive to a stream.

```

``````

     try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
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


Extraheert een snappy-archief naar een bestand via pad.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
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
java.io.File - java.io.File instance containing extracted data
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


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive
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
java.lang.Long - length.
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.snappy"));
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.File | het bestand dat als bestemmingsstream wordt geopend |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Slaat het snappy-archief op in de opgegeven stream.

```

``````

try (FileOutputStream snappyFile = new FileOutputStream("archive.snappy")) {
try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save(snappyFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.snappy");
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

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as an input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.snappy");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de invoerstream voor het archief |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | the path to the file which will be opened as an input stream |

