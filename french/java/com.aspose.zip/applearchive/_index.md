---
title: "AppleArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier Apple Archive .aar."
type: docs
weight: 16
url: /fr/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier Apple Archive (.aar). Utilisez‑la pour composer des fichiers Apple Archive.

Apple et Apple Archive sont des marques déposées d'Apple Inc.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) avec les paramètres utilisés pour les entrées composées. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) avec les paramètres utilisés pour les entrées composées. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crée une entrée unique dans l'archive. |
| [dispose()](#dispose--) | Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [getEntries()](#getEntries--) | Obtient les entrées constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Obtient les paramètres utilisés pour les nouvelles entrées composées. |
| [isSolid()](#isSolid--) | Obtient une valeur indiquant si l'archive utilise la compression solide. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) avec les paramètres utilisés pour les entrées composées.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) avec les paramètres utilisés pour les entrées composées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Paramètres utilisés lors de la composition d'une nouvelle Apple Archive. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | La source de l’archive. |

Ce constructeur ne décompresse aucune entrée. Voir les méthodes [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) et [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) pour la décompression. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | La source de l’archive. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Options pour charger une archive existante. |

Ce constructeur ne décompresse aucune entrée. Voir les méthodes [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) et [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) pour la décompression. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | path | java.lang.String | Le chemin complet ou relatif vers le fichier d’archive. |

Ce constructeur ne décompresse aucune entrée. Voir les méthodes [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) et [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) pour la décompression. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [AppleArchive](../../com.aspose.zip/applearchive) et compose une liste d'entrées pouvant être extraites de l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin complet ou relatif vers le fichier d’archive. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Options pour charger une archive existante. |

Ce constructeur ne décompresse aucune entrée. Voir les méthodes [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) et [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) pour la décompression. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.io.File | Répertoire à compresser. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.io.File | Répertoire à compresser. |
| includeRootDirectory | booléen | Indique s'il faut inclure le répertoire racine lui‑-même ou non. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Crée une entrée unique dans l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| fileInfo | java.io.File | Les métadonnées du fichier à compresser. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Crée une entrée unique dans l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| fileInfo | java.io.File | Les métadonnées du fichier à compresser. |
| openImmediately | booléen | Vrai, si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Crée une entrée unique dans l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| source | java.io.InputStream | Le flux d'entrée pour l'élément. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Crée une entrée unique dans l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| path | java.lang.String | Le chemin du fichier à compresser. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Crée une entrée unique dans l'archive.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| path | java.lang.String | Le chemin du fichier à compresser. |
| openImmediately | booléen | Vrai, si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Effectue les tâches définies par l'application associées à la libération, la remise ou la réinitialisation des ressources non gérées.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait tous les fichiers de l'archive vers le répertoire fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Le chemin du répertoire où placer les fichiers extraits. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Obtient les entrées constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - entrées constituant l'archive.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtient le format de l'archive.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Obtient les paramètres utilisés pour les nouvelles entrées composées.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Obtient une valeur indiquant si l'archive utilise la compression solide. En mode solide, toutes les données des entrées sont compressées en un seul flux et l'extraction individuelle des entrées n'est pas disponible. Utilisez [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) à la place.

**Returns:**
boolean - une valeur indiquant si l'archive utilise la compression solide.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Enregistre l'archive dans le flux fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | Flux de destination. |

`output` doit être accessible en écriture. Certains paramètres de compression, comme LZ4, nécessitent également un flux positionnable. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Enregistre l'archive dans le fichier de destination fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | Le chemin de l'archive à créer. |

