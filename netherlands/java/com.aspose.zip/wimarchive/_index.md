---
title: "WimArchive"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Deze klasse vertegenwoordigt een wim-archiefbestand."
type: docs
weight: 130
url: /nl/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Deze klasse vertegenwoordigt een wim-archiefbestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Initialiseert een nieuw exemplaar van de [WimArchive](../../com.aspose.zip/wimarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Initialiseert een nieuw exemplaar van de [WimArchive](../../com.aspose.zip/wimarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Initialiseert een nieuw exemplaar van de [WimArchive](../../com.aspose.zip/wimarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Initialiseert een nieuw exemplaar van de [WimArchive](../../com.aspose.zip/wimarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraheert het archief naar het bestand op het opgegeven pad. |
| [getBootImageIndex()](#getBootImageIndex--) | Haalt de (nul-gebaseerde) index van de opstartbare afbeelding op. |
| [getEntries()](#getEntries--) | Haalt items van het type [WimEntry](../../com.aspose.zip/wimentry) op die het archief vormen. |
| [getFileEntries()](#getFileEntries--) | Haalt items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) op die het wim-archief vormen. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Haalt de versie van het bestandsformaat op. |
| [getFormat()](#getFormat--) | Haalt het archiefformaat op. |
| [getGuid()](#getGuid--) | Haalt de identificerende UUID voor het archief op. |
| [getImages()](#getImages--) | Haalt items van het type [WimImage](../../com.aspose.zip/wimimage) op die het archief vormen. |
| [getManifest()](#getManifest--) | Haalt het ingebedde manifest op dat het bestand en de daarin opgenomen afbeeldingen beschrijft. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Initialiseert een nieuw exemplaar van de [WimArchive](../../com.aspose.zip/wimarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream(\"archive.wim\"))) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Deze constructor pakt geen enkel item uit. Zie de methode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | java.io.InputStream | de bron van het archief |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opties om een bestaand archief mee te laden. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Initialiseert een nieuw exemplaar van de [WimArchive](../../com.aspose.zip/wimarchive) klasse en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd.

Het volgende voorbeeld toont hoe alle items naar een map te extraheren.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

Deze constructor pakt geen enkel item uit. Zie de methode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) voor uitpakken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | java.lang.String | het pad naar het archiefbestand |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opties om een bestaand archief mee te laden. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraheert het archief naar het bestand op het opgegeven pad.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | java.lang.String | het pad naar de map waarin de geëxtraheerde bestanden worden geplaatst |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Haalt de (nul-gebaseerde) index van de opstartbare afbeelding op.

**Returns:**
int - de (nul-gebaseerde) index van de opstartbare afbeelding
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Haalt items van het type [WimEntry](../../com.aspose.zip/wimentry) op die het archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - items die het archief vormen
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Haalt items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) op die het wim-archief vormen.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - items van het type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) die het wim-archief vormen
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Haalt de versie van het bestandsformaat op.

**Returns:**
int - de versie van het bestandsformaat
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Haalt het archiefformaat op.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Haalt de identificerende UUID voor het archief op.

**Returns:**
java.util.UUID - de identificerende UUID voor het archief
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Haalt items van het type [WimImage](../../com.aspose.zip/wimimage) op die het archief vormen.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - items van het type [WimImage](../../com.aspose.zip/wimimage) die het archief vormen
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Haalt het ingebedde manifest op dat het bestand en de daarin opgenomen afbeeldingen beschrijft.

**Returns:**
java.lang.String - het ingebedde manifest dat het bestand en de bijbehorende afbeeldingen beschrijft
