---
title: "XzArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een xz-archiefbestand."
type: docs
weight: 146
url: /nl/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een xz-archiefbestand. Gebruik het om xz-archieven samen te stellen en te extraheren.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XzArchive()](#XzArchive--) | Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) en stelt het archief samen in xz-formaat. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) en stelt het archief samen in xz-formaat. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extraheert xz-archief naar een bestand. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert xz-archief naar een stroom. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert xz-archief naar een bestand via pad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert de inhoud van het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het xz-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getLength()](#getLength--) | Haalt de lengte van het item op in bytes. |
| [getName()](#getName--) | Haalt de naam van het item binnen het archief op. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de ongecomprimeerde grootte van de bestandsgegevens op in bytes. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat het xz-archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het xz-archief op in het opgegeven bestemmingsbestand. |
| [setSource(File file)](#setSource-java.io.File-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) en stelt het archief samen in xz-formaat.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) en stelt het archief samen in xz-formaat.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | instelling van specifieke xz-archief: woordenboekgrootte, blokgrootte, controletype |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie.

Deze constructor decompresseert niet. Zie de methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie.

Deze constructor decompresseert niet. Zie de methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Opties om het archief mee te laden. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie.

Deze constructor decompresseert niet. Zie de methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | pad naar de bron van het archief |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Initialiseert een nieuw exemplaar van de klasse [XzArchive](../../com.aspose.zip/xzarchive) dat is voorbereid op decompressie.

Deze constructor decompresseert niet. Zie de methode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | pad naar de bron van het archief |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraheert xz-archief naar een bestand.

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | stream voor het opslaan van gedecomprimeerde gegevens |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert xz-archief naar een bestand via pad.

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

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

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
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


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


Slaat het xz-archief op in het opgegeven bestemmingsbestand.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.xz\");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| file | java.io.File | bestand, dat als invoerstream wordt geopend |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourcePath | java.lang.String | pad naar het bestand dat als invoerstream wordt geopend |

