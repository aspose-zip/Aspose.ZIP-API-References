---
title: "SharArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive shar."
type: docs
weight: 119
url: /fr/java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

Cette classe représente un fichier d'archive shar.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SharArchive()](#SharArchive--) | Initialise une nouvelle instance de la classe [SharArchive](../../com.aspose.zip/shararchive). |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [SharArchive](../../com.aspose.zip/shararchive) préparée pour la décompression. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crée une entrée unique dans l’archive. |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | Supprime la première occurrence d'une entrée spécifique de la liste d'entrées. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Supprime l'entrée de la liste d'entrées par indice. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [SharEntry](../../com.aspose.zip/sharentry) constituant l'archive. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


Initialise une nouvelle instance de la classe [SharArchive](../../com.aspose.zip/shararchive).

L'exemple suivant montre comment compresser un fichier.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.io.File | le répertoire à compresser |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```

``````

try (FileOutputStream sharFile = new FileOutputStream(\"archive.shar\")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | le répertoire à compresser |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```

``````

try (FileOutputStream sharFile = new FileOutputStream(\"archive.shar\")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| file | java.io.File | les métadonnées du fichier ou du dossier à compresser |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


Crée une entrée unique dans l’archive.

```

``````

java.io.File file = new java.io.File("data.bin");
try (SharArchive archive = new SharArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| source | java.io.InputStream | le flux d'entrée pour l'entrée |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


Crée une entrée unique dans l’archive.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
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

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


Supprime la première occurrence d'une entrée spécifique de la liste d'entrées.

Voici comment vous pouvez supprimer toutes les entrées sauf la dernière :

```

``````

try (SharArchive archive = new SharArchive(\"archive.shar\")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save(\"outputSharFile.shar\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entryIndex | int | l'index basé sur zéro de l'entrée à supprimer |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


Obtient les entrées de type [SharEntry](../../com.aspose.zip/sharentry) constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - entrées de type [SharEntry](../../com.aspose.zip/sharentry) constituant l'archive
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Enregistre l'archive dans le flux fourni.

```

``````

try (FileOutputStream sharFile = new FileOutputStream(\"archive.shar\")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |

Il est possible d'enregistrer une archive au même chemin d'où elle a été chargée. Cependant, ce n'est pas recommandé car cette approche utilise une copie vers un fichier temporaire |

