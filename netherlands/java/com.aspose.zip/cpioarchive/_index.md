---
title: "CpioArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een cpio-archiefbestand."
type: docs
weight: 57
url: /nl/java/com.aspose.zip/cpioarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class CpioArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een cpio-archiefbestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CpioArchive()](#CpioArchive--) | Initialiseert een nieuw exemplaar van de klasse [CpioArchive](../../com.aspose.zip/cpioarchive). |
| [CpioArchive(InputStream sourceStream)](#CpioArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de klasse [CpioArchive](../../com.aspose.zip/cpioarchive) en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd. |
| [CpioArchive(String path)](#CpioArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [CpioArchive](../../com.aspose.zip/cpioarchive) en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Maakt een enkel item binnen het archief. |
| [deleteEntry(CpioEntry entry)](#deleteEntry-com.aspose.zip.CpioEntry-) | Verwijdert de eerste voorkoming van een specifiek item uit de itemlijst. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Verwijdert het item uit de itemslijst op index. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden in het archief naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt items op van het type [CpioEntry](../../com.aspose.zip/cpioentry) die het cpio-archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) dat het cpio-archief vormt. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(OutputStream output, CpioFormat cpioFormat)](#save-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Slaat het archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [save(String destinationFileName, CpioFormat cpioFormat)](#save-java.lang.String-com.aspose.zip.CpioFormat-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Slaat het archief op naar de stream met gzip-compressie. |
| [saveGzipped(OutputStream output, CpioFormat cpioFormat)](#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Slaat het archief op naar de stream met gzip-compressie. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Slaat het archief op naar het bestand via pad met gzip-compressie. |
| [saveGzipped(String path, CpioFormat cpioFormat)](#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Slaat het archief op naar het bestand via pad met gzip-compressie. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Slaat het archief op naar de stream met LZMA-compressie. |
| [saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Slaat het archief op naar de stream met LZMA-compressie. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Slaat het archief op naar het bestand via pad met lzma-compressie. |
| [saveLZMACompressed(String path, CpioFormat cpioFormat)](#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Slaat het archief op naar het bestand via pad met lzma-compressie. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Slaat het archief op naar de stream met lzip-compressie. |
| [saveLzipped(OutputStream output, CpioFormat cpioFormat)](#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Slaat het archief op naar de stream met lzip-compressie. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Slaat het archief op naar het bestand via pad met lzip-compressie. |
| [saveLzipped(String path, CpioFormat cpioFormat)](#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-) | Slaat het archief op naar het bestand via pad met lzip-compressie. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Slaat het archief op naar de stream met xz-compressie. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Slaat het archief op naar de stream met xz-compressie. |
| [saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Slaat het archief op naar de stream met xz-compressie. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Slaat het archief op naar het bestand via pad met xz-compressie. |
| [saveXzCompressed(String path, CpioFormat cpioFormat)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Slaat het archief op naar het bestand via pad met xz-compressie. |
| [saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-) | Slaat het archief op naar het bestand via pad met xz-compressie. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Slaat het archief op naar de stream met Z-compressie. |
| [saveZCompressed(OutputStream output, CpioFormat cpioFormat)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Slaat het archief op naar de stream met Z-compressie. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Slaat het archief op naar het bestand via pad met Z-compressie. |
| [saveZCompressed(String path, CpioFormat cpioFormat)](#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-) | Slaat het archief op naar het bestand via pad met Z-compressie. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Slaat het archief op naar de stream met Zstandard-compressie. |
| [saveZstandard(OutputStream output, CpioFormat cpioFormat)](#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-) | Slaat het archief op naar de stream met Zstandard-compressie. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Slaat het archief op naar het bestand via pad met Zstandard-compressie. |
| [saveZstandard(String path, CpioFormat cpioFormat)](#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-) | Slaat het archief op naar het bestand via pad met Zstandard-compressie. |
### CpioArchive() {#CpioArchive--}
```
public CpioArchive()
```


Initialiseert een nieuw exemplaar van de klasse [CpioArchive](../../com.aspose.zip/cpioarchive).

Het volgende voorbeeld laat zien hoe een bestand te comprimeren.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```



### CpioArchive(InputStream sourceStream) {#CpioArchive-java.io.InputStream-}
```
public CpioArchive(InputStream sourceStream)
```


Initializes a new instance of the [CpioArchive](../../com.aspose.zip/cpioarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CpioArchive archive = new CpioArchive(new FileInputStream("archive.cpio"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Deze constructor pakt geen enkele entry uit. Zie de methode [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |

### CpioArchive(String path) {#CpioArchive-java.lang.String-}
```
public CpioArchive(String path)
```


Initialiseert een nieuw exemplaar van de klasse [CpioArchive](../../com.aspose.zip/cpioarchive) en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CpioEntry.open()](../../com.aspose.zip/cpioentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CpioArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | java.io.File | directory om te comprimeren |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CpioArchive createEntries(File directory, boolean includeRootDirectory)
```


Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CpioArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory om te comprimeren |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CpioArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final CpioEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new File("data.bin");
     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| file | java.io.File | de metadata van het bestand of de map die moet worden gecomprimeerd |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final CpioEntry createEntry(String name, File file, boolean openImmediately)
```


Maakt een enkel item binnen het archief.

```

``````

java.io.File file = new File("data.bin");
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CpioEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.cpio");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| source | java.io.InputStream | de invoerstroom voor de entry |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final CpioEntry createEntry(String name, String sourcePath)
```


Maakt een enkel item binnen het archief.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.cpio");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | path to file to be compressed. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final CpioEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.cpio");
     }
 
```

De entrynaam wordt uitsluitend ingesteld via de `name`-parameter. De bestandsnaam die wordt opgegeven in de `sourcePath`-parameter heeft geen invloed op de entrynaam

Als het bestand onmiddellijk wordt geopend met de `openImmediately`-parameter, wordt het geblokkeerd totdat het archief wordt vrijgegeven

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| sourcePath | java.lang.String | pad naar het te comprimeren bestand. |
| openImmediately | boolean | true, als het bestand onmiddellijk wordt geopend, anders wordt het bestand geopend bij het opslaan van het archief. |

**Returns:**
[CpioEntry](../../com.aspose.zip/cpioentry) - cpio entry instance
### deleteEntry(CpioEntry entry) {#deleteEntry-com.aspose.zip.CpioEntry-}
```
public final CpioArchive deleteEntry(CpioEntry entry)
```


Verwijdert de eerste voorkoming van een specifiek item uit de itemlijst.

Hier ziet u hoe u alle entries behalve de laatste kunt verwijderen:

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputCpioFile.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [CpioEntry](../../com.aspose.zip/cpioentry) | the entry to remove from the entries list |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - cpio entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final CpioArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (CpioArchive archive = new CpioArchive("two_files.cpio")) {
         archive.deleteEntry(0);
         archive.save("single_file.cpio");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entryIndex | int | de nulgebaseerde index van de te verwijderen entry |

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert alle bestanden in het archief naar de opgegeven map.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<CpioEntry> getEntries()
```


Gets entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.

**Returns:**
java.util.List&lt;com.aspose.zip.CpioEntry&gt; - entries of [CpioEntry](../../com.aspose.zip/cpioentry) type constituting the cpio archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the cpio archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(cpioFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |

### save(OutputStream output, CpioFormat cpioFormat) {#save-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void save(OutputStream output, CpioFormat cpioFormat)
```


Slaat het archief op in de opgegeven stream.

```

``````

try (FileOutputStream cpioFile = new FileOutputStream("archive.cpio")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(cpioFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (CpioArchive archive = new CpioArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.cpio");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt dit overschreven. |

Het is mogelijk om een archief op hetzelfde pad op te slaan als waar het vandaan is geladen. Dit wordt echter niet aanbevolen omdat deze aanpak een kopie naar een tijdelijk bestand maakt |

### save(String destinationFileName, CpioFormat cpioFormat) {#save-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void save(String destinationFileName, CpioFormat cpioFormat)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

```

``````

try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("archive.cpio");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |

### saveGzipped(OutputStream output, CpioFormat cpioFormat) {#saveGzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(OutputStream output, CpioFormat cpioFormat)
```


Slaat het archief op naar de stream met gzip-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.cpio.gz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### saveGzipped(String path, CpioFormat cpioFormat) {#saveGzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveGzipped(String path, CpioFormat cpioFormat)
```


Slaat het archief op naar het bestand via pad met gzip-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.cpio.gz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Saves the archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Belangrijk: cpio-archief wordt samengesteld en vervolgens gecomprimeerd binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |

### saveLZMACompressed(OutputStream output, CpioFormat cpioFormat) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(OutputStream output, CpioFormat cpioFormat)
```


Slaat het archief op naar de stream met LZMA-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Saves the archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.cpio.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Belangrijk: cpio-archief wordt samengesteld en vervolgens gecomprimeerd binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### saveLZMACompressed(String path, CpioFormat cpioFormat) {#saveLZMACompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLZMACompressed(String path, CpioFormat cpioFormat)
```


Slaat het archief op naar het bestand via pad met lzma-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.cpio.lzma");
}
} catch (IOException ex) {
}
 
```

Important: cpio archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |

### saveLzipped(OutputStream output, CpioFormat cpioFormat) {#saveLzipped-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(OutputStream output, CpioFormat cpioFormat)
```


Slaat het archief op naar de stream met lzip-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.cpio.lz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### saveLzipped(String path, CpioFormat cpioFormat) {#saveLzipped-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveLzipped(String path, CpioFormat cpioFormat)
```


Slaat het archief op naar het bestand via pad met lzip-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.cpio.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output`De stream moet schrijfbaar zijn |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat)
```


Slaat het archief op naar de stream met xz-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output`De stream moet schrijfbaar zijn. |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | definieert cpio-headerformaat |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | instelling van specifieke xz-archief: woordenboekgrootte, blokgrootte, controletype |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Slaat het archief op naar het bestand via pad met xz-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveXzCompressed(String path, CpioFormat cpioFormat) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.cpio.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | definieert cpio-headerformaat |

### saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.CpioFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, CpioFormat cpioFormat, XzArchiveSettings settings)
```


Slaat het archief op naar het bestand via pad met xz-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.cpio.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | de bestemmingsstroom. |

`output` moet schrijfbaar zijn |

### saveZCompressed(OutputStream output, CpioFormat cpioFormat) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(OutputStream output, CpioFormat cpioFormat)
```


Slaat het archief op naar de stream met Z-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.cpio.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### saveZCompressed(String path, CpioFormat cpioFormat) {#saveZCompressed-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZCompressed(String path, CpioFormat cpioFormat)
```


Slaat het archief op naar het bestand via pad met Z-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.cpio.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | d cpio header format |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (CpioArchive archive = new CpioArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |

### saveZstandard(OutputStream output, CpioFormat cpioFormat) {#saveZstandard-java.io.OutputStream-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(OutputStream output, CpioFormat cpioFormat)
```


Slaat het archief op naar de stream met Zstandard-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.cpio.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (CpioArchive archive = new CpioArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.cpio.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### saveZstandard(String path, CpioFormat cpioFormat) {#saveZstandard-java.lang.String-com.aspose.zip.CpioFormat-}
```
public final void saveZstandard(String path, CpioFormat cpioFormat)
```


Slaat het archief op naar het bestand via pad met Zstandard-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (CpioArchive archive = new CpioArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.cpio.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| cpioFormat | [CpioFormat](../../com.aspose.zip/cpioformat) | defines cpio header format |

