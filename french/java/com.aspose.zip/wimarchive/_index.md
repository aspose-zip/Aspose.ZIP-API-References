---
title: "WimArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive wim."
type: docs
weight: 130
url: /fr/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive wim.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [WimArchive](../../com.aspose.zip/wimarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Initialise une nouvelle instance de la classe [WimArchive](../../com.aspose.zip/wimarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [WimArchive](../../com.aspose.zip/wimarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Initialise une nouvelle instance de la classe [WimArchive](../../com.aspose.zip/wimarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait l'archive vers le fichier indiqué par le chemin. |
| [getBootImageIndex()](#getBootImageIndex--) | Obtient l'index (à partir de zéro) de l'image amorçable. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [WimEntry](../../com.aspose.zip/wimentry) constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive wim. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Obtient la version du format de fichier. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getGuid()](#getGuid--) | Obtient l'UUID d'identification de l'archive. |
| [getImages()](#getImages--) | Obtient les entrées de type [WimImage](../../com.aspose.zip/wimimage) constituant l'archive. |
| [getManifest()](#getManifest--) | Obtient le manifeste intégré décrivant le fichier et les images contenues. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Initialise une nouvelle instance de la classe [WimArchive](../../com.aspose.zip/wimarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant montre comment extraire toutes les entrées vers un répertoire.

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

Ce constructeur ne décompresse aucune entrée. Voir la méthode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) pour le déballage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Options pour charger une archive existante. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Initialise une nouvelle instance de la classe [WimArchive](../../com.aspose.zip/wimarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant montre comment extraire toutes les entrées vers un répertoire.

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

Ce constructeur ne décompresse aucune entrée. Voir la méthode [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) pour le déballage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Options pour charger une archive existante. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait l'archive vers le fichier indiqué par le chemin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | le chemin du répertoire où placer les fichiers extraits |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Obtient l'index (à partir de zéro) de l'image amorçable.

**Returns:**
int - l'index (à partir de zéro) de l'image amorçable
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Obtient les entrées de type [WimEntry](../../com.aspose.zip/wimentry) constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - entrées constituant l'archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive wim.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive wim
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Obtient la version du format de fichier.

**Returns:**
int - la version du format de fichier
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtient le format de l'archive.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Obtient l'UUID d'identification de l'archive.

**Returns:**
java.util.UUID - l'UUID d'identification de l'archive
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Obtient les entrées de type [WimImage](../../com.aspose.zip/wimimage) constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - entrées de type [WimImage](../../com.aspose.zip/wimimage) constituant l'archive
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Obtient le manifeste intégré décrivant le fichier et les images contenues.

**Returns:**
java.lang.String - le manifeste intégré décrivant le fichier et les images contenues
