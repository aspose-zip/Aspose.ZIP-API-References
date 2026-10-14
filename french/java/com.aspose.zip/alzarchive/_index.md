---
title: "AlzArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Représente un fichier d'archive ALZ."
type: docs
weight: 11
url: /fr/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Représente un fichier d'archive ALZ. Utilisez cette classe pour inspecter et extraire les archives ALZ.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Initialise une archive ALZ à partir d'un flux. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Initialise une archive ALZ à partir d'un flux en utilisant les options de chargement fournies. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Initialise une archive ALZ à partir d'un chemin de fichier. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Initialise une archive ALZ à partir d'un chemin de fichier en utilisant les options de chargement fournies. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | Libère les ressources détenues par cette archive. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers et répertoires vers le répertoire fourni. |
| [getEntries()](#getEntries--) | Obtient les entrées constituant cette archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées via l'interface d'archive commune. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Initialise une archive ALZ à partir d'un flux.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Flux d'archive ALZ ; il doit prendre en charge la lecture et le déplacement |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Initialise une archive ALZ à partir d'un flux en utilisant les options de chargement fournies.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| flux | java.io.InputStream | Flux d'archive ALZ ; il doit prendre en charge la lecture et le déplacement |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | options utilisées pour charger l'archive |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Initialise une archive ALZ à partir d'un chemin de fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | chemin vers une archive ALZ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Initialise une archive ALZ à partir d'un chemin de fichier en utilisant les options de chargement fournies.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | chemin vers une archive ALZ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | options utilisées pour charger l'archive |

### close() {#close--}
```
public void close()
```


Libère les ressources détenues par cette archive.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait tous les fichiers et répertoires vers le répertoire fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | répertoire de destination ; il est créé si nécessaire |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Obtient les entrées constituant cette archive.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - liste immuable d'entrées ALZ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées via l'interface d'archive commune.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées d'archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtient le format de l'archive.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
