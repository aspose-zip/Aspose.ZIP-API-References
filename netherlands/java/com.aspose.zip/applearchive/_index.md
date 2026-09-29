---
title: "AppleArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een Apple Archive .aar-bestand."
type: docs
weight: 16
url: /nl/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een Apple Archive (.aar)-bestand. Gebruik deze om Apple Archive-bestanden samen te stellen.

Apple en Apple Archive zijn handelsmerken van Apple Inc.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse met instellingen die worden gebruikt voor samengestelde items. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse met instellingen die worden gebruikt voor samengestelde items. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Voegt alle bestanden en mappen recursief toe aan het archief in de opgegeven map. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Voegt alle bestanden en mappen recursief toe aan het archief in de opgegeven map. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Maakt een enkel item binnen het archief. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Maakt een enkel item binnen het archief. |
| [dispose()](#dispose--) | Voert toepassingsgedefinieerde taken uit die verband houden met het vrijgeven, loslaten of resetten van niet-beheerde bronnen. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert alle bestanden in het archief naar de opgegeven map. |
| [getEntries()](#getEntries--) | Haalt de items op die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Haalt de instellingen op die worden gebruikt voor nieuw samengestelde items. |
| [isSolid()](#isSolid--) | Haalt een waarde op die aangeeft of het archief solide compressie gebruikt. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat het archief op in de opgegeven stream. |
| [save(String destinationFileName)](#save-java.lang.String-) | Slaat het archief op naar een opgegeven doelbestand. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse met instellingen die worden gebruikt voor samengestelde items.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse met instellingen die worden gebruikt voor samengestelde items.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Instellingen die worden gebruikt bij het samenstellen van een nieuw Apple Archive. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | De bron van het archief. |

Deze constructor decompresseert geen enkel item. Zie de methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) en [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) voor decompressie. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | De bron van het archief. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opties om een bestaand archief mee te laden. |

Deze constructor decompresseert geen enkel item. Zie de methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) en [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) voor decompressie. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | path | java.lang.String | Het volledig gekwalificeerde of het relatieve pad naar het archiefbestand. |

Deze constructor decompresseert geen enkel item. Zie de methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) en [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) voor decompressie. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van de [AppleArchive](../../com.aspose.zip/applearchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | Het volledig gekwalificeerde of het relatieve pad naar het archiefbestand. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opties om een bestaand archief mee te laden. |

Deze constructor decompresseert geen enkel item. Zie de methoden [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) en [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) voor decompressie. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Voegt alle bestanden en mappen recursief toe aan het archief in de opgegeven map.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | java.io.File | Map om te comprimeren. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Voegt alle bestanden en mappen recursief toe aan het archief in de opgegeven map.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| directory | java.io.File | Map om te comprimeren. |
| includeRootDirectory | boolean | Geeft aan of de hoofdmap zelf moet worden opgenomen of niet. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Maakt een enkel item binnen het archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
| fileInfo | java.io.File | De metadata van het te comprimeren bestand. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Maakt een enkel item binnen het archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
| fileInfo | java.io.File | De metadata van het te comprimeren bestand. |
| openImmediately | boolean | Waar, als het bestand onmiddellijk wordt geopend, anders wordt het bestand geopend bij het opslaan van het archief. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Maakt een enkel item binnen het archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
| source | java.io.InputStream | De invoerstroom voor het item. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Maakt een enkel item binnen het archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
| path | java.lang.String | Het pad naar het te comprimeren bestand. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Maakt een enkel item binnen het archief.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | De naam van het item. |
| path | java.lang.String | Het pad naar het te comprimeren bestand. |
| openImmediately | boolean | Waar, als het bestand onmiddellijk wordt geopend, anders wordt het bestand geopend bij het opslaan van het archief. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Voert toepassingsgedefinieerde taken uit die verband houden met het vrijgeven, loslaten of resetten van niet-beheerde bronnen.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert alle bestanden in het archief naar de opgegeven map.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Het pad naar de map waarin de uitgepakte bestanden worden geplaatst. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Haalt de items op die het archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - items die het archief vormen.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items op van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het archief vormen
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Haalt de instellingen op die worden gebruikt voor nieuw samengestelde items.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Haalt een waarde op die aangeeft of het archief solide compressie gebruikt. In solid-modus wordt alle itemdata gecomprimeerd als één enkele stroom en is individuele extractie van items niet beschikbaar. Gebruik in plaats daarvan [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) .

**Returns:**
boolean - een waarde die aangeeft of het archief solide compressie gebruikt.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Slaat het archief op in de opgegeven stream.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | Doelstream. |

`output` moet beschrijfbaar zijn. Sommige compressie-instellingen, zoals LZ4, vereisen ook een doorzoekbare stream. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Slaat het archief op naar een opgegeven doelbestand.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationFileName | java.lang.String | Het pad van het te maken archief. |

