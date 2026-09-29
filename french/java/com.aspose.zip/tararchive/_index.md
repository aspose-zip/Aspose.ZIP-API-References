---
title: "TarArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive tar."
type: docs
weight: 125
url: /fr/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive tar. Utilisez‑la pour composer, extraire ou mettre à jour des archives tar.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TarArchive()](#TarArchive--) | Initialise une nouvelle instance de la classe [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [Archive](../../com.aspose.zip/archive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [TarArchive](../../com.aspose.zip/tararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crée une entrée unique dans l'archive. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crée une entrée unique dans l'archive. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Supprime la première occurrence d'une entrée spécifique de la liste d'entrées. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Supprime l'entrée de la liste d'entrées par indice. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Extrait l'archive gzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Extrait l'archive gzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Extrait l'archive LZ4 fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Extrait l'archive LZ4 fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Extrait l'archive LZMA fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Extrait l'archive LZMA fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Extrait l'archive lzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Extrait l'archive lzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Extrait l'archive au format xz fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Extrait l'archive au format xz fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Extrait l'archive au format Z fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Extrait l'archive au format Z fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Extrait l'archive Zstandard fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Extrait l'archive Zstandard fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [TarEntry](../../com.aspose.zip/tarentry) constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive tar. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier de destination fourni. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Enregistre l'archive dans le flux avec compression gzip. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux avec compression gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Enregistre l'archive dans le fichier par chemin avec compression gzip. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier par chemin avec compression gzip. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Enregistre l'archive dans le flux avec compression LZ4. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux avec compression LZ4. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Enregistre l'archive dans le fichier par chemin avec compression LZ4. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier par chemin avec compression LZ4. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Enregistre l'archive dans le flux avec compression LZMA. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux avec compression LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Enregistre l'archive dans le fichier par chemin avec compression lzma. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier par chemin avec compression lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Enregistre l'archive dans le flux avec compression lzip. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux avec compression lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Enregistre l'archive dans le fichier par chemin avec compression lzip. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier par chemin avec compression lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Enregistre l'archive dans le flux avec compression xz. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux avec compression xz. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Enregistre l'archive dans le flux avec compression xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Enregistre l'archive dans le fichier par chemin avec compression xz. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier par chemin avec compression xz. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Enregistre l'archive dans le fichier par chemin avec compression xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Enregistre l'archive dans le flux avec compression Z. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux avec compression Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Enregistre l'archive dans le fichier par chemin avec compression Z. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier par chemin avec compression Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Enregistre l'archive dans le flux avec compression Zstandard. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le flux avec compression Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Enregistre l'archive dans le fichier par chemin avec compression Zstandard. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Enregistre l'archive dans le fichier par chemin avec compression Zstandard. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Initialise une nouvelle instance de la classe [TarArchive](../../com.aspose.zip/tararchive).

L'exemple suivant montre comment compresser un fichier.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) pour le déballage.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Initialise une nouvelle instance de la classe [TarArchive](../../com.aspose.zip/tararchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant montre comment extraire toutes les entrées dans un répertoire.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| répertoire | java.io.File | répertoire à compresser |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | répertoire à compresser |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Ajoute à l'archive tous les fichiers et répertoires de manière récursive dans le répertoire donné.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `file` n'affecte pas le nom de l'entrée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| file | java.io.File | les métadonnées du fichier ou du dossier à compresser |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Crée une entrée unique dans l'archive.

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

Le nom de l'entrée est uniquement défini dans le paramètre `name`.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| source | java.io.InputStream | le flux d'entrée pour l'entrée |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Crée une entrée unique dans l'archive.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

Le nom de l'élément est uniquement défini dans le paramètre `name`. Le nom de fichier fourni dans le paramètre `path` n'affecte pas le nom de l'élément.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String | le nom de l'élément |
| path | java.lang.String | chemin du fichier à compresser |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Crée une entrée unique dans l'archive.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | l'entrée à supprimer de la liste des entrées |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Supprime l'entrée de la liste d'entrées par indice.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Si le répertoire n'existe pas, il sera créé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | le chemin du répertoire où placer les fichiers extraits |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Extrait l'archive gzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important: l'archive gzip est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

Le flux d'extraction GZip n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner sur un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Extrait l'archive gzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important: l'archive gzip est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

Le flux d'extraction GZip n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner sur un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Extrait l'archive LZ4 fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important: l'archive LZ4 est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | source | java.io.InputStream | La source de l’archive. |

Le flux d'extraction LZ4 n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Extrait l'archive LZ4 fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important: l'archive LZ4 est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | path | java.lang.String | Le chemin du fichier d'archive. |

Le flux d'extraction LZ4 n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Extrait l'archive LZMA fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive LZMA est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

Le flux d'extraction LZMA n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Extrait l'archive LZMA fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive LZMA est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

Le flux d'extraction LZMA n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Extrait l'archive lzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive lzip est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

Le flux d'extraction lzip n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Extrait l'archive lzip fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive lzip est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

Le flux d'extraction lzip n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Extrait l'archive au format xz fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive xz est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, elle doit donc fonctionner avec un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Extrait l'archive au format xz fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive xz est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, elle doit donc fonctionner avec un flux positionnable en interne.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Extrait l'archive au format Z fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive Z est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Extrait l'archive au format Z fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive Z est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Extrait l'archive Zstandard fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive Zstandard est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Extrait l'archive Zstandard fournie et compose un [TarArchive](../../com.aspose.zip/tararchive) à partir des données extraites.

Important : l'archive Zstandard est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Obtient les entrées de type [TarEntry](../../com.aspose.zip/tarentry) constituant l'archive.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - entrées de type [TarEntry](../../com.aspose.zip/tarentry) constituant l'archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive tar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive tar
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

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | flux de destination. |

`output` doit être inscriptible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Enregistre l'archive dans le fichier de destination fourni.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

Il est possible d'enregistrer une archive au même emplacement d'où elle a été chargée. Cependant, ce n'est pas recommandé car cette approche utilise une copie vers un fichier temporaire

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Enregistre l'archive dans le flux avec compression gzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | flux de destination. |

`output` doit être inscriptible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Enregistre l'archive dans le fichier par chemin avec compression gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Enregistre l'archive dans le flux avec compression LZ4.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | java.io.OutputStream | Flux de destination. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Enregistre l'archive dans le fichier par chemin avec compression LZ4.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Enregistre l'archive dans le flux avec compression LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Important : l'archive tar est d'abord composée puis compressée dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | flux de destination. |

`output` doit être inscriptible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Enregistre l'archive dans le fichier par chemin avec compression lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Important : l'archive tar est d'abord composée puis compressée dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Enregistre l'archive dans le flux avec compression lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | flux de destination. |

`output` doit être inscriptible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Enregistre l'archive dans le fichier par chemin avec compression lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Enregistre l'archive dans le flux avec compression xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | flux de destination. |

`output`Le flux doit être accessible en écriture |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Enregistre l'archive dans le flux avec compression xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Enregistre l'archive dans le fichier par chemin avec compression xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | ensemble de paramètres spécifiques à l'archive xz : taille du dictionnaire, taille du bloc, type de contrôle |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Enregistre l'archive dans le flux avec compression Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | java.io.OutputStream | le flux de destination |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Enregistre l'archive dans le fichier par chemin avec compression Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Enregistre l'archive dans le flux avec compression Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | sortie | java.io.OutputStream | flux de destination. |

`output` doit être inscriptible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Enregistre l'archive dans le fichier par chemin avec compression Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |
| format | [TarFormat](../../com.aspose.zip/tarformat) | définit le format d'en-tête tar. La valeur null sera traitée comme USTar lorsque possible |

