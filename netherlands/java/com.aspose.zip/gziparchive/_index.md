---
title: "GzipArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een gzip-archiefbestand."
type: docs
weight: 69
url: /nl/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Deze klasse vertegenwoordigt een gzip-archiefbestand. Gebruik deze om gzip-archieven samen te stellen of te extraheren.

Het gzip-compressiealgoritme is gebaseerd op het DEFLATE-algoritme, dat een combinatie is van LZ77 en Huffman-codering.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor compressie. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor decompressie. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor decompressie. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor decompressie. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor decompressie. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse. |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het archief naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het archief naar het bestand op het opgegeven pad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert de inhoud van het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het gzip-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getLength()](#getLength--) | Haalt de grootte op van een origineel bestand. |
| [getName()](#getName--) | De naam van het originele bestand. |
| [getUncompressedSize()](#getUncompressedSize--) | Haalt de grootte op van een origineel bestand. |
| [open()](#open--) | Opent het archief voor extractie en levert een stream met de archiefinhoud. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(File file)](#setSource-java.io.File-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(String path)](#setSource-java.lang.String-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor compressie.

Het volgende voorbeeld laat zien hoe een bestand te comprimeren.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Deze constructor decompresseert niet. Zie de [open()](../../com.aspose.zip/gziparchive\#open--) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | De bron van het archief. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor decompressie.

Open een archief vanuit een stream en extraheer het naar een `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

Deze constructor decompresseert niet. Zie de [open()](../../com.aspose.zip/gziparchive\#open--) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | De bron van het archief. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Opties om het archief mee te laden. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse, voorbereid voor decompressie.

Open een archief vanuit een bestand via pad en extraheer het naar een `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Deze constructor decompresseert niet. Zie de [open()](../../com.aspose.zip/gziparchive\#open--) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Het pad naar het archiefbestand. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Initialiseert een nieuw exemplaar van de [GzipArchive](../../com.aspose.zip/gziparchive) klasse.

Open een archief vanuit een bestand via pad en extraheer het naar een `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | Doelstream. Moet beschrijfbaar zijn. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert het archief naar het bestand op het opgegeven pad.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Het pad naar het doelbestand. Als het bestand al bestaat, wordt het overschreven. |

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
|  | destinationDirectory | java.lang.String | Het pad naar de map waarin de uitgepakte bestanden worden geplaatst. |

Als de map niet bestaat, wordt deze aangemaakt. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het gzip-archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type die het gzip-archief vormen.
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


Haalt de grootte op van een origineel bestand.

Tijdens decompressie kan deze eigenschap een onjuiste grootte bevatten. Als de grootte van het uitgepakte bestand 4 GB overschrijdt, zal deze eigenschap een verkeerde waarde geven vanwege de 32‑bit limiet in de header.

**Returns:**
java.lang.Long - grootte van een origineel bestand
### getName() {#getName--}
```
public final String getName()
```


De naam van het originele bestand.

**Returns:**
java.lang.String - de naam van het oorspronkelijke bestand
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Haalt de grootte op van een origineel bestand.

Tijdens decompressie kan deze eigenschap een onjuiste grootte bevatten. Als de grootte van het uitgepakte bestand 4 GB overschrijdt, zal deze eigenschap een verkeerde waarde geven vanwege de 32‑bit limiet in de header.

**Returns:**
long - grootte van een origineel bestand.
### open() {#open--}
```
public final InputStream open()
```


Opent het archief voor extractie en levert een stream met de archiefinhoud.

Extraheert het archief en kopieert de geëxtraheerde inhoud naar een bestandsstream.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Doelstream. |

`outputStream` moet schrijfbaar zijn. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Gebruik deze methode om een gezamenlijk tar.gz‑archief samen te stellen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar-archief dat moet worden gecomprimeerd. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | De invoerstroom voor het archief. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

Open een archief vanuit een bestand via pad en extraheer het naar een `MemoryStream`

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource("data.bin");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

