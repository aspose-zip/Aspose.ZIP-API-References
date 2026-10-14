---
title: "LhaArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive LHA .lzh."
type: docs
weight: 75
url: /fr/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive LHA (.lzh).

Seules les méthodes de compression suivantes sont prises en charge :

| ------ | --------------------------------------------- |
| Méthode | Explication                                   |
| lh0    | Non compressé                                  |
| lh4    | Dictionnaire glissant de 8 Ko et Huffman statique   |
| lh5    | Dictionnaire glissant de 16 Ko et Huffman statique  |
| lh6    | Dictionnaire glissant de 64 Ko et Huffman statique  |
| lh7    | Dictionnaire glissant de 128 Ko et Huffman statique |
| lhx    | Dictionnaire glissant de 1 Mio et Huffman statique   |
| lhd    | Répertoire                                     |
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [LhaArchive](../../com.aspose.zip/lhaarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Initialise une nouvelle instance de la classe [LhaArchive](../../com.aspose.zip/lhaarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [LhaArchive](../../com.aspose.zip/lhaarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Initialise une nouvelle instance de la classe [LhaArchive](../../com.aspose.zip/lhaarchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers et répertoires de l'archive vers le répertoire fourni. |
| [getEntries()](#getEntries--) | Obtient les entrées de fichiers du type [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) constituant l'archive. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Initialise une nouvelle instance de la classe [LhaArchive](../../com.aspose.zip/lhaarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

Ce constructeur ne décompresse aucune entrée. Voir la méthode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [LhaArchive](../../com.aspose.zip/lhaarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

Ce constructeur ne décompresse aucune entrée. Voir la méthode [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Options pour charger une archive existante. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Initialise une nouvelle instance de la classe [LhaArchive](../../com.aspose.zip/lhaarchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant extrait une archive, puis décompresse la première entrée vers un `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\\#extract-OutputStream-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin complet ou relatif vers le fichier d'archive |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Options pour charger une archive existante. |

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

try (LhaArchive archive = new LhaArchive(\"archive.lzh\")) {
archive.extractToDirectory(\"C:/extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
