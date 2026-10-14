---
title: "XzArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive xz."
type: docs
weight: 146
url: /fr/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive xz. Utilisez‑la pour composer et extraire des archives xz.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [XzArchive()](#XzArchive--) | Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) et compose l'archive au format xz. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) et compose l'archive au format xz. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extract(File file)](#extract-java.io.File-) | Extrait l'archive xz vers un fichier. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'archive xz vers un flux. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'archive xz vers un fichier par chemin. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait le contenu de l'archive vers le répertoire fourni. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive xz. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille non compressée des données du fichier en octets. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Enregistre l'archive xz dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive xz dans le fichier de destination fourni. |
| [setSource(File file)](#setSource-java.io.File-) | Définit le contenu à compresser dans l'archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Définit le contenu à compresser dans l'archive. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Définit le contenu à compresser dans l'archive. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) et compose l'archive au format xz.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) et compose l'archive au format xz.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | ensemble de paramètres spécifiques à l'archive xz : taille du dictionnaire, taille du bloc, type de contrôle |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression.

Ce constructeur ne décompresse pas. Voir la méthode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression.

Ce constructeur ne décompresse pas. Voir la méthode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | la source de l'archive |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Options pour charger l'archive. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression.

Ce constructeur ne décompresse pas. Voir la méthode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | chemin vers la source de l'archive |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Initialise une nouvelle instance de la classe [XzArchive](../../com.aspose.zip/xzarchive) préparée pour la décompression.

Ce constructeur ne décompresse pas. Voir la méthode [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | chemin vers la source de l'archive |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrait l'archive xz vers un fichier.

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

``````

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux pour stocker les données décompressées |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrait l'archive xz vers un fichier par chemin.

```

``````

try (FileInputStream xzFile = new FileInputStream(\"sourceFileName\")) {
try (XzArchive archive = new XzArchive(xzFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves xz archive to the stream provided.

```

``````

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | java.io.OutputStream | flux de destination |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Enregistre l'archive xz dans le fichier de destination fourni.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.xz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| file | java.io.File | fichier, qui sera ouvert en tant que flux d'entrée |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Définit le contenu à compresser dans l'archive.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save(\"archive.xz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | chemin vers le fichier qui sera ouvert en tant que flux d'entrée |

