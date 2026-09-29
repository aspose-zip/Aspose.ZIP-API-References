---
title: "IsoArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente une archive ISO ISO 9660."
type: docs
weight: 71
url: /fr/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Représente une archive ISO (ISO 9660).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et crée une archive ISO vide pour ajouter de nouveaux fichiers et répertoires. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Ajoute un répertoire à l'image ISO. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Ajoute un fichier à l'image ISO. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Ajoute un fichier à l'image ISO. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Ajoute un fichier à l'image ISO. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait toutes les entrées vers le répertoire spécifié. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [IsoEntry](../../com.aspose.zip/isoentry) constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Enregistre l'image ISO dans le flux spécifié. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Enregistre l'image ISO dans le flux spécifié. |
| [save(String path)](#save-java.lang.String-) | Enregistre l'image ISO dans le chemin spécifié. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Enregistre l'image ISO dans le chemin spécifié. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et crée une archive ISO vide pour ajouter de nouveaux fichiers et répertoires.

L'exemple suivant montre comment créer une nouvelle archive ISO vide et y ajouter des fichiers :

```

``````

// Crée une nouvelle archive ISO vide
try (IsoArchive isoArchive = new IsoArchive()) {
// Ajoute des fichiers à l'archive ISO
isoArchive.createEntry(\"example_file.txt\", \"path_to_file.txt\");
// Enregistre l'archive ISO dans un fichier
isoArchive.save(\"new_archive.iso\");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Ce constructeur ne décompresse aucune entrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant montre comment extraire toutes les entrées dans un répertoire.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream(\"archive.iso\"))) {
archive.extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Ce constructeur ne décompresse aucune entrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [IsoArchive](../../com.aspose.zip/isoarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant montre comment extraire toutes les entrées dans un répertoire.

```

``````

try (IsoArchive archive = new IsoArchive(\"archive.iso\")) {
archive.extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | le répertoire où extraire les entrées |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Obtient les entrées de type [IsoEntry](../../com.aspose.zip/isoentry) constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - entrées de type [IsoEntry](../../com.aspose.zip/isoentry) constituant l'archive iso
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive iso
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Obtient le format de l'archive.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Enregistre l'image ISO dans le flux spécifié.

L'exemple suivant montre comment enregistrer une archive ISO dans un flux mémoire :

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Crée une nouvelle archive ISO vide
try (IsoArchive isoArchive = new IsoArchive()) {
// Ajoute des fichiers à l'archive ISO
isoArchive.createEntry(\"example_file.txt\", \"path_to_file.txt\");
// Enregistre l'archive ISO dans un flux mémoire
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.OutputStream | le flux où l'image ISO sera enregistrée |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | les options pour enregistrer l'archive ISO |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Enregistre l'image ISO dans le chemin spécifié.

L'exemple suivant montre comment enregistrer une archive ISO dans un fichier :

```

``````

// Crée une nouvelle archive ISO vide
try (IsoArchive isoArchive = new IsoArchive()) {
// Ajoute des fichiers à l'archive ISO
isoArchive.createEntry(\"example_file.txt\", \"path_to_file.txt\");
// Enregistre l'archive ISO dans un fichier
isoArchive.save(\"new_archive.iso\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin où l'image ISO sera enregistrée |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | les options pour enregistrer l'archive ISO |

