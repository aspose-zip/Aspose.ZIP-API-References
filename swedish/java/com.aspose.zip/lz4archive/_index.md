---
title: "Lz4Archive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en LZ4-arkivfil."
type: docs
weight: 80
url: /sv/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Denna klass representerar en LZ4-arkivfil. Använd den för att extrahera eller skapa LZ4-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive) för dekomprimering. |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive) för dekomprimering. |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive()](#Lz4Archive--) | Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive) för komprimering. |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive) för komprimering. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar arkivet till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar arkivet till filen enligt sökväg. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar arkivets innehåll till den angivna katalogen. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getLength()](#getLength--) | Hämtar längd. |
| [getName()](#getName--) | Hämtar det ursprungliga namnet. |
| [open()](#open--) | Öppnar arkivet för extraktion och tillhandahåller en ström med arkivinnehåll. |
| [save(File destination)](#save-java.io.File-) | Sparar lz4-arkivet till den angivna destinationsfilen. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sparar lz4-arkivet till den angivna strömmen. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sparar arkivet till den angivna destinationsfilen. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(File fileInfo)](#setSource-java.io.File-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(String path)](#setSource-java.lang.String-) | Ställer in innehållet som ska komprimeras i arkivet. |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive) för dekomprimering.

Öppna ett arkiv från en ström och extrahera det till en `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream(\"archive.lz4\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Denna konstruktor dekomprimerar inte. Se [open()](../../com.aspose.zip/lz4archive\#open--) metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | källan till arkivet |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Alternativen för att ladda arkivet med. |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive).

Öppna ett arkiv från fil med sökväg och extrahera det till en `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Denna konstruktor dekomprimerar inte. Se [open()](../../com.aspose.zip/lz4archive\#open--) metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till arkivfilen |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Alternativen för att ladda arkivet med. |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive) för komprimering.

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


Initierar en ny instans av klassen [Lz4Archive](../../com.aspose.zip/lz4archive) för komprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | Inställningarna för det sammansatta arkivet. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar arkivet till den angivna strömmen.

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
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


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Läs från strömmen för att få originalinnehållet i en fil. Se avsnittet med exempel.

**Returns:**
java.io.InputStream – strömmen som representerar innehållet i arkivet
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Sparar lz4-arkivet till den angivna destinationsfilen.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lz4\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| utdata | java.io.OutputStream | Destinationsström. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Sparar arkivet till den angivna destinationsfilen.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource("data.bin");
archive.save(\"archive.lz4\");
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
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

Använd den här metoden för att skapa ett gemensamt tar.lz4-arkiv.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar-arkivet som ska komprimeras. |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


Ställer in innehållet som ska komprimeras i arkivet.

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileInfo | java.io.File | Referensen till en fil som ska komprimeras. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ställer in innehållet som ska komprimeras i arkivet.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save(\"archive.lz4\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | Sökväg till fil som ska komprimeras. |

