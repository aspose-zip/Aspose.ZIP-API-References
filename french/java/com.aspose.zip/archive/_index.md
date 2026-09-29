---
title: "Archive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive zip."
type: docs
weight: 26
url: /fr/java/com.aspose.zip/archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class Archive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive zip. Utilisez‑la pour composer, extraire ou mettre à jour des archives zip.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Archive()](#Archive--) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) avec des paramètres optionnels pour ses entrées. |
| [Archive(ArchiveEntrySettings newEntrySettings)](#Archive-com.aspose.zip.ArchiveEntrySettings-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) avec des paramètres optionnels pour ses entrées. |
| [Archive(InputStream sourceStream)](#Archive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [Archive(String path)](#Archive-java.lang.String-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [Archive(String path, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [Archive(String mainSegment, String[] segmentsInOrder)](#Archive-java.lang.String-java.lang.String---) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) à partir d'une archive ZIP multi‑volumes et compose une liste d'entrées pouvant être extraites de l'archive. |
| [Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) à partir d'une archive ZIP multi‑volumes et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Ajoutez à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Ajoutez à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Ajoutez à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Ajoutez à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-) | Crée une entrée unique dans l'archive. |
| [deleteEntry(ArchiveEntry entry)](#deleteEntry-com.aspose.zip.ArchiveEntry-) | Supprime la première occurrence de l'entrée spécifique de la liste d'entrées. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Supprime l'entrée de la liste d'entrées par indice. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [getComment()](#getComment--) | Obtient le commentaire de l'ensemble de l'archive. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [ArchiveEntry](../../com.aspose.zip/archiveentry) constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive (Zip) |
| [getNewEntrySettings()](#getNewEntrySettings--) | Paramètres de compression et de chiffrement utilisés pour les nouveaux éléments [ArchiveEntry](../../com.aspose.zip/archiveentry) ajoutés. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(OutputStream outputStream, ArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
| [save(String destinationFileName, ArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-) | Enregistre l'archive dans le fichier de destination fourni. |
| [saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-) | Enregistre l'archive multi‑volumes dans le répertoire de destination fourni. |
### Archive() {#Archive--}
```
public Archive()
```


Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) avec des paramètres optionnels pour ses entrées.


L'exemple suivant montre comment compresser un seul fichier avec les paramètres par défaut.

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```



### Archive(ArchiveEntrySettings newEntrySettings) {#Archive-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries.


The following example shows how to compress a single file with default settings.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Paramètres de compression et de chiffrement utilisés pour les éléments [ArchiveEntry](../../com.aspose.zip/archiveentry) nouvellement ajoutés. Si aucun n’est spécifié, la compression Deflate la plus courante sans chiffrement sera utilisée. |

### Archive(InputStream sourceStream) {#Archive-java.io.InputStream-}
```
public Archive(InputStream sourceStream)
```


Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive.

L’exemple suivant extrait une archive chiffrée, puis décompresse la première entrée vers un `ByteArrayOutputStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | La source de l’archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options pour charger une archive existante. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive.

L’exemple suivant extrait une archive chiffrée, puis décompresse la première entrée vers un `ByteArrayOutputStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, the most common Deflate compression without encryption would be used. |

### Archive(String path) {#Archive-java.lang.String-}
```
public Archive(String path)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin complet ou relatif vers le fichier d’archive. |

### Archive(String path, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String path, ArchiveLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive.

L’exemple suivant extrait une archive chiffrée, puis décompresse la première entrée vers un `ByteArrayOutputStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
ArchiveLoadOptions options = new ArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (Archive archive = new Archive("encrypted.zip", options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |

### Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example extracts an encrypted archive, then decompresses first entry to a `ByteArrayOutputStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin complet ou relatif vers le fichier d’archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options pour charger une archive existante. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Paramètres de compression et de chiffrement utilisés pour les éléments [ArchiveEntry](../../com.aspose.zip/archiveentry) nouvellement ajoutés. Si aucun n’est spécifié, la compression Deflate la plus courante sans chiffrement sera utilisée. |

### Archive(String mainSegment, String[] segmentsInOrder) {#Archive-java.lang.String-java.lang.String---}
```
public Archive(String mainSegment, String[] segmentsInOrder)
```


Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) à partir d'une archive ZIP multi‑volumes et compose une liste d'entrées pouvant être extraites de l'archive.

```

``````

try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
a.extractToDirectory("destination");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| mainSegment | java.lang.String | Path to the last segment of multi-volume archive with the central directory.

Usually this segment has \*.zip extension and smaller than others. |
| segmentsInOrder | java.lang.String[] | Paths to each segment but the last of multi-volume zip archive respecting order.

Usually they named filename.z01, filename.z02, ..., filename.z(n-1). |

### Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-java.lang.String---com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String mainSegment, String[] segmentsInOrder, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class from multi-volume ZIP archive and composes an entry list can be extracted from the archive.

This sample extract to a directory an archive of three segments.

```

``````

     try (Archive a = new Archive("archive.zip", new String[] { "archive.z01", "archive.z02" })) {
         a.extractToDirectory("destination");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | mainSegment | java.lang.String | Chemin vers le dernier segment d’une archive multi-volumes contenant le répertoire central. |

Habituellement, ce segment a l’extension \*.zip et est plus petit que les autres. |
|  | segmentsInOrder | java.lang.String[] | Chemins vers chaque segment sauf le dernier d’une archive zip multi-volumes, en respectant l’ordre. |

Habituellement, ils sont nommés filename.z01, filename.z02, ..., filename.z(n-1). |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options pour charger une archive existante. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final Archive createEntries(File directory)
```


Ajoutez à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué.

```

``````

try (Archive archive = new Archive()) {
java.io.File folder = new java.io.File("C:\\folder");
archive.createEntries(folder);
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final Archive createEntries(File directory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        java.io.File folder = new java.io.File("C:\\folder");
        archive.createEntries(folder);
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.io.File | Répertoire à compresser. |
| includeRootDirectory | booléen | Indique s'il faut inclure le répertoire racine lui‑-même ou non. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final Archive createEntries(String sourceDirectory)
```


Ajoutez à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire indiqué.

```

``````

try (Archive archive = new Archive()) {
archive.createEntries("C:\\folder");
archive.save("folder.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final Archive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Add to the archive all files and directories recursively in the directory given.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntries("C:\\folder");
        archive.save("folder.zip");
    }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Répertoire à compresser. |
| includeRootDirectory | booléen | Indique s'il faut inclure le répertoire racine lui‑-même ou non. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final ArchiveEntry createEntry(String name, File file)
```


Crée une entrée unique dans l'archive.

Composez une archive avec des entrées chiffrées chacune avec des méthodes de chiffrement et des mots de passe différents.

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Creates a single entry within the archive.

Compose archive with entries encrypted with different encryption methods and passwords each.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `file` n'affecte pas le nom de l'entrée.

Si le fichier est ouvert immédiatement avec le paramètre `openImmediately`, il devient bloqué jusqu'à ce que l'archive soit enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| file | java.io.File | Les métadonnées du fichier à compresser. |
| openImmediately | booléen | Vrai, si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Crée une entrée unique dans l'archive.

Composez une archive avec des entrées chiffrées chacune avec des méthodes de chiffrement et des mots de passe différents.

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
java.io.File fi1 = new java.io.File("data1.bin");
java.io.File fi2 = new java.io.File("data2.bin");
java.io.File fi3 = new java.io.File("data3.bin");
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
archive.save(zipFile);
}
} catch (IOException ignored) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final ArchiveEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.zip");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| source | java.io.InputStream | Le flux d'entrée pour l'élément. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)
```


Crée une entrée unique dans l'archive.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.zip\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {
                    0x00,
                    (byte) 0xFF
            }), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new java.io.File("data1.bin"));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `file` n'affecte pas le nom de l'entrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| source | java.io.InputStream | Le flux d'entrée pour l'élément. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Paramètres de compression et de chiffrement utilisés pour l'élément [ArchiveEntry](../../com.aspose.zip/archiveentry) ajouté. |
| file | java.io.File | Les métadonnées du fichier ou du dossier à compresser. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final ArchiveEntry createEntry(String name, String path)
```


Crée une entrée unique dans l'archive.

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Creates a single entry within the archive.

```

``````

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

Le nom de l'élément est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `path` n'affecte pas le nom de l'élément.

Si le fichier est ouvert immédiatement avec le paramètre `openImmediately`, il devient bloqué jusqu'à ce que l'archive soit enregistrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | Le nom de l'entrée. |
| path | java.lang.String | Le nom complet du nouveau fichier, ou le nom de fichier relatif à compresser. |
| openImmediately | booléen | Vrai, si le fichier est ouvert immédiatement, sinon le fichier est ouvert lors de l'enregistrement de l'archive. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Crée une entrée unique dans l'archive.

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry(\"data.bin\", \"file.dat\");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | boolean | True, if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Creates a single entry within the archive.

Compose archive with encrypted entry.

```

``````

     Supplier<InputStream> provider = new Supplier<InputStream>() {
         public InputStream get() {
             return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
         }
     };
     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
             archive.save(zipFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | la méthode fournissant le flux d'entrée pour l'élément |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, Supplier<InputStream> streamProvider, ArchiveEntrySettings newEntrySettings)
```


Crée une entrée unique dans l'archive.

Composer une archive avec un élément chiffré.

```

``````

Supplier<InputStream> provider = new Supplier<InputStream>() {
public InputStream get() {
return new ByteArrayInputStream(new byte[] {(byte) 0xFF, 0x00});
}
};
try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry1.bin", provider, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
archive.save(zipFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | the method providing input stream for the entry |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - zip entry instance
### deleteEntry(ArchiveEntry entry) {#deleteEntry-com.aspose.zip.ArchiveEntry-}
```
public final Archive deleteEntry(ArchiveEntry entry)
```


Removes the first occurrence of the specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        while (archive.getEntries().size() > 1)
            archive.deleteEntry(archive.getEntries().get(0));
        archive.save("last_entry.zip");
    }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | L'entrée à supprimer de la liste des entrées. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final Archive deleteEntry(int entryIndex)
```


Supprime l'entrée de la liste d'entrées par indice.

```

``````

try (Archive archive = new Archive("two_files.zip")) {
archive.deleteEntry(0);
archive.save("single_file.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | The zero-based index of the entry to remove. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

    try (Archive archive = new Archive("archive.zip")) {
        archive.extractToDirectory("C:\\extracted");
    }
 
```

Si le répertoire n'existe pas, il sera créé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Le chemin du répertoire où placer les fichiers extraits. |

### getComment() {#getComment--}
```
public final String getComment()
```


Obtient le commentaire de l'ensemble de l'archive.

Si `ArchiveLoadOptions.Encoding`([ArchiveLoadOptions.getEncoding](../../com.aspose.zip/archiveloadoptions\#getEncoding)/[ArchiveLoadOptions.setEncoding](../../com.aspose.zip/archiveloadoptions\#setEncoding)) est fourni, il est décodé en l'utilisant. Sinon, UTF-8 est utilisé.

**Returns:**
java.lang.String - commentaire pour l'ensemble de l'archive.
### getEntries() {#getEntries--}
```
public final List<ArchiveEntry> getEntries()
```


Obtient les entrées de type [ArchiveEntry](../../com.aspose.zip/archiveentry) constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArchiveEntry&gt; - entrées de type [ArchiveEntry](../../com.aspose.zip/archiveentry) constituant l'archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtient le format de l'archive (Zip)

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - Zip archive format.
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final ArchiveEntrySettings getNewEntrySettings()
```


Paramètres de compression et de chiffrement utilisés pour les nouveaux éléments [ArchiveEntry](../../com.aspose.zip/archiveentry) ajoutés.

**Returns:**
[ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) - the [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) instance
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Enregistre l'archive dans le flux fourni.

```

``````

try (FileOutputStream zipFile = new FileOutputStream(\"archive.zip\")) {
try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.save(zipFile);
}
} catch (IOException ex) {
}
 
```

`outputStream` must be writable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream. |

### save(OutputStream outputStream, ArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(OutputStream outputStream, ArchiveSaveOptions saveOptions)
```


Saves archive to the stream provided.

```

``````

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry.bin", "data.bin");
            archive.save(zipFile);
        }
    } catch (IOException ex) {
    }
 
```

`outputStream` doit être accessible en écriture.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Flux de destination. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Options pour l'enregistrement de l'archive. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Enregistre l'archive dans le fichier de destination fourni.

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
ArchiveSaveOptions options = new ArchiveSaveOptions();
options.setEncoding(StandardCharsets.US_ASCII);
archive.save("archive.zip", options);
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, ArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(String destinationFileName, ArchiveSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncoding(StandardCharsets.US_ASCII);
        archive.save("archive.zip", options);
    }
 
```

Il est possible d'enregistrer une archive au même emplacement d'où elle a été chargée. Cependant, cette approche utilise la copie vers un fichier temporaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Options pour l'enregistrement de l'archive. |

### saveSplit(String destinationDirectory, SplitArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)
```


Enregistre l'archive multi‑volumes dans le répertoire de destination fourni.

```

``````

try (Archive archive = new Archive()) {
archive.createEntry("entry.bin", "data.bin");
archive.saveSplit( "C:\\Folder", new SplitArchiveSaveOptions("volume", 65536));
}
 
```

This method composes several (n) files filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Cannot make existing archive multi-volume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory where archive segments to be created. |
| options | [SplitArchiveSaveOptions](../../com.aspose.zip/splitarchivesaveoptions) | Options for archive saving, including file name. |

