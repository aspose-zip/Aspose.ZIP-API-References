---
title: "GzipArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en gzip-arkivfil."
type: docs
weight: 69
url: /sv/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Denna klass representerar en gzip-arkivfil. Använd den för att skapa eller extrahera gzip-arkiv.

Gzip-komprimeringsalgoritmen är baserad på DEFLATE-algoritmen, som är en kombination av LZ77 och Huffman-kodning.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för komprimering. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för dekomprimering. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för dekomprimering. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för dekomprimering. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för dekomprimering. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive). |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar arkivet till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar arkivet till filen enligt sökväg. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar arkivets innehåll till den angivna katalogen. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör gzip-arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getLength()](#getLength--) | Hämtar storleken på en originalfil. |
| [getName()](#getName--) | Namnet på originalfilen. |
| [getUncompressedSize()](#getUncompressedSize--) | Hämtar storleken på en originalfil. |
| [open()](#open--) | Öppnar arkivet för extraktion och tillhandahåller en ström med arkivinnehåll. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Sparar arkivet till den angivna strömmen. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sparar arkivet till den angivna destinationsfilen. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(File file)](#setSource-java.io.File-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(String path)](#setSource-java.lang.String-) | Ställer in innehållet som ska komprimeras i arkivet. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för komprimering.

Följande exempel visar hur man komprimerar en fil.

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

Denna konstruktor dekomprimerar inte. Se metoden [open()](../../com.aspose.zip/gziparchive\#open--) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Källan till arkivet. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för dekomprimering.

Öppna ett arkiv från en ström och extrahera det till en `ByteArrayOutputStream`

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

Denna konstruktor dekomprimerar inte. Se metoden [open()](../../com.aspose.zip/gziparchive\#open--) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Källan till arkivet. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Alternativ för att läsa in arkivet med. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive) för dekomprimering.

Öppna ett arkiv från fil med sökväg och extrahera det till en `MemoryStream`

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

Denna konstruktor dekomprimerar inte. Se metoden [open()](../../com.aspose.zip/gziparchive\#open--) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | Sökvägen till arkivfilen. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Initierar en ny instans av klassen [GzipArchive](../../com.aspose.zip/gziparchive).

Öppna ett arkiv från fil med sökväg och extrahera det till en `MemoryStream`

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | Destinationsström. Måste vara skrivbar. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar arkivet till filen enligt sökväg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | Sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

**Returns:**
java.io.File - filinformationen för den extraherade filen
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraherar arkivets innehåll till den angivna katalogen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | Sökvägen till katalogen där de extraherade filerna ska placeras. |

Om katalogen inte finns, kommer den att skapas. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör gzip-arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör gzip-arkivet.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Hämtar arkivformatet.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Hämtar storleken på en originalfil.

Under dekomprimering kan den här egenskapen innehålla felaktig storlek. Om den dekomprimerade filstorleken överstiger 4 GB kommer egenskapen att ge ett felaktigt värde på grund av 32-bitsgränsen i headern.

**Returns:**
java.lang.Long - storlek på en originalfil
### getName() {#getName--}
```
public final String getName()
```


Namnet på originalfilen.

**Returns:**
java.lang.String - namnet på den ursprungliga filen
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Hämtar storleken på en originalfil.

Under dekomprimering kan den här egenskapen innehålla felaktig storlek. Om den dekomprimerade filstorleken överstiger 4 GB kommer egenskapen att ge ett felaktigt värde på grund av 32-bitsgränsen i headern.

**Returns:**
long - storlek på en originalfil.
### open() {#open--}
```
public final InputStream open()
```


Öppnar arkivet för extraktion och tillhandahåller en ström med arkivinnehåll.

Extraherar arkivet och kopierar extraherat innehåll till filström.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
try (FileOutputStream extracted = new FileOutputStream(\"data.bin\")) {
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Destinationsström. |

`outputStream` måste vara skrivbar. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Sparar arkivet till den angivna destinationsfilen.

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

Använd den här metoden för att skapa ett gemensamt tar.gz-arkiv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar-arkivet som ska komprimeras. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Ställer in innehållet som ska komprimeras i arkivet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | java.io.InputStream | Inmatningsströmmen för arkivet. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Ställer in innehållet som ska komprimeras i arkivet.

Öppna ett arkiv från fil med sökväg och extrahera det till en `MemoryStream`

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

