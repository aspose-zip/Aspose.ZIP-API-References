---
title: "UueArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een uuencoded-bestand."
type: docs
weight: 128
url: /nl/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Deze klasse vertegenwoordigt een uuencoded-bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [UueArchive()](#UueArchive--) | Initialiseert een nieuw exemplaar van de [UueArchive](../../com.aspose.zip/uuearchive) klasse, voorbereid voor codering. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [UueArchive](../../com.aspose.zip/uuearchive) klasse, voorbereid voor decodering. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [UueArchive](../../com.aspose.zip/uuearchive) klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraheert het archief naar de opgegeven stream. |
| [extract(String path)](#extract-java.lang.String-) | Extraheert het archief naar het bestand op het opgegeven pad. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert de inhoud van het archief naar de opgegeven map. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het uue-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getLength()](#getLength--) | Haalt de lengte op. |
| [getName()](#getName--) | Naam van het oorspronkelijke bestand. |
| [open()](#open--) | Opent het archief voor decodering en levert een stream met de archiefinhoud. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | Slaat het archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [setSource(File file)](#setSource-java.io.File-) | Stelt de inhoud in die binnen het archief moet worden gecomprimeerd. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Stelt de inhoud in die in het archief moet worden gecodeerd. |
| [setSource(String path)](#setSource-java.lang.String-) | Stelt de inhoud in die in het archief moet worden gecodeerd. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


Initialiseert een nieuw exemplaar van de [UueArchive](../../com.aspose.zip/uuearchive) klasse, voorbereid voor codering.

Het volgende voorbeeld toont hoe een bestand te uuencoden.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource("data.bin");
archive.save("archive.uue");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Deze constructor decodeert niet. Zie de [open()](../../com.aspose.zip/uuearchive\#open--) methode voor decompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


Initialiseert een nieuw exemplaar van de [UueArchive](../../com.aspose.zip/uuearchive) klasse.

Open een archief vanaf een bestandspad en decodeer het naar een `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream("archive.uue"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

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

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | java.io.OutputStream | bestemmingsstroom |

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
java.io.File - informatie van het uitgepakte bestand
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


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het uue-archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het uue-archief vormen
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


Naam van het oorspronkelijke bestand.

**Returns:**
java.lang.String - de naam van het oorspronkelijke bestand
### open() {#open--}
```
public final InputStream open()
```


Opent het archief voor decodering en levert een stream met de archiefinhoud.

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

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | java.io.OutputStream | bestemmingsstroom |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


Slaat het archief op in de opgegeven stream.

Schrijf gecomprimeerde data naar de http-responsestream.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

Schrijf gecodeerde gegevens naar bestand.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
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


Stelt de inhoud in die in het archief moet worden gecodeerd.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.uue");
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


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | pad naar bestand dat moet worden gecodeerd |

