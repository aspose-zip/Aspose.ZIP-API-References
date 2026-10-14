---
title: "UueArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier uuencoded."
type: docs
weight: 128
url: /fr/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Cette classe représente un fichier uuencoded.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [UueArchive()](#UueArchive--) | Initialise une nouvelle instance de la classe [UueArchive](../../com.aspose.zip/uuearchive) préparée pour l’encodage. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [UueArchive](../../com.aspose.zip/uuearchive) préparée pour le décodage. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [UueArchive](../../com.aspose.zip/uuearchive). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'archive vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'archive vers le fichier indiqué par le chemin. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait le contenu de l'archive vers le répertoire fourni. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l’archive uue. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getLength()](#getLength--) | Obtient la longueur. |
| [getName()](#getName--) | Nom du fichier original. |
| [open()](#open--) | Ouvre l’archive pour le décodage et fournit un flux contenant le contenu de l’archive. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l’archive dans le fichier de destination fourni. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | Enregistre l’archive dans le fichier de destination fourni. |
| [setSource(File file)](#setSource-java.io.File-) | Définit le contenu à compresser dans l'archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Définit le contenu à encoder dans l’archive. |
| [setSource(String path)](#setSource-java.lang.String-) | Définit le contenu à encoder dans l’archive. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


Initialise une nouvelle instance de la classe [UueArchive](../../com.aspose.zip/uuearchive) préparée pour l’encodage.

L’exemple suivant montre comment uuencoder un fichier.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.uue");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Ce constructeur ne décode pas. Voir la méthode [open()](../../com.aspose.zip/uuearchive\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la source de l'archive |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


Initialise une nouvelle instance de la classe [UueArchive](../../com.aspose.zip/uuearchive).

Ouvrez une archive depuis un fichier par son chemin et décodez‑la dans un `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream("archive.uue"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

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

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | flux de destination |

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
java.io.File - informations du fichier extrait
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


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l’archive uue.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l’archive uue
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


Obtient la longueur.

**Returns:**
java.lang.Long - longueur
### getName() {#getName--}
```
public final String getName()
```


Nom du fichier original.

**Returns:**
java.lang.String - le nom du fichier original
### open() {#open--}
```
public final InputStream open()
```


Ouvre l’archive pour le décodage et fournit un flux contenant le contenu de l’archive.

Utilisation :

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | flux de destination |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


Enregistre l'archive dans le flux fourni.

Écrire des données compressées vers le flux de réponse http.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


Enregistre l’archive dans le fichier de destination fourni.

Écrire les données encodées dans le fichier.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
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


Définit le contenu à encoder dans l’archive.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.uue");
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


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | chemin du fichier à encoder |

