---
title: "ArjArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive ARJ."
type: docs
weight: 37
url: /fr/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive ARJ.

Seules les méthodes de compression suivantes sont prises en charge :

| ------ | ------------------------------------------------------------ |
| Méthode | Explication                                                  |
| 0      | Non compressé                                                 |
| 1      | Combinaison de LZ77 et de codage Huffman adaptatif. Meilleur ratio. |
| 2      | Combinaison de LZ77 et de codage Huffman adaptatif.             |
| 3      | Combinaison de LZ77 et de codage Huffman adaptatif. Meilleure vitesse. |
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [ArjArchive](../../com.aspose.zip/arjarchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Initialise une nouvelle instance de la classe [ArjArchive](../../com.aspose.zip/arjarchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [ArjArchive](../../com.aspose.zip/arjarchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Initialise une nouvelle instance de la classe [ArjArchive](../../com.aspose.zip/arjarchive) et compose une liste d’entrées pouvant être extraites de l’archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait toutes les entrées vers le répertoire spécifié. |
| [getCommentary()](#getCommentary--) | Obtient le commentaire. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [ArjEntryPlain](../../com.aspose.zip/arjentryplain) constituant l’archive ARJ. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getName()](#getName--) | Obtient le nom original. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Initialise une nouvelle instance de la classe [ArjArchive](../../com.aspose.zip/arjarchive) et compose une liste d’entrées pouvant être extraites de l’archive.

Ce constructeur ne décompresse aucune entrée. Voir la méthode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) pour décompresser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extractionSource | java.io.InputStream | la source de l'archive |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Initialise une nouvelle instance de la classe [ArjArchive](../../com.aspose.zip/arjarchive) et compose une liste d’entrées pouvant être extraites de l’archive.

Ce constructeur ne décompresse aucune entrée. Voir la méthode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) pour décompresser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| extractionSource | java.io.InputStream | la source de l'archive |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Options pour charger une archive existante. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Initialise une nouvelle instance de la classe [ArjArchive](../../com.aspose.zip/arjarchive) et compose une liste d’entrées pouvant être extraites de l’archive.

L'exemple suivant montre comment extraire toutes les entrées dans un répertoire.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) pour décompresser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Options pour charger une archive existante. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait toutes les entrées vers le répertoire spécifié.

L’exemple suivant montre comment extraire toutes les entrées vers un répertoire :

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
