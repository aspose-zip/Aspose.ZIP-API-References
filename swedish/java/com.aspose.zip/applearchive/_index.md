---
title: "AppleArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en Apple Archive .aar-fil."
type: docs
weight: 16
url: /sv/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Denna klass representerar en Apple Archive (.aar)-fil. Använd den för att skapa Apple Archive-filer.

Apple och Apple Archive är varumärken som tillhör Apple Inc.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) med inställningar som används för sammansatta poster. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) med inställningar som används för sammansatta poster. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Skapar en enskild post i arkivet. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Skapar en enskild post i arkivet. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Skapar en enskild post i arkivet. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Skapar en enskild post i arkivet. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Skapar en enskild post i arkivet. |
| [dispose()](#dispose--) | Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar alla filer i arkivet till den angivna katalogen. |
| [getEntries()](#getEntries--) | Hämtar poster som utgör arkivet. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Hämtar inställningar som används för nyss sammansatta poster. |
| [isSolid()](#isSolid--) | Hämtar ett värde som indikerar om arkivet använder solid kompression. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Sparar arkivet till den angivna strömmen. |
| [save(String destinationFileName)](#save-java.lang.String-) | Sparar arkivet till den angivna destinationsfilen. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) med inställningar som används för sammansatta poster.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) med inställningar som används för sammansatta poster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Inställningar som används när en ny Apple Archive skapas. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | Källan till arkivet. |

Denna konstruktor dekomprimerar inte någon post. Se metoderna [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) och [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) för dekomprimering. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | Källan till arkivet. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

Denna konstruktor dekomprimerar inte någon post. Se metoderna [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) och [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) för dekomprimering. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | path | java.lang.String | Den fullständiga eller relativa sökvägen till arkivfilen. |

Denna konstruktor dekomprimerar inte någon post. Se metoderna [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) och [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) för dekomprimering. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Initierar en ny instans av klassen [AppleArchive](../../com.aspose.zip/applearchive) och skapar en postlista som kan extraheras från arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | Den fullständiga eller relativa sökvägen till arkivfilen. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

Denna konstruktor dekomprimerar inte någon post. Se metoderna [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) och [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) för dekomprimering. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directory | java.io.File | Katalog att komprimera. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directory | java.io.File | Katalog att komprimera. |
| includeRootDirectory | boolean | Anger om rotkatalogen ska inkluderas eller inte. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Skapar en enskild post i arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String | Postens namn. |
| fileInfo | java.io.File | Metadata för filen som ska komprimeras. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Skapar en enskild post i arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String | Postens namn. |
| fileInfo | java.io.File | Metadata för filen som ska komprimeras. |
| openImmediately | boolean | Sant, om filen öppnas omedelbart, annars öppnas filen vid arkivets sparande. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Skapar en enskild post i arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String | Postens namn. |
| source | java.io.InputStream | Inmatningsströmmen för posten. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Skapar en enskild post i arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String | Postens namn. |
| path | java.lang.String | Sökvägen till filen som ska komprimeras. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Skapar en enskild post i arkivet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String | Postens namn. |
| path | java.lang.String | Sökvägen till filen som ska komprimeras. |
| openImmediately | boolean | Sant, om filen öppnas omedelbart, annars öppnas filen vid arkivets sparande. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Utför applikationsdefinierade uppgifter som är kopplade till att frigöra, släppa eller återställa ohanterade resurser.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraherar alla filer i arkivet till den angivna katalogen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Sökvägen till katalogen där de extraherade filerna ska placeras. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Hämtar poster som utgör arkivet.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - poster som utgör arkivet.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör arkivet
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Hämtar arkivformatet.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Hämtar inställningar som används för nyss sammansatta poster.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Hämtar ett värde som indikerar om arkivet använder solid kompression. I solid läge komprimeras all postdata som en enda ström och individuell postextraktion är inte tillgänglig. Använd [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) istället.

**Returns:**
boolean - ett värde som indikerar om arkivet använder solid kompression.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Sparar arkivet till den angivna strömmen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | utdata | java.io.OutputStream | Destinationsström. |

`output` måste vara skrivbar. Vissa komprimeringsinställningar, såsom LZ4, kräver också en sökbar ström. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Sparar arkivet till den angivna destinationsfilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | java.lang.String | Sökvägen till arkivet som ska skapas. |

