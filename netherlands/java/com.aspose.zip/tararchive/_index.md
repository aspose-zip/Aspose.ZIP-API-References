---
title: "TarArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een tar-archiefbestand."
type: docs
weight: 125
url: /nl/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een tar‑archiefbestand. Gebruik deze om tar‑archieven samen te stellen, uit te pakken of bij te werken.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TarArchive()](#TarArchive--) | Initialiseert een nieuw exemplaar van de klasse [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [Archive](../../com.aspose.zip/archive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [TarArchive](../../com.aspose.zip/tararchive) en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd. |
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
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Maakt een enkel item binnen het archief. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Verwijdert de eerste voorkoming van een specifiek item uit de itemlijst. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Verwijdert het item uit de itemslijst op index. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden in het archief naar de opgegeven map. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Extraheert het opgegeven gzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Extraheert het opgegeven gzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Extraheert het opgegeven LZ4‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Extraheert het opgegeven LZ4‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Extraheert het opgegeven LZMA‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Extraheert het opgegeven LZMA‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Extraheert het opgegeven lzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Extraheert het opgegeven lzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Extraheert het opgegeven xz‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Extraheert het opgegeven xz‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Extraheert het opgegeven Z‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Extraheert het opgegeven Z‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Extraheert het opgegeven Zstandard‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Extraheert het opgegeven Zstandard‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens. |
| [getEntries()](#getEntries--) | Haalt items op van het type [TarEntry](../../com.aspose.zip/tarentry) die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het tar‑archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Slaat het archief op naar de stream met gzip-compressie. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op naar de stream met gzip-compressie. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Slaat het archief op naar het bestand via pad met gzip-compressie. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op naar het bestand via pad met gzip-compressie. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Slaat het archief op in de stream met LZ4‑compressie. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op in de stream met LZ4‑compressie. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Slaat het archief op in het bestand via pad met LZ4‑compressie. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op in het bestand via pad met LZ4‑compressie. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Slaat het archief op in de stream met LZMA‑compressie. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op in de stream met LZMA‑compressie. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Slaat het archief op in het bestand via pad met LZMA‑compressie. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op in het bestand via pad met LZMA‑compressie. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Slaat het archief op naar de stream met lzip-compressie. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op naar de stream met lzip-compressie. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Slaat het archief op naar het bestand via pad met lzip-compressie. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op naar het bestand via pad met lzip-compressie. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Slaat het archief op naar de stream met xz-compressie. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op naar de stream met xz-compressie. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Slaat het archief op naar de stream met xz-compressie. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Slaat het archief op naar het bestand via pad met xz-compressie. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op naar het bestand via pad met xz-compressie. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Slaat het archief op naar het bestand via pad met xz-compressie. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Slaat het archief op naar de stream met Z-compressie. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op naar de stream met Z-compressie. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Slaat het archief op naar het bestand via pad met Z-compressie. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op naar het bestand via pad met Z-compressie. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Slaat het archief op naar de stream met Zstandard-compressie. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Slaat het archief op naar de stream met Zstandard-compressie. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Slaat het archief op naar het bestand via pad met Zstandard-compressie. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Slaat het archief op naar het bestand via pad met Zstandard-compressie. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Initialiseert een nieuw exemplaar van de klasse [TarArchive](../../com.aspose.zip/tararchive).

Het volgende voorbeeld laat zien hoe een bestand te comprimeren.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Deze constructor pakt geen enkele entry uit. Zie [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) methode voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Initialiseert een nieuw exemplaar van de klasse [TarArchive](../../com.aspose.zip/tararchive) en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

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
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | java.io.File | directory om te comprimeren |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory om te comprimeren |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

De naam van het item wordt uitsluitend ingesteld via de `name`‑parameter. De bestandsnaam die wordt opgegeven in de `file`‑parameter heeft geen invloed op de naam van het item.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| file | java.io.File | de metadata van het bestand of de map die moet worden gecomprimeerd |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Maakt een enkel item binnen het archief.

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

De entrynaam wordt uitsluitend ingesteld binnen de `name` parameter.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| source | java.io.InputStream | de invoerstroom voor de entry |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Maakt een enkel item binnen het archief.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

De itemnaam wordt uitsluitend ingesteld via de `name`-parameter. De bestandsnaam die wordt opgegeven in de `path`-parameter heeft geen invloed op de itemnaam.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| path | java.lang.String | pad naar bestand dat moet worden gecomprimeerd |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Maakt een enkel item binnen het archief.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | de entry die verwijderd moet worden uit de lijst met entries |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Verwijdert het item uit de itemslijst op index.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Als de map niet bestaat, wordt deze aangemaakt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | java.lang.String | het pad naar de map waarin de geëxtraheerde bestanden worden geplaatst |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Extraheert het opgegeven gzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: gzip-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

GZip-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record uit te pakken, dus moet het onder de motorkap met een doorzoekbare stroom werken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Extraheert het opgegeven gzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: gzip-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

GZip-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record uit te pakken, dus moet het onder de motorkap met een doorzoekbare stroom werken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Extraheert het opgegeven LZ4‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: LZ4-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | source | java.io.InputStream | De bron van het archief. |

LZ4-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Extraheert het opgegeven LZ4‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: LZ4-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | path | java.lang.String | Het pad naar het archiefbestand. |

LZ4-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Extraheert het opgegeven LZMA‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: LZMA-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

LZMA-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Extraheert het opgegeven LZMA‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: LZMA-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

LZMA-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Extraheert het opgegeven lzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: lzip-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

Lzip-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Extraheert het opgegeven lzip‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: lzip-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

Lzip-extractiestroom is niet doorzoekbaar vanwege de aard van het compressie‑algoritme. Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Extraheert het opgegeven xz‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: xz-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Extraheert het opgegeven xz‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: xz-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

Tar‑archief biedt de mogelijkheid om een willekeurig record te extraheren, dus moet het onder de motorkap een doorzoekbare stroom gebruiken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Extraheert het opgegeven Z‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: Z-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Extraheert het opgegeven Z‑formaatarchief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: Z-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Extraheert het opgegeven Zstandard‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: Zstandard-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | java.io.InputStream | de bron van het archief |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Extraheert het opgegeven Zstandard‑archief en stelt een [TarArchive](../../com.aspose.zip/tararchive) samen uit de geëxtraheerde gegevens.

Belangrijk: Zstandard-archief wordt volledig uitgepakt binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Haalt items op van het type [TarEntry](../../com.aspose.zip/tarentry) die het archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - items van het type [TarEntry](../../com.aspose.zip/tarentry) die het archief vormen
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het tar‑archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het tar‑archief vormen
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Slaat het archief op in de opgegeven stream.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(\"myarchive.tar\");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

Het is mogelijk om een archief op hetzelfde pad op te slaan als waar het werd geladen. Dit wordt echter niet aanbevolen omdat deze aanpak een kopie naar een tijdelijk bestand maakt

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt dit overschreven. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Slaat het archief op naar de stream met gzip-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream(\"result.tar.gz\")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Slaat het archief op naar het bestand via pad met gzip-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(\"result.tar.gz\");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Slaat het archief op in de stream met LZ4‑compressie.

```

``````

try (FileOutputStream result = new FileOutputStream(\"result.tar.lz4\")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | java.io.OutputStream | Doelstream. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Slaat het archief op in het bestand via pad met LZ4‑compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt dit overschreven. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Slaat het archief op in de stream met LZMA‑compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Belangrijk: het tar-archief wordt samengesteld en vervolgens gecomprimeerd binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | doelstream. |

`output` moet schrijfbaar zijn |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Slaat het archief op in het bestand via pad met LZMA‑compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Belangrijk: het tar-archief wordt samengesteld en vervolgens gecomprimeerd binnen deze methode, de inhoud wordt intern bewaard. Let op het geheugenverbruik.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Slaat het archief op naar de stream met lzip-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Slaat het archief op naar het bestand via pad met lzip-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Slaat het archief op naar de stream met xz-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Slaat het archief op naar de stream met xz-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Slaat het archief op naar het bestand via pad met xz-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | instelling van specifieke xz-archief: woordenboekgrootte, blokgrootte, controletype |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Slaat het archief op naar de stream met Z-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| output | java.io.OutputStream | de bestemmingsstream |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Slaat het archief op naar het bestand via pad met Z-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Slaat het archief op naar de stream met Zstandard-compressie.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
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

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
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
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Slaat het archief op naar het bestand via pad met Zstandard-compressie.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definieert het tar‑headerformaat. Een null‑waarde wordt, indien mogelijk, behandeld als USTar |

