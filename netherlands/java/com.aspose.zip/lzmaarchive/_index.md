---
title: "LzmaArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een LZMA-archiefbestand."
type: docs
weight: 86
url: /nl/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Deze klasse vertegenwoordigt een LZMA-archiefbestand. Gebruik deze om LZMA-archieven samen te stellen of te extraheren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse en stelt het archief samen in LZMA-formaat. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse en stelt het archief samen in LZMA-formaat. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse, voorbereid op decompressie. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse, voorbereid op decompressie. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extraheert LZMA-archief naar een bestand. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert LZMA-archief naar een stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert LZMA-archief naar een bestand via pad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert de inhoud van het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het LZMA-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getName()](#getName--) | De naam van het oorspronkelijke bestand. |
| [save(File destination)](#save-java.io.File-) | Slaat het LZMA-archief op naar het opgegeven bestemmingsbestand. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat lzma-archief op naar de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het LZMA-archief op naar het opgegeven bestemmingsbestand. |
| [setSource(File file)](#setSource-java.io.File-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse en stelt het archief samen in LZMA-formaat.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse en stelt het archief samen in LZMA-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | set van instellingen voor een specifiek lzma-archief |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse, voorbereid op decompressie.

Deze constructor decompresseert niet. Zie de methode [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\\#extract-OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Initialiseert een nieuw exemplaar van de [LzmaArchive](../../com.aspose.zip/lzmaarchive) klasse, voorbereid op decompressie.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| file | java.io.File | het bestand voor het opslaan van gedecomprimeerde gegevens |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraheert LZMA-archief naar een stream.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestand dat de gedecomprimeerde gegevens zal opslaan |

**Returns:**
java.io.File - de bestandsinformatie van het geëxtraheerde bestand
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert de inhoud van het archief naar de opgegeven map.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | het pad naar de map waarin de uitgepakte bestanden moeten worden geplaatst. |

Als de map niet bestaat, wordt deze aangemaakt |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het LZMA-archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het lzma-archief vormen.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Haalt de lengte op.

**Returns:**
java.lang.Long - lengte
### getName() {#getName--}
```
public final String getName()
```


De naam van het oorspronkelijke bestand.

**Returns:**
java.lang.String - de naam van het oorspronkelijke bestand
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Slaat het LZMA-archief op naar het opgegeven bestemmingsbestand.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lzma\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | java.io.OutputStream | bestemmingsstroom |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Slaat het LZMA-archief op naar het opgegeven bestemmingsbestand.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| file | java.io.File | het bestand dat als invoerstroom wordt geopend |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save(\"archive.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourcePath | java.lang.String | pad naar bestand, dat wordt geopend als invoerstroom |

