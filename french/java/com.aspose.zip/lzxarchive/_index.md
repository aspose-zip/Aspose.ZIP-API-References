---
title: "LzxArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive LZX .lzx."
type: docs
weight: 89
url: /fr/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive LZX (.lzx).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [LzxArchive](../../com.aspose.zip/lzxarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Initialise une nouvelle instance de la classe [LzxArchive](../../com.aspose.zip/lzxarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [LzxArchive](../../com.aspose.zip/lzxarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Initialise une nouvelle instance de la classe [LzxArchive](../../com.aspose.zip/lzxarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers et répertoires de l'archive vers le répertoire fourni. |
| [getEntries()](#getEntries--) | Obtient les entrées de fichiers de type [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Initialise une nouvelle instance de la classe [LzxArchive](../../com.aspose.zip/lzxarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

Ce constructeur ne décompresse aucune entrée. Voir la méthode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extractionSource | java.io.InputStream | La source de l’archive. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [LzxArchive](../../com.aspose.zip/lzxarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

Ce constructeur ne décompresse aucune entrée. Voir la méthode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extractionSource | java.io.InputStream | La source de l’archive. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Options pour charger une archive existante. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Initialise une nouvelle instance de la classe [LzxArchive](../../com.aspose.zip/lzxarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant extrait une archive, puis décompresse la première entrée vers un `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive(\"sample.lzx\")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\\#extract-OutputStream-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin complet ou relatif vers le fichier d’archive. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Options pour charger une archive existante. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait tous les fichiers et répertoires de l'archive vers le répertoire fourni.

```

``````

try (LzxArchive archive = new LzxArchive(\"archive.lzx\")) {
archive.extractToDirectory(\"C:/extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
