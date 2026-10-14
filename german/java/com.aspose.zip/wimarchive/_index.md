---
title: "WimArchive"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Diese Klasse repräsentiert eine Wim-Archivdatei."
type: docs
weight: 130
url: /de/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Diese Klasse repräsentiert eine Wim-Archivdatei.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Initialisiert eine neue Instanz der [WimArchive](../../com.aspose.zip/wimarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Initialisiert eine neue Instanz der [WimArchive](../../com.aspose.zip/wimarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Initialisiert eine neue Instanz der [WimArchive](../../com.aspose.zip/wimarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Initialisiert eine neue Instanz der [WimArchive](../../com.aspose.zip/wimarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrahiert das Archiv in die Datei anhand des Pfads. |
| [getBootImageIndex()](#getBootImageIndex--) | Liefert den (nullbasierten) Index des bootfähigen Images. |
| [getEntries()](#getEntries--) | Liefert Einträge vom Typ [WimEntry](../../com.aspose.zip/wimentry), die das Archiv bilden. |
| [getFileEntries()](#getFileEntries--) | Liefert Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das Wim-Archiv bilden. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Liefert die Version des Dateiformats. |
| [getFormat()](#getFormat--) | Liefert das Archivformat. |
| [getGuid()](#getGuid--) | Liefert die identifizierende UUID für das Archiv. |
| [getImages()](#getImages--) | Liefert Einträge vom Typ [WimImage](../../com.aspose.zip/wimimage), die das Archiv bilden. |
| [getManifest()](#getManifest--) | Liefert das eingebettete Manifest, das die Datei und die enthaltenen Images beschreibt. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Initialisiert eine neue Instanz der [WimArchive](../../com.aspose.zip/wimarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden können.

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

Dieser Konstruktor entpackt keinen Eintrag. Siehe die Methode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) zum Entpacken.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sourceStream | java.io.InputStream | die Quelle des Archivs |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Initialisiert eine neue Instanz der [WimArchive](../../com.aspose.zip/wimarchive)-Klasse und erstellt eine Eintragsliste, die aus dem Archiv extrahiert werden kann.

Das folgende Beispiel zeigt, wie alle Einträge in ein Verzeichnis extrahiert werden können.

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

Dieser Konstruktor entpackt keinen Eintrag. Siehe die Methode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) zum Entpacken.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | java.lang.String | der Pfad zur Archivdatei |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Optionen zum Laden eines bestehenden Archivs. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrahiert das Archiv in die Datei anhand des Pfads.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Der Pfad zu dem Verzeichnis, in dem die extrahierten Dateien abgelegt werden sollen |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Liefert den (nullbasierten) Index des bootfähigen Images.

**Returns:**
int – der (nullbasierte) Index des bootfähigen Images
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Liefert Einträge vom Typ [WimEntry](../../com.aspose.zip/wimentry), die das Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; – Einträge, die das Archiv bilden
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Liefert Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das Wim-Archiv bilden.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; – Einträge vom Typ [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), die das Wim-Archiv bilden
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Liefert die Version des Dateiformats.

**Returns:**
int – die Version des Dateiformats
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Liefert das Archivformat.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Liefert die identifizierende UUID für das Archiv.

**Returns:**
java.util.UUID - die identifizierende UUID für das Archiv
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Liefert Einträge vom Typ [WimImage](../../com.aspose.zip/wimimage), die das Archiv bilden.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - Einträge vom Typ [WimImage](../../com.aspose.zip/wimimage), die das Archiv bilden
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Liefert das eingebettete Manifest, das die Datei und die enthaltenen Images beschreibt.

**Returns:**
java.lang.String - das eingebettete Manifest, das die Datei und die enthaltenen Bilder beschreibt
