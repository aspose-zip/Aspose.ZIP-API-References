---
title: "ZArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en Z-komprimeringsarkivfil."
type: docs
weight: 153
url: /sv/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Denna klass representerar en Z (compress) arkivfil. Använd den för att komponera eller extrahera Z-arkiv.

Se [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ZArchive()](#ZArchive--) | Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för komprimering. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extraherar Z-arkivet till en fil. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extraherar Z-arkivet till en ström. |
| [extract(String path)](#extract-java.lang.String-) | Extraherar Z-arkivet till en fil enligt sökväg. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar arkivets innehåll till den angivna katalogen. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör Z-arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getLength()](#getLength--) | Hämtar längden på posten i byte. |
| [getName()](#getName--) | Hämtar namnet på posten i arkivet. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sparar Z-arkivet till den angivna strömmen. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Sparar Z-arkivet till den angivna strömmen. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sparar Z-arkivet till den angivna destinationsfilen. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Sparar Z-arkivet till den angivna destinationsfilen. |
| [setSource(File file)](#setSource-java.io.File-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Ställer in innehållet som ska komprimeras i arkivet. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Ställer in innehållet som ska komprimeras i arkivet. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för komprimering.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering.

Den här konstruktorn dekomprimerar inte. Se [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | java.io.InputStream | källan till arkivet |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering.

Den här konstruktorn dekomprimerar inte. Se [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | java.io.InputStream | källan till arkivet |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | alternativen för att ladda arkivet med |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering.

Den här konstruktorn dekomprimerar inte. Se [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till källan för arkivet |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Initierar en ny instans av klassen [ZArchive](../../com.aspose.zip/zarchive) för dekomprimering.

Den här konstruktorn dekomprimerar inte. Se [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) metoden för dekomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till källan för arkivet |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | alternativen för att ladda arkivet med |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extraherar Z-arkivet till en fil.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract(new File(\"extracted.bin\"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | java.io.OutputStream | strömmen för att lagra dekomprimerade data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extraherar Z-arkivet till en fil enligt sökväg.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract(\"extracted.bin\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| utdata | java.io.OutputStream | destinationsströmmen |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Sparar Z-arkivet till den angivna strömmen.

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | java.lang.String | sökvägen till arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Sparar Z-arkivet till den angivna destinationsfilen.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| file | java.io.File | filinformationen som kommer att öppnas som inmatningsström |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Ställer in innehållet som ska komprimeras i arkivet.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
});
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourcePath | java.lang.String | sökvägen till filen som kommer att öppnas som inmatningsström |

