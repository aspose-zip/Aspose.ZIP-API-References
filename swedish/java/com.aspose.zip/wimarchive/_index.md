---
title: "WimArchive"
second_title: "Aspose.ZIP för Java API-referens"
description: "Denna klass representerar en wim-arkivfil."
type: docs
weight: 130
url: /sv/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Denna klass representerar en wim-arkivfil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Initialiserar en ny instans av klassen [WimArchive](../../com.aspose.zip/wimarchive) och skapar en postlista som kan extraheras från arkivet. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Initialiserar en ny instans av klassen [WimArchive](../../com.aspose.zip/wimarchive) och skapar en postlista som kan extraheras från arkivet. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Initialiserar en ny instans av klassen [WimArchive](../../com.aspose.zip/wimarchive) och skapar en postlista som kan extraheras från arkivet. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Initialiserar en ny instans av klassen [WimArchive](../../com.aspose.zip/wimarchive) och skapar en postlista som kan extraheras från arkivet. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extraherar arkivet till filen enligt sökväg. |
| [getBootImageIndex()](#getBootImageIndex--) | Hämtar det (nollbaserade) indexet för den startbara avbilden. |
| [getEntries()](#getEntries--) | Hämtar poster av typen [WimEntry](../../com.aspose.zip/wimentry) som utgör arkivet. |
| [getFileEntries()](#getFileEntries--) | Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör wim‑arkivet. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Hämtar versionen av filformatet. |
| [getFormat()](#getFormat--) | Hämtar arkivformatet. |
| [getGuid()](#getGuid--) | Hämtar det identifierande UUID‑et för arkivet. |
| [getImages()](#getImages--) | Hämtar poster av typen [WimImage](../../com.aspose.zip/wimimage) som utgör arkivet. |
| [getManifest()](#getManifest--) | Hämtar den inbäddade manifestfilen som beskriver filen och de innehållna avbilderna. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Initialiserar en ny instans av klassen [WimArchive](../../com.aspose.zip/wimarchive) och skapar en postlista som kan extraheras från arkivet.

Följande exempel visar hur man extraherar alla poster till en katalog.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
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

Den här konstruktorn packar inte upp någon post. Se metoden [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) för uppackning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceStream | java.io.InputStream | källan till arkivet |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Initialiserar en ny instans av klassen [WimArchive](../../com.aspose.zip/wimarchive) och skapar en postlista som kan extraheras från arkivet.

Följande exempel visar hur man extraherar alla poster till en katalog.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
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

Den här konstruktorn packar inte upp någon post. Se metoden [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) för uppackning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | java.lang.String | sökvägen till arkivfilen |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Alternativ för att läsa in befintligt arkiv med. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extraherar arkivet till filen enligt sökväg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationDirectory | java.lang.String | sökvägen till katalogen där de extraherade filerna ska placeras |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Hämtar det (nollbaserade) indexet för den startbara avbilden.

**Returns:**
int – det (nollbaserade) indexet för den startbara avbilden
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Hämtar poster av typen [WimEntry](../../com.aspose.zip/wimentry) som utgör arkivet.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; – poster som utgör arkivet
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Hämtar poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör wim‑arkivet.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; – poster av typen [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) som utgör wim‑arkivet
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Hämtar versionen av filformatet.

**Returns:**
int – versionen av filformatet
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Hämtar arkivformatet.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Hämtar det identifierande UUID‑et för arkivet.

**Returns:**
java.util.UUID - den identifierande UUID:n för arkivet
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Hämtar poster av typen [WimImage](../../com.aspose.zip/wimimage) som utgör arkivet.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - poster av typen [WimImage](../../com.aspose.zip/wimimage) som utgör arkivet
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Hämtar den inbäddade manifestfilen som beskriver filen och de innehållna avbilderna.

**Returns:**
java.lang.String - den inbäddade manifestfilen som beskriver filen och de innehållna bilderna
