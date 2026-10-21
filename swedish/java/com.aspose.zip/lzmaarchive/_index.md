---
title: "LzmaArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en LZMA-arkivfil."
type: docs
weight: 86
url: /sv/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Denna klass representerar en LZMA-arkivfil. Använd den för att skapa eller extrahera LZMA-arkiv.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) och skapar arkivet i lzma-format. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) och skapar arkivet i lzma-format. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) för dekomprimering. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) för dekomprimering. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extraherar lzma-arkivet till en fil. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar lzma-arkivet till en ström. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar lzma-arkivet till en fil via sökväg. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar arkivets innehåll till den angivna katalogen. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör lzma-arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getLength()](#getLength--) | Hämtar längd. |
| [getName()](#getName--) | Namnet på den ursprungliga filen. |
| [save(File destination)](#save-java.io.File-) | Sparar lzma-arkivet till den angivna destinationsfilen. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sparar lzma-arkivet till den angivna strömmen. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sparar lzma-arkivet till den angivna destinationsfilen. |
| [setSource(File file)](#setSource-java.io.File-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Ställer in innehållet som ska komprimeras i arkivet. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) och skapar arkivet i lzma-format.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) och skapar arkivet i lzma-format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | uppsättning av inställningar för ett specifikt lzma-arkiv |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) för dekomprimering.

Denna konstruktor dekomprimerar inte. Se [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | java.io.InputStream | källan till arkivet |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Initierar en ny instans av klassen [LzmaArchive](../../com.aspose.zip/lzmaarchive) för dekomprimering.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | java.io.File | filen för att lagra dekomprimerad data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extraherar lzma-arkivet till en ström.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till filen som kommer att lagra dekomprimerad data |

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


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör lzma-arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör lzma-arkivet.
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


Namnet på den ursprungliga filen.

**Returns:**
java.lang.String - namnet på den ursprungliga filen
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Sparar lzma-arkivet till den angivna destinationsfilen.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| utdata | java.io.OutputStream | målström |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Sparar lzma-arkivet till den angivna destinationsfilen.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | java.io.File | filen, som kommer att öppnas som inmatningsström |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ställer in innehållet som ska komprimeras i arkivet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourcePath | java.lang.String | sökväg till filen som kommer att öppnas som inmatningsström |

