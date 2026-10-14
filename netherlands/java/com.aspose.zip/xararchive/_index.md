---
title: "XarArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een xar-archiefbestand."
type: docs
weight: 136
url: /nl/java/com.aspose.zip/xararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XarArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een xar-archiefbestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XarArchive()](#XarArchive--) | Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(XarCompressionSettings defaultCompressionSettings)](#XarArchive-com.aspose.zip.XarCompressionSettings-) | Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(InputStream sourceStream)](#XarArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive) en stelt een lijst met items samen die uit het archief kunnen worden gehaald. |
| [XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)](#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive) en stelt een lijst met items samen die uit het archief kunnen worden gehaald. |
| [XarArchive(String path)](#XarArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive) en stelt een lijst met items samen die uit het archief kunnen worden gehaald. |
| [XarArchive(String path, XarLoadOptions loadOptions)](#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-) | Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive) en stelt een lijst met items samen die uit het archief kunnen worden gehaald. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Maak een enkel item binnen het archief. |
| [deleteEntry(XarEntry entry)](#deleteEntry-com.aspose.zip.XarEntry-) | Verwijdert de eerste voorkoming van een specifiek item uit de itemlijst. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden in het archief naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt items op van het type [XarEntry](../../com.aspose.zip/xarentry) die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het xar‑archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(OutputStream output, XarSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-) | Slaat het archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [save(String destinationFileName, XarSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.XarSaveOptions-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
### XarArchive() {#XarArchive--}
```
public XarArchive()
```


Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive).

Het volgende voorbeeld laat zien hoe een bestand te comprimeren.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```



### XarArchive(XarCompressionSettings defaultCompressionSettings) {#XarArchive-com.aspose.zip.XarCompressionSettings-}
```
public XarArchive(XarCompressionSettings defaultCompressionSettings)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class.

The following example shows how to compress a file.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| defaultCompressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | de standaardcompressie-instellingen, toegepast op alle items van het archief |

### XarArchive(InputStream sourceStream) {#XarArchive-java.io.InputStream-}
```
public XarArchive(InputStream sourceStream)
```


Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive) en stelt een lijst met items samen die uit het archief kunnen worden gehaald.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### XarArchive(InputStream sourceStream, XarLoadOptions loadOptions) {#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Deze constructor pakt geen enkel item uit. Zie de methode [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | de opties om het archief mee te laden |

### XarArchive(String path) {#XarArchive-java.lang.String-}
```
public XarArchive(String path)
```


Initialiseert een nieuw exemplaar van de klasse [XarArchive](../../com.aspose.zip/xararchive) en stelt een lijst met items samen die uit het archief kunnen worden gehaald.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (XarArchive archive = new XarArchive(\"archive.xar\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### XarArchive(String path, XarLoadOptions loadOptions) {#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(String path, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Deze constructor pakt geen enkel item uit. Zie de methode [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | de opties om het archief mee te laden |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final XarArchive createEntries(File directory)
```


Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | java.io.File | directory om te comprimeren |
| includeRootDirectory | boolean | geeft aan of de hoofdmap zelf moet worden opgenomen of niet |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final XarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory om te comprimeren |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(xarFile);
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
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory om te comprimeren |
| includeRootDirectory | boolean | geeft aan of de hoofdmap zelf moet worden opgenomen of niet |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | de compressie-instellingen die worden gebruikt voor toegevoegde [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final XarEntry createEntry(String name, File file)
```


Maak een enkel item binnen het archief.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.xar");
     }
 
```

Als het bestand onmiddellijk wordt geopend met de `openImmediately`-parameter, wordt het geblokkeerd totdat het archief wordt vrijgegeven

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| file | java.io.File | de metadata van het bestand of de map die moet worden gecomprimeerd |
| openImmediately | boolean | true als het bestand onmiddellijk wordt geopend, anders wordt het bestand geopend bij het opslaan van het archief. |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Maak een enkel item binnen het archief.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final XarEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.xar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| source | java.io.InputStream | de invoerstroom voor de entry |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)
```


Maak een enkel item binnen het archief.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", new FileInputStream("data.bin"));
archive.save("archive.xar");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final XarEntry createEntry(String name, String sourcePath)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

De naam van het item wordt uitsluitend ingesteld via de `name`‑parameter. De bestandsnaam die wordt opgegeven in de `sourcePath`‑parameter heeft geen invloed op de itemnaam.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| sourcePath | java.lang.String | het pad naar het te comprimeren bestand |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Maak een enkel item binnen het archief.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

De naam van het item wordt uitsluitend ingesteld via de `name`‑parameter. De bestandsnaam die wordt opgegeven in de `sourcePath`‑parameter heeft geen invloed op de itemnaam.

Als het bestand onmiddellijk wordt geopend met de `openImmediately`‑parameter, wordt het geblokkeerd totdat het archief wordt vrijgegeven.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | de naam van het item |
| sourcePath | java.lang.String | het pad naar het te comprimeren bestand |
| openImmediately | boolean | true, als het bestand onmiddellijk moet worden geopend, anders het bestand openen bij het opslaan van het archief |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | de compressie‑instellingen die worden gebruikt voor toegevoegde [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### deleteEntry(XarEntry entry) {#deleteEntry-com.aspose.zip.XarEntry-}
```
public final XarArchive deleteEntry(XarEntry entry)
```


Verwijdert de eerste voorkoming van een specifiek item uit de itemlijst.

Hier ziet u hoe u alle entries behalve de laatste kunt verwijderen:

```

``````

try (XarArchive archive = new XarArchive(\"archive.xar\")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputXarFile.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | the entry to remove from the entries list |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | het pad naar de map waarin de uitgepakte bestanden moeten worden geplaatst. |

Als de map niet bestaat, wordt deze aangemaakt |

### getEntries() {#getEntries--}
```
public final List<XarEntry> getEntries()
```


Haalt items op van het type [XarEntry](../../com.aspose.zip/xarentry) die het archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.XarEntry&gt; - items van het type [XarEntry](../../com.aspose.zip/xarentry) die het archief vormen
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het xar‑archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het xar‑archief vormen
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

Gebruik voor grote archieven [save(String)](../../com.aspose.zip/xararchive\#save-String-) in plaats van opslaan naar java.io.FileOutputStream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | java.io.OutputStream | de bestemmingsstream |

### save(OutputStream output, XarSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-}
```
public final void save(OutputStream output, XarSaveOptions saveOptions)
```


Slaat het archief op in de opgegeven stream.

Gebruik voor grote archieven [save(String)](../../com.aspose.zip/xararchive\#save-String-) in plaats van opslaan naar java.io.FileOutputStream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | java.io.OutputStream | de bestemmingsstream |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | de opties om het xar‑archief op te slaan met |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |

### save(String destinationFileName, XarSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.XarSaveOptions-}
```
public final void save(String destinationFileName, XarSaveOptions saveOptions)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt het overschreven |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | de opties om het xar‑archief op te slaan met |

