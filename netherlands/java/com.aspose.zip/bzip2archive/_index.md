---
title: "Bzip2Archive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een bzip2-archiefbestand."
type: docs
weight: 40
url: /nl/java/com.aspose.zip/bzip2archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Bzip2Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Deze klasse vertegenwoordigt een bzip2-archiefbestand. Gebruik deze om bzip2-archieven samen te stellen of te extraheren.

bzip2 comprimeert bestanden met behulp van het Burrows-Wheeler bloksorteringstekstcompressie-algoritme en Huffman-codering. Zie meer: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Bzip2Archive()](#Bzip2Archive--) | Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op comprimeren. |
| [Bzip2Archive(InputStream sourceStream)](#Bzip2Archive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op decomprimeren. |
| [Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op decomprimeren. |
| [Bzip2Archive(String path)](#Bzip2Archive-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op decomprimeren. |
| [Bzip2Archive(String path, Bzip2LoadOptions loadOptions)](#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op decomprimeren. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het archief naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het archief naar het bestand op het opgegeven pad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert de inhoud van het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het bzip2-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getName()](#getName--) | De naam van het oorspronkelijke bestand. |
| [open()](#open--) | Opent het archief voor extractie en levert een stream met de archiefinhoud. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(OutputStream outputStream, Bzip2SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-) | Slaat het archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [save(String destinationFileName, Bzip2SaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [setSource(CpioArchive cpioArchive)](#setSource-com.aspose.zip.CpioArchive-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(CpioArchive cpioArchive, CpioFormat format)](#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(File file)](#setSource-java.io.File-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(String path)](#setSource-java.lang.String-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
### Bzip2Archive() {#Bzip2Archive--}
```
public Bzip2Archive()
```


Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op comprimeren.

Het volgende voorbeeld laat zien hoe een bestand te comprimeren.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource("data.bin");
archive.save("archive.bz2");
}
 
```



### Bzip2Archive(InputStream sourceStream) {#Bzip2Archive-java.io.InputStream-}
```
public Bzip2Archive(InputStream sourceStream)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Deze constructor decompresseert niet. Zie de methode [open()](../../com.aspose.zip/bzip2archive\#open--) voor het decomprimeren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |

### Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.io.InputStream-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(InputStream sourceStream, Bzip2LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op decomprimeren.

Open een archief vanuit een stream en extraheer het naar een `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive(new FileInputStream("archive.bz2"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

### Bzip2Archive(String path) {#Bzip2Archive-java.lang.String-}
```
public Bzip2Archive(String path)
```


Initializes a new instance of the [Bzip2Archive](../../com.aspose.zip/bzip2archive) class prepared for decompressing.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Deze constructor decompresseert niet. Zie de methode [open()](../../com.aspose.zip/bzip2archive\#open--) voor het decomprimeren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |

### Bzip2Archive(String path, Bzip2LoadOptions loadOptions) {#Bzip2Archive-java.lang.String-com.aspose.zip.Bzip2LoadOptions-}
```
public Bzip2Archive(String path, Bzip2LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de klasse [Bzip2Archive](../../com.aspose.zip/bzip2archive) voorbereid op decomprimeren.

Open een archief vanuit een bestand via pad en extraheer het naar een `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Bzip2Archive archive = new Bzip2Archive(\"archive.bz2\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/bzip2archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [Bzip2LoadOptions](../../com.aspose.zip/bzip2loadoptions) | the options to load archive with |

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

     try (Bzip2Archive archive = new Bzip2Archive("archive.bz2")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | doelstream. Moet beschrijfbaar zijn. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraheert het archief naar het bestand op het opgegeven pad.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven |

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


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het bzip2-archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het bzip2-archief vormen
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
### open() {#open--}
```
public final InputStream open()
```


Opent het archief voor extractie en levert een stream met de archiefinhoud.


Gebruik:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to an output stream.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | java.io.OutputStream | doelstream. |

### save(OutputStream outputStream, Bzip2SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(OutputStream outputStream, Bzip2SaveOptions saveOptions)
```


Slaat het archief op in de opgegeven stream.

Schrijf gecomprimeerde gegevens naar een uitvoerstream.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream. |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

Writes compressed data to file.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bz2");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### save(String destinationFileName, Bzip2SaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.Bzip2SaveOptions-}
```
public final void save(String destinationFileName, Bzip2SaveOptions saveOptions)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

Schrijft gecomprimeerde gegevens naar een bestand.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"data.bz2\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [Bzip2SaveOptions](../../com.aspose.zip/bzip2saveoptions) | options for saving a bzip2 archive. If not specified, 900 Kb block size would be used |

### setSource(CpioArchive cpioArchive) {#setSource-com.aspose.zip.CpioArchive-}
```
public final void setSource(CpioArchive cpioArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (CpioArchive cpioArchive = new CpioArchive()) {
         cpioArchive.createEntry("first.bin", "data1.bin");
         cpioArchive.createEntry("second.bin", "data2.bin");
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(cpioArchive);
             bzippedArchive.save("archive.cpio.bz2");
         }
     }
 
```

Gebruik deze methode om een gezamenlijk cpio.bz2-archief samen te stellen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | cpio-archief om te comprimeren |

### setSource(CpioArchive cpioArchive, CpioFormat format) {#setSource-com.aspose.zip.CpioArchive-com.aspose.zip.CpioFormat-}
```
public final void setSource(CpioArchive cpioArchive, CpioFormat format)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (CpioArchive cpioArchive = new CpioArchive()) {
cpioArchive.createEntry(\"first.bin\", \"data1.bin\");
cpioArchive.createEntry(\"second.bin\", \"data2.bin\");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(cpioArchive);
bzippedArchive.save(\"archive.cpio.bz2\");
}
}
 
```

Use this method to compose joint cpio.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cpioArchive | [CpioArchive](../../com.aspose.zip/cpioarchive) | cpio archive to be compressed |
| format | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

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
         try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
             bzippedArchive.setSource(tarArchive);
             bzippedArchive.save("archive.tar.bz2");
         }
     }
 
```

Gebruik deze methode om een gezamenlijk tar.bz2-archief samen te stellen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | tar-archief om te comprimeren |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry(\"first.bin\", \"data1.bin\");
tarArchive.createEntry(\"second.bin\", \"data2.bin\");
try (Bzip2Archive bzippedArchive = new Bzip2Archive()) {
bzippedArchive.setSource(tarArchive);
bzippedArchive.save(\"archive.tar.bz2\");
}
}
 
```

Use this method to compose joint tar.bz2 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | tar archive to be compressed |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| file | java.io.File | de referentie naar een bestand dat moet worden gecomprimeerd |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```

``````

try (Bzip2Archive archive = new Bzip2Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.bz2");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (Bzip2Archive archive = new Bzip2Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.bz2");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | pad naar bestand dat moet worden gecomprimeerd |

