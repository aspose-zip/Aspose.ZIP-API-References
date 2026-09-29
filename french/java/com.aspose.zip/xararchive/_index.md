---
title: "XarArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive xar."
type: docs
weight: 136
url: /fr/java/com.aspose.zip/xararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XarArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive xar.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [XarArchive()](#XarArchive--) | Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(XarCompressionSettings defaultCompressionSettings)](#XarArchive-com.aspose.zip.XarCompressionSettings-) | Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(InputStream sourceStream)](#XarArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)](#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-) | Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [XarArchive(String path)](#XarArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [XarArchive(String path, XarLoadOptions loadOptions)](#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-) | Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Crée une entrée unique dans l’archive. |
| [deleteEntry(XarEntry entry)](#deleteEntry-com.aspose.zip.XarEntry-) | Supprime la première occurrence d'une entrée spécifique de la liste d'entrées. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [XarEntry](../../com.aspose.zip/xarentry) constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive xar. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(OutputStream output, XarSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
| [save(String destinationFileName, XarSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.XarSaveOptions-) | Enregistre l'archive dans le fichier de destination fourni. |
### XarArchive() {#XarArchive--}
```
public XarArchive()
```


Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive).

L'exemple suivant montre comment compresser un fichier.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```



### XarArchive(XarCompressionSettings defaultCompressionSettings) {#XarArchive-com.aspose.zip.XarCompressionSettings-}
```
public XarArchive(XarCompressionSettings defaultCompressionSettings)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class.

The following example shows how to compress a file.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultCompressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | les paramètres de compression par défaut, appliqués à toutes les entrées de l'archive |

### XarArchive(InputStream sourceStream) {#XarArchive-java.io.InputStream-}
```
public XarArchive(InputStream sourceStream)
```


Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant montre comment extraire toutes les entrées dans un répertoire.

```

``````

try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
archive.extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### XarArchive(InputStream sourceStream, XarLoadOptions loadOptions) {#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\\#open--) pour le déballage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | les options pour charger l'archive |

### XarArchive(String path) {#XarArchive-java.lang.String-}
```
public XarArchive(String path)
```


Initialise une nouvelle instance de la classe [XarArchive](../../com.aspose.zip/xararchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant montre comment extraire toutes les entrées dans un répertoire.

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
archive.extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### XarArchive(String path, XarLoadOptions loadOptions) {#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(String path, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\\#open--) pour le déballage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | les options pour charger l'archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final XarArchive createEntries(File directory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.io.File | répertoire à compresser |
| includeRootDirectory | booléen | indique s'il faut inclure le répertoire racine lui-même ou non |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final XarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | répertoire à compresser |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | répertoire à compresser |
| includeRootDirectory | booléen | indique s'il faut inclure le répertoire racine lui-même ou non |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | les paramètres de compression utilisés pour les éléments [XarEntry](../../com.aspose.zip/xarentry) ajoutés |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final XarEntry createEntry(String name, File file)
```


Crée une entrée unique dans l’archive.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.xar");
     }
 
```

Si le fichier est ouvert immédiatement avec le paramètre `openImmediately`, il devient bloqué jusqu'à ce que l'archive soit libérée

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| file | java.io.File | les métadonnées du fichier ou du dossier à compresser |
| openImmediately | booléen | true si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive. |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Crée une entrée unique dans l’archive.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.xar");
}
 
```

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final XarEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.xar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| source | java.io.InputStream | le flux d'entrée pour l'entrée |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)
```


Crée une entrée unique dans l’archive.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", new FileInputStream("data.bin"));
archive.save("archive.xar");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final XarEntry createEntry(String name, String sourcePath)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `sourcePath` n'affecte pas le nom de l'entrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| sourcePath | java.lang.String | le chemin du fichier à compresser |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Crée une entrée unique dans l’archive.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `sourcePath` n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec le paramètre `openImmediately`, il devient bloqué jusqu'à ce que l'archive soit libérée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| sourcePath | java.lang.String | le chemin du fichier à compresser |
| openImmediately | booléen | true, si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | les paramètres de compression utilisés pour l'élément [XarEntry](../../com.aspose.zip/xarentry) ajouté |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### deleteEntry(XarEntry entry) {#deleteEntry-com.aspose.zip.XarEntry-}
```
public final XarArchive deleteEntry(XarEntry entry)
```


Supprime la première occurrence d'une entrée spécifique de la liste d'entrées.

Voici comment vous pouvez supprimer toutes les entrées sauf la dernière :

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputXarFile.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | the entry to remove from the entries list |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | le chemin du répertoire où placer les fichiers extraits. |

Si le répertoire n'existe pas, il sera créé |

### getEntries() {#getEntries--}
```
public final List<XarEntry> getEntries()
```


Obtient les entrées de type [XarEntry](../../com.aspose.zip/xarentry) constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.XarEntry&gt; - entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive xar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xar archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtient le format de l'archive.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Enregistre l'archive dans le flux fourni.

Pour les grandes archives, utilisez [save(String)](../../com.aspose.zip/xararchive\#save-String-) au lieu d'enregistrer dans java.io.FileOutputStream.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | java.io.OutputStream | le flux de destination |

### save(OutputStream output, XarSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-}
```
public final void save(OutputStream output, XarSaveOptions saveOptions)
```


Enregistre l'archive dans le flux fourni.

Pour les grandes archives, utilisez [save(String)](../../com.aspose.zip/xararchive\#save-String-) au lieu d'enregistrer dans java.io.FileOutputStream.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | java.io.OutputStream | le flux de destination |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | les options pour enregistrer l'archive xar avec |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Enregistre l'archive dans le fichier de destination fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |

### save(String destinationFileName, XarSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.XarSaveOptions-}
```
public final void save(String destinationFileName, XarSaveOptions saveOptions)
```


Enregistre l'archive dans le fichier de destination fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | les options pour enregistrer l'archive xar avec |

