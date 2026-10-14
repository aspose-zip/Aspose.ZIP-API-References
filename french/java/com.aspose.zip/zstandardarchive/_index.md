---
title: "ZstandardArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive Zstandard."
type: docs
weight: 156
url: /fr/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive Zstandard. Utilisez‑la pour composer des archives Zstandard.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) préparée pour la compression. |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) préparée pour la décompression. |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) préparée pour la décompression. |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'archive vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'archive vers le fichier indiqué par le chemin. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait le contenu de l'archive vers le répertoire fourni. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive zstandard. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getLength()](#getLength--) | Obtient la longueur de l'entrée en octets. |
| [getName()](#getName--) | Obtient le nom de l'entrée dans l'archive. |
| [open()](#open--) | Ouvre l'archive pour l'extraction et fournit un flux contenant le contenu de l'archive. |
| [save(File destination)](#save-java.io.File-) | Enregistre l'archive dans le fichier de destination fourni. |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | Enregistre l'archive dans le fichier de destination fourni. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | Enregistre l'archive dans le fichier de destination fourni. |
| [setSource(File file)](#setSource-java.io.File-) | Définit le contenu à compresser dans l'archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Définit le contenu à compresser dans l'archive. |
| [setSource(String path)](#setSource-java.lang.String-) | Définit le contenu à compresser dans l'archive. |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) préparée pour la compression.

L'exemple suivant montre comment compresser un fichier.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(\"data.bin\");
archive.save(\"archive.zst\");
}
 
```



### ZstandardArchive(InputStream sourceStream) {#ZstandardArchive-java.io.InputStream-}
```
public ZstandardArchive(InputStream sourceStream)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Ce constructeur ne décompresse pas. Voir la méthode [open()](../../com.aspose.zip/zstandardarchive\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) préparée pour la décompression.

Ouvrir une archive depuis un flux et l'extraire vers un `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### ZstandardArchive(String path) {#ZstandardArchive-java.lang.String-}
```
public ZstandardArchive(String path)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class.

Open an archive from file by path and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Ce constructeur ne décompresse pas. Voir la méthode [open()](../../com.aspose.zip/zstandardarchive\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier d'archive |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


Initialise une nouvelle instance de la classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive).

Ouvrir une archive depuis un fichier par chemin et l'extraire vers un `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux de destination. Doit être accessible en écriture |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrait l'archive vers le fichier indiqué par le chemin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

**Returns:**
java.io.File - les informations du fichier extrait
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait le contenu de l'archive vers le répertoire fourni.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | le chemin du répertoire où placer les fichiers extraits. |

Si le répertoire n'existe pas, il sera créé |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive zstandard.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées du type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive zstandard
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtient le format de l'archive.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtient la longueur de l'entrée en octets.

**Returns:**
java.lang.Long - la longueur de l'entrée en octets
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom de l'entrée dans l'archive.

**Returns:**
java.lang.String - le nom de l'entrée dans l'archive
### open() {#open--}
```
public final InputStream open()
```


Ouvre l'archive pour l'extraction et fournit un flux contenant le contenu de l'archive.

Extrait l'archive et copie le contenu extrait vers le flux de fichier.

```

``````

try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.zst"));
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.File | le fichier qui sera ouvert en tant que flux de destination |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


Enregistre l'archive dans le fichier de destination fourni.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File("archive.zst"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | le flux de destination |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


Enregistre l'archive dans le flux fourni.

Écrire des données compressées vers le flux de réponse http.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | the destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.zst");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


Enregistre l'archive dans le fichier de destination fourni.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("result.zst");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| file | java.io.File | la référence à un fichier à compresser |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Définit le contenu à compresser dans l'archive.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.zst\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | chemin du fichier à compresser |

