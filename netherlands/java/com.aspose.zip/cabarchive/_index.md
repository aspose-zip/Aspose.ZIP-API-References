---
title: "CabArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een CAB-archiefbestand."
type: docs
weight: 44
url: /nl/java/com.aspose.zip/cabarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.zip.ICompressionArchive, java.lang.AutoCloseable
```
public class CabArchive implements ICompressionArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een CAB-archiefbestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [CabArchive(CabEntrySettings settings)](#CabArchive-com.aspose.zip.CabEntrySettings-) | Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse, voorbereid op compressie. |
| [CabArchive(InputStream sourceStream)](#CabArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse en stelt een lijst met entries samen die uit het archief kan worden gehaald. |
| [CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)](#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-) | Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse en stelt een lijst met entries samen die uit het archief kan worden gehaald. |
| [CabArchive(String path)](#CabArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse en stelt een lijst met entries samen die uit het archief kan worden gehaald. |
| [CabArchive(String path, CabLoadOptions loadOptions)](#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-) | Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse en stelt een lijst met entries samen die uit het archief kan worden gehaald. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Voegt alle bestanden, recursief, uit de opgegeven map toe aan het archief. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Voegt alle bestanden, recursief, uit de opgegeven map toe aan het archief. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Voegt alle bestanden recursief toe aan het archief vanuit het opgegeven directorypad. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Voegt alle bestanden recursief toe aan het archief vanuit het opgegeven directorypad. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-) | Maak een enkele entry binnen het archief met specifieke instellingen. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, String path, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-) | Maak een enkel item binnen het archief. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Maak een enkel item binnen het archief. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-) | Maak een enkel item binnen het archief. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden in het archief naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt entries van het type [CabEntry](../../com.aspose.zip/cabentry) op die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt entries van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) op die het cab-archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(OutputStream outputStream, CabSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-) | Slaat het archief op in de opgegeven stream met specifieke opties. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
| [save(String destinationFileName, CabSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.CabSaveOptions-) | Slaat het archief op in het opgegeven bestemmingsbestand. |
### CabArchive(CabEntrySettings settings) {#CabArchive-com.aspose.zip.CabEntrySettings-}
```
public CabArchive(CabEntrySettings settings)
```


Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse, voorbereid op compressie.

Comprimeer een bestand met specifieke compressie-instellingen.

```

``````

CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings()));
try (CabArchive archive = new CabArchive(settings))
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | the source of the archive |

### CabArchive(InputStream sourceStream) {#CabArchive-java.io.InputStream-}
```
public CabArchive(InputStream sourceStream)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Deze constructor pakt geen enkele entry uit. Zie [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) methode voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |

### CabArchive(InputStream sourceStream, CabLoadOptions loadOptions) {#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse en stelt een lijst met entries samen die uit het archief kan worden gehaald.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### CabArchive(String path) {#CabArchive-java.lang.String-}
```
public CabArchive(String path)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Deze constructor pakt geen enkele entry uit. Zie [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) methode voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |

### CabArchive(String path, CabLoadOptions loadOptions) {#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(String path, CabLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [CabArchive](../../com.aspose.zip/cabarchive) klasse en stelt een lijst met entries samen die uit het archief kan worden gehaald.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CabArchive createEntries(File directory)
```


Adds to the archive all files, recursively, from the specified directory.

```

``````

 try (var archive = new CabArchive())
 {
     File directory = new File("C:/Logs");
     archive.createEntries(directory);
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | java.io.File | Map om te comprimeren. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CabArchive createEntries(File directory, boolean includeRootDirectory)
```


Voegt alle bestanden, recursief, uit de opgegeven map toe aan het archief.

```

``````

try (var archive = new CabArchive())
{
File directory = new File("C:/Logs");
archive.createEntries(directory, false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CabArchive createEntries(String sourceDirectory)
```


Adds to the archive all files recursively from the specified directory path.

```

``````

 try (var archive = new CabArchive())
 {
     archive.createEntries("C:/Logs");
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Pad van de directory om te comprimeren. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CabArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Voegt alle bestanden recursief toe aan het archief vanuit het opgegeven directorypad.

```

``````

try (var archive = new CabArchive())
{
archive.createEntries("C:/Logs", false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory path to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final CabEntry createEntry(String name, File fileInfo)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     var sourceFile = new java.io.File("logs\\log.txt");
     archive.createEntry("log.txt", sourceFile);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
|  | fileInfo | java.io.File | De metadata van het te comprimeren bestand. |

De entrynaam wordt uitsluitend ingesteld via de `name`-parameter. De bestandsnaam die wordt opgegeven in de `fileInfo`-parameter heeft geen invloed op de entrynaam. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)
```


Maak een enkel item binnen het archief.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
File sourceFile = new File("logs\\log.txt");
archive.createEntry("log.txt", sourceFile, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| fileInfo | java.io.File | The metadata of file to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `fileInfo` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CabEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
 {
     archive.createEntry("stream-entry.bin", stream);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
| source | java.io.InputStream | De invoerstroom voor het item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, InputStream source, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)
```


Maak een enkele entry binnen het archief met specifieke instellingen.

```

``````

try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
{
CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings());
archive.createEntry("stream-entry.bin", stream, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final CabEntry createEntry(String name, String path)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("entry.bin", "data.bin");
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
|  | path | java.lang.String | De volledig gekwalificeerde naam van het nieuwe bestand, of de relatieve bestandsnaam die moet worden gecomprimeerd. |

De naam van het item wordt uitsluitend ingesteld via de `name`-parameter. De bestandsnaam die wordt opgegeven in de `path`-parameter heeft geen invloed op de naam van het item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, String path, CabEntrySettings newEntrySettings)
```


Maak een enkel item binnen het archief.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry("entry.bin", "data.bin", settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("log.txt", () -> new FileInputStream("log.txt"));
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | De methode die een invoerstroom levert voor het item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider, CabEntrySettings newEntrySettings)
```


Maak een enkel item binnen het archief.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry("log.txt", () -> new FileInputStream("log.txt"), settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | het pad naar de map waarin de uitgepakte bestanden moeten worden geplaatst. |

Als de map niet bestaat, wordt deze aangemaakt |

### getEntries() {#getEntries--}
```
public final List<CabEntry> getEntries()
```


Haalt entries van het type [CabEntry](../../com.aspose.zip/cabentry) op die het archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.CabEntry&gt; - items van het type [CabEntry](../../com.aspose.zip/cabentry) die het archief vormen
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt entries van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) op die het cab-archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het cab-archief vormen
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Slaat het archief op in de opgegeven stream.

```

``````

try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream("archive.cab"))
{
archive.createEntry("entry.bin", "data.bin");
archive.save(cabFile);
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream.

`outputStream` must be writable. |

### save(OutputStream outputStream, CabSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-}
```
public final void save(OutputStream outputStream, CabSaveOptions saveOptions)
```


Saves archive to the stream provided with specific options.

```

``````

  try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream("archive.cab"))
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save(cabFile, options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Doelstream. |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | Opties voor het opslaan van het archief. |

`outputStream` moet schrijfbaar zijn. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Slaat het archief op in het opgegeven bestemmingsbestand.

```

``````

try (CabArchive archive = new CabArchive())
{
archive.createEntry("entry.bin", "data.bin");
archive.save("archive.cab");
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### save(String destinationFileName, CabSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.CabSaveOptions-}
```
public final void save(String destinationFileName, CabSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

  try (CabArchive archive = new CabArchive())
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save("archive.cab", options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand wijst, wordt dit overschreven. |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | Opties voor het opslaan van het archief. |

Het is mogelijk om een archief op hetzelfde pad op te slaan als waar het vandaan is geladen. Echter, dit wordt niet aanbevolen omdat deze aanpak kopiëren naar een tijdelijk bestand gebruikt. |

