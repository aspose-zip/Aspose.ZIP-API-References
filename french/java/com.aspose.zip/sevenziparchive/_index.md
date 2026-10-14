---
title: "SevenZipArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive 7z."
type: docs
weight: 104
url: /fr/java/com.aspose.zip/sevenziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class SevenZipArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d’archive 7z. Utilisez‑la pour composer et extraire des archives 7z.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SevenZipArchive()](#SevenZipArchive--) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) avec des paramètres optionnels pour ses entrées. |
| [SevenZipArchive(SevenZipEntrySettings newEntrySettings)](#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) avec des paramètres optionnels pour ses entrées. |
| [SevenZipArchive(InputStream sourceStream)](#SevenZipArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [SevenZipArchive(InputStream sourceStream, String password)](#SevenZipArchive-java.io.InputStream-java.lang.String-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [SevenZipArchive(String path)](#SevenZipArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [SevenZipArchive(String path, String password)](#SevenZipArchive-java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)](#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [SevenZipArchive(String path, SevenZipLoadOptions options)](#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [SevenZipArchive(String[] parts)](#SevenZipArchive-java.lang.String---) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) à partir d’une archive 7z multi‑volumes et compose une liste d’entrées pouvant être extraites de l’archive. |
| [SevenZipArchive(String[] parts, String password)](#SevenZipArchive-java.lang.String---java.lang.String-) | Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) à partir d’une archive 7z multi‑volumes et compose une liste d’entrées pouvant être extraites de l’archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Crée une entrée unique dans l’archive. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-) | Crée une entrée unique dans l’archive. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [extractToDirectory(String destinationDirectory, String password)](#extractToDirectory-java.lang.String-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) constituant l’archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l’archive 7z. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Paramètres de compression et de chiffrement utilisés pour les nouveaux éléments [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) ajoutés. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Enregistre l’archive 7z dans le flux fourni. |
| [save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-) | Enregistre l’archive 7z dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
| [save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-) | Enregistre l'archive dans le fichier de destination fourni. |
| [saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-) | Enregistre l’archive multi‑volumes dans le répertoire de destination fourni. |
### SevenZipArchive() {#SevenZipArchive--}
```
public SevenZipArchive()
```


Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) avec des paramètres optionnels pour ses entrées.

L’exemple suivant montre comment compresser un fichier unique avec les paramètres par défaut : compression LZMA sans chiffrement.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

LZMA compression without encryption would be used.

### SevenZipArchive(SevenZipEntrySettings newEntrySettings) {#SevenZipArchive-com.aspose.zip.SevenZipEntrySettings-}
```
public SevenZipArchive(SevenZipEntrySettings newEntrySettings)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class with optional settings for its entries.

The following example shows how to compress a single file with default settings: LZMA compression without encryption.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | paramètres de compression et de chiffrement utilisés pour les éléments [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) nouvellement ajoutés. Si non spécifié, la compression LZMA sans chiffrement sera utilisée |

### SevenZipArchive(InputStream sourceStream) {#SevenZipArchive-java.io.InputStream-}
```
public SevenZipArchive(InputStream sourceStream)
```


Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
archive.extractToDirectory(\"C:\\\\extracted\");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### SevenZipArchive(InputStream sourceStream, String password) {#SevenZipArchive-java.io.InputStream-java.lang.String-}
```
public SevenZipArchive(InputStream sourceStream, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new FileInputStream("archive.7z"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

Ce constructeur ne décompresse aucun élément. Voir la méthode [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |
| password | java.lang.String | mot de passe optionnel pour le déchiffrement. Si les noms de fichiers sont chiffrés, il doit être présent |

### SevenZipArchive(String path) {#SevenZipArchive-java.lang.String-}
```
public SevenZipArchive(String path)
```


Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory(\"C:\\\\extracted\");
} catch (FileNotFoundException ex) {
}
 
```

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### SevenZipArchive(String path, String password) {#SevenZipArchive-java.lang.String-java.lang.String-}
```
public SevenZipArchive(String path, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (FileNotFoundException ex) {
     }
 
```

Ce constructeur ne décompresse aucun élément. Voir la méthode [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin complet ou relatif vers le fichier d'archive |
| password | java.lang.String | mot de passe optionnel pour le déchiffrement. Si les noms de fichiers sont chiffrés, il doit être présent |

### SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options) {#SevenZipArchive-java.io.InputStream-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(InputStream sourceStream, SevenZipLoadOptions options)
```


Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) et compose une liste d’entrées pouvant être extraites de l’archive.

Extrayez une archive chiffrée. Autorisez jusqu'à 60 secondes pour procéder, annulez après cette période.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
SevenZipLoadOptions options = new SevenZipLoadOptions();
options.setDecryptionPassword("Top$ecr3t");
options.setCancellationFlag(cf);
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
a.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Options to load existing archive with.

This constructor does not decompress any entry. See [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) method for decompressing. |

### SevenZipArchive(String path, SevenZipLoadOptions options) {#SevenZipArchive-java.lang.String-com.aspose.zip.SevenZipLoadOptions-}
```
public SevenZipArchive(String path, SevenZipLoadOptions options)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class and composes an entry list can be extracted from the archive.

Extract an encrypted archive. Allow up to 60 seconds to proceed, cancel after that period.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         SevenZipLoadOptions options = new SevenZipLoadOptions();
         options.setDecryptionPassword("Top$ecr3t");
         options.setCancellationFlag(cf);
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         try (SevenZipArchive a = new SevenZipArchive(new FileInputStream("archive.7z"), options)) {
             a.extractToDirectory("C:\\extracted");
         } catch (IOException ex) {
         }
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin complet ou relatif vers le fichier d’archive. |
|  | options | [SevenZipLoadOptions](../../com.aspose.zip/sevenziploadoptions) | Options pour charger une archive existante. |

Ce constructeur ne décompresse aucun élément. Voir la méthode [extractToDirectory(String, String)](../../com.aspose.zip/sevenziparchive\#extractToDirectory-String--String-) pour la décompression. |

### SevenZipArchive(String[] parts) {#SevenZipArchive-java.lang.String---}
```
public SevenZipArchive(String[] parts)
```


Initialise une nouvelle instance de la classe [SevenZipArchive](../../com.aspose.zip/sevenziparchive) à partir d’une archive 7z multi‑volumes et compose une liste d’entrées pouvant être extraites de l’archive.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
archive.extractToDirectory(\"C:\\\\extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| parts | java.lang.String[] | paths to each segment of multi-volume 7z archive respecting order |

### SevenZipArchive(String[] parts, String password) {#SevenZipArchive-java.lang.String---java.lang.String-}
```
public SevenZipArchive(String[] parts, String password)
```


Initializes a new instance of the [SevenZipArchive](../../com.aspose.zip/sevenziparchive) class from multi-volume 7z archive and composes an entry list can be extracted from the archive.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new String[] { "multi.7z.001", "multi.7z.002", "multi.7z.003" } )) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| parts | java.lang.String[] | chemins vers chaque segment de l'archive 7z multi-volume en respectant l'ordre |
| password | java.lang.String | mot de passe optionnel pour le déchiffrement. Si les noms de fichiers sont chiffrés, il doit être présent |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SevenZipArchive createEntries(File directory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué.

```

``````

try (SevenZipArchive archive = new SevenZipArchive()) {
File folder = new File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SevenZipArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         File folder = new File("C:\\folder");
         archive.createEntries(folder);
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.io.File | répertoire à compresser |
| includeRootDirectory | booléen | indique s'il faut inclure le répertoire racine lui-même ou non |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SevenZipArchive createEntries(String sourceDirectory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué.

Composez une archive 7z avec compression LZMA.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntries("C:\\folder");
archive.save("folder.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SevenZipArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

Compose 7z archive with LZMA compression.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
         archive.createEntries("C:\\folder");
         archive.save("folder.7z");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | répertoire à compresser |
| includeRootDirectory | booléen | indique s'il faut inclure le répertoire racine lui-même ou non |

**Returns:**
[SevenZipArchive](../../com.aspose.zip/sevenziparchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, File file)
```


Crée une entrée unique dans l'archive.

Composer une archive avec des entrées chiffrées chacune avec un mot de passe différent.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different passwords each.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         File fi1 = new File("data1.bin");
         File fi2 = new File("data2.bin");
         File fi3 = new File("data3.bin");

         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
             archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
             archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `file` n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec le paramètre `openImmediately`, il devient bloqué jusqu'à ce que l'archive soit enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| file | java.io.File | les métadonnées du fichier à compresser |
| openImmediately | booléen | true, si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, File file, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


Crée une entrée unique dans l'archive.

Composer une archive avec des entrées chiffrées chacune avec un mot de passe différent.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
File fi1 = new File("data1.bin");
File fi2 = new File("data2.bin");
File fi3 = new File("data3.bin");

try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.createEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
archive.createEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

Compose 7z archive with LZMA compression and encryption of all entries.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.7z");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| source | java.io.InputStream | le flux d'entrée pour l'entrée |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings)
```


Crée une entrée unique dans l'archive.

Composer une archive 7z avec compression LZMA et chiffrement de toutes les entrées.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("p@s$")))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
archive.save("archive.7z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.SevenZipEntrySettings-java.io.File-}
```
public final SevenZipArchiveEntry createEntry(String name, InputStream source, SevenZipEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with LZMA compressed encrypted entry.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive()) {
             archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF}), new SevenZipEntrySettings(new SevenZipLZMACompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new File("data1.bin"));
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `file` n'affecte pas le nom de l'entrée.

`file` peut faire référence à un répertoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| source | java.io.InputStream | le flux d'entrée pour l'entrée |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | paramètres de compression et de chiffrement utilisés pour l'élément [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) ajouté. Les paramètres de compression individuels sont ignorés en cas de compression solide, voir `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\\#setSolid)). |
| file | java.io.File | les métadonnées du fichier ou du dossier à compresser |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final SevenZipArchiveEntry createEntry(String name, String path)
```


Crée une entrée unique dans l'archive.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(sevenZipFile);
         }
     } catch (IOException ex) {
     }
 
```

Le nom de l'élément est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `path` n'affecte pas le nom de l'élément.

Si le fichier est ouvert immédiatement avec le paramètre `openImmediately`, il devient bloqué jusqu'à ce que l'archive soit enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| path | java.lang.String | le nom complet du nouveau fichier, ou le nom de fichier relatif à compresser |
| openImmediately | booléen | true, si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Seven Zip entry instance
### createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, String path, boolean openImmediately, SevenZipEntrySettings newEntrySettings)
```


Crée une entrée unique dans l'archive.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(sevenZipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | the fully qualified name of the new file, or the relative file name to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - Zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

Compose archive with LZMA2 compressed encrypted entry.

```

``````

 System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
 using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
 {
     using (var archive = new SevenZipArchive())
     {
         archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1"))); 
         archive.Save(sevenZipFile);
     }
 }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | La méthode fournissant le flux d'entrée pour l'entrée. |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, SevenZipEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.SevenZipEntrySettings-}
```
public final SevenZipArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, SevenZipEntrySettings newEntrySettings)
```


Crée une entrée unique dans l’archive.

Composer une archive avec une entrée chiffrée compressée LZMA2.

```

``````

System.Func&lt;Stream&gt; provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
using (var archive = new SevenZipArchive())
{
archive.CreateEntry("entry1.bin", provider, new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
archive.Save(sevenZipFile);
}
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) | Compression and encryption settings used for added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) item. Individual compression settings is ignored in case of solid compression, see `SevenZipEntrySettings.Solid`([SevenZipEntrySettings.getSolid](../../com.aspose.zip/sevenzipentrysettings\#getSolid)/[SevenZipEntrySettings.setSolid](../../com.aspose.zip/sevenzipentrysettings\#setSolid)). |

**Returns:**
[SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) - SevenZip entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | le chemin du répertoire où placer les fichiers extraits. |

Si le répertoire n'existe pas, il sera créé |

### extractToDirectory(String destinationDirectory, String password) {#extractToDirectory-java.lang.String-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory, String password)
```


Extrait tous les fichiers de l'archive vers le répertoire fourni.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.extractToDirectory(\"C:\\\\extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |
| password | java.lang.String | optional password for content decryption.

`password` is used for content decryption only. If file names are encrypted provide password in [SevenZipArchive(String, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-String--String-) or [SevenZipArchive(java.io.InputStream, String)](../../com.aspose.zip/sevenziparchive\#SevenZipArchive-java.io.InputStream--String-) constructor. |

### getEntries() {#getEntries--}
```
public final List<SevenZipArchiveEntry> getEntries()
```


Gets entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.SevenZipArchiveEntry&gt; - entries of [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the 7z archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final SevenZipEntrySettings getNewEntrySettings()
```


Compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items.

**Returns:**
[SevenZipEntrySettings](../../com.aspose.zip/sevenzipentrysettings) - compression and encryption settings used for newly added [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) items
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves 7z archive to the stream provided.

```

``````

     try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (SevenZipArchive archive = new SevenZipArchive()) {
                 archive.createEntry("data", source);
                 archive.save(sevenZipFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | java.io.OutputStream | flux de destination |

### save(OutputStream output, SevenZipArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(OutputStream output, SevenZipArchiveSaveOptions saveOptions)
```


Enregistre l’archive 7z dans le flux fourni.

```

``````

try (FileOutputStream sevenZipFile = new FileOutputStream("archive.7z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive()) {
archive.createEntry("data", source);
archive.save(sevenZipFile);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to a destination file provided.

```

``````

  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
     using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
     {
        archive.CreateEntry("data", source);
        archive.Save("archive.7z");
     }
  }
  
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |

Il est possible d'enregistrer une archive au même chemin qu'elle a été chargée. Cependant, ce n'est pas recommandé car cette approche utilise la copie vers un fichier temporaire. |

### save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.SevenZipArchiveSaveOptions-}
```
public final void save(String destinationFileName, SevenZipArchiveSaveOptions saveOptions)
```


Enregistre l'archive dans le fichier de destination fourni.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data", source);
archive.save("archive.7z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | [SevenZipArchiveSaveOptions](../../com.aspose.zip/sevenziparchivesaveoptions) | Options for archive saving.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitSevenZipArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```


Saves multi-volume archive to destination directory provided.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive()) {
         archive.createEntry("entry.bin", "data.bin");
         archive.saveSplit("C:\\Folder", new SplitSevenZipArchiveSaveOptions("volume", 65536));
     }
 
```

Cette méthode compose plusieurs fichiers `(n)` filename.7z.001, filename.7z.002, ..., filename.7z.(n).

Impossible de rendre l'archive existante multi-volume.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | le chemin du répertoire où les segments d'archive seront créés |
| options | [SplitSevenZipArchiveSaveOptions](../../com.aspose.zip/splitsevenziparchivesaveoptions) | options pour l'enregistrement de l'archive, y compris le nom de fichier |

