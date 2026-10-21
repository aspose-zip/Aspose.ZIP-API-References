---
title: "UueArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en uu-kodad fil."
type: docs
weight: 128
url: /sv/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Denna klass representerar en uu-kodad fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [UueArchive()](#UueArchive--) | Initierar en ny instans av klassen [UueArchive](../../com.aspose.zip/uuearchive) för kodning. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | Initierar en ny instans av klassen [UueArchive](../../com.aspose.zip/uuearchive) för avkodning. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | Initierar en ny instans av klassen [UueArchive](../../com.aspose.zip/uuearchive). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar arkivet till den angivna strömmen. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar arkivet till filen enligt sökväg. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar arkivets innehåll till den angivna katalogen. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör uue‑arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getLength()](#getLength--) | Hämtar längd. |
| [getName()](#getName--) | Namn på den ursprungliga filen. |
| [open()](#open--) | Öppnar arkivet för avkodning och tillhandahåller en ström med arkivinnehållet. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Sparar arkivet till den angivna strömmen. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | Sparar arkivet till den angivna strömmen. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sparar arkivet till den angivna destinationsfilen. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | Sparar arkivet till den angivna destinationsfilen. |
| [setSource(File file)](#setSource-java.io.File-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ställer in innehållet som ska kodas i arkivet. |
| [setSource(String path)](#setSource-java.lang.String-) | Ställer in innehållet som ska kodas i arkivet. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


Initierar en ny instans av klassen [UueArchive](../../com.aspose.zip/uuearchive) för kodning.

Följande exempel visar hur man uuencodar en fil.

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

Denna konstruktor avkodar inte. Se [open()](../../com.aspose.zip/uuearchive\#open--)‑metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | källan till arkivet |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


Initierar en ny instans av klassen [UueArchive](../../com.aspose.zip/uuearchive).

Öppna ett arkiv från fil via sökväg och avkoda det till en `MemoryStream`

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | målström |

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
java.io.File – information om den extraherade filen
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


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör uue‑arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; – poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör uue‑arkivet
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


Hämtar längd.

**Returns:**
java.lang.Long - längd
### getName() {#getName--}
```
public final String getName()
```


Namn på den ursprungliga filen.

**Returns:**
java.lang.String - namnet på den ursprungliga filen
### open() {#open--}
```
public final InputStream open()
```


Öppnar arkivet för avkodning och tillhandahåller en ström med arkivinnehållet.

Användning:

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| outputStream | java.io.OutputStream | målström |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


Sparar arkivet till den angivna strömmen.

Skriv komprimerad data till http-svarsströmmen.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | java.lang.String | sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


Sparar arkivet till den angivna destinationsfilen.

Skriv kodad data till fil.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | java.io.File | referensen till en fil som ska komprimeras |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ställer in innehållet som ska kodas i arkivet.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökväg till fil som ska kodas |

