---
title: "ZstandardArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en Zstandard-arkivfil."
type: docs
weight: 156
url: /sv/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Denna klass representerar en Zstandard-arkivfil. Använd den för att skapa Zstandard-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive) för komprimering. |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive) för dekomprimering. |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive) för dekomprimering. |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar arkivet till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar arkivet till filen enligt sökväg. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar arkivets innehåll till den angivna katalogen. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör zstandard-arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getName()](#getName--) | Hämtar namnet på posten i arkivet. |
| [open()](#open--) | Öppnar arkivet för extraktion och tillhandahåller en ström med arkivinnehåll. |
| [save(File destination)](#save-java.io.File-) | Sparar arkivet till den angivna destinationsfilen. |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | Sparar arkivet till den angivna destinationsfilen. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Sparar arkivet till den angivna strömmen. |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | Sparar arkivet till den angivna strömmen. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sparar arkivet till den angivna destinationsfilen. |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | Sparar arkivet till den angivna destinationsfilen. |
| [setSource(File file)](#setSource-java.io.File-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(String path)](#setSource-java.lang.String-) | Ställer in innehållet som ska komprimeras i arkivet. |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive) för komprimering.

Följande exempel visar hur man komprimerar en fil.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource("data.bin");
archive.save("archive.zst");
}
 
```



### ZstandardArchive(InputStream sourceStream) {#ZstandardArchive-java.io.InputStream-}
```
public ZstandardArchive(InputStream sourceStream)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
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

Denna konstruktor dekomprimerar inte. Se metoden [open()](../../com.aspose.zip/zstandardarchive\\#open--) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | källan till arkivet |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive) för dekomprimering.

Öppna ett arkiv från en ström och extrahera det till en `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream(\"archive.zst\"))) {
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

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### ZstandardArchive(String path) {#ZstandardArchive-java.lang.String-}
```
public ZstandardArchive(String path)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class.

Open an archive from file by path and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
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

Denna konstruktor dekomprimerar inte. Se metoden [open()](../../com.aspose.zip/zstandardarchive\\#open--) för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till arkivfilen |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


Initierar en ny instans av klassen [ZstandardArchive](../../com.aspose.zip/zstandardarchive).

Öppna ett arkiv från en fil via sökväg och extrahera det till en `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(\"archive.zst\")) {
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

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

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

     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | destinationsström. Måste vara skrivbar |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar arkivet till filen enligt sökväg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till destinationsfilen. Om filen redan finns kommer den att skrivas över. |

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
|  | destinationDirectory | java.lang.String | sökvägen till katalogen där de extraherade filerna ska placeras. |

Om katalogen inte finns, kommer den att skapas |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör zstandard-arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör zstandard-arkivet
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


Hämtar längden på posten i byte.

**Returns:**
java.lang.Long - längden på posten i byte
### getName() {#getName--}
```
public final String getName()
```


Hämtar namnet på posten i arkivet.

**Returns:**
java.lang.String - namnet på posten i arkivet
### open() {#open--}
```
public final InputStream open()
```


Öppnar arkivet för extraktion och tillhandahåller en ström med arkivinnehåll.

Extraherar arkivet och kopierar extraherat innehåll till filström.

```

``````

try (ZstandardArchive archive = new ZstandardArchive(\"archive.zst\")) {
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

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.zst"));
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.File | filen som kommer att öppnas som destinationsström |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


Sparar arkivet till den angivna destinationsfilen.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.zst\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destinationsströmmen |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


Sparar arkivet till den angivna strömmen.

Skriv komprimerad data till http-svarsströmmen.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | the destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.zst");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | java.lang.String | sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


Sparar arkivet till den angivna destinationsfilen.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.zst\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | java.io.File | referensen till en fil som ska komprimeras |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ställer in innehållet som ska komprimeras i arkivet.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save("archive.zst");
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

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökväg till fil som ska komprimeras |

