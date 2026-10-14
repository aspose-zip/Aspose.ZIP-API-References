---
title: "GzipArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive gzip."
type: docs
weight: 69
url: /fr/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Cette classe représente un fichier d'archive gzip. Utilisez‑la pour créer ou extraire des archives gzip.

L'algorithme de compression Gzip est basé sur l'algorithme DEFLATE, qui est une combinaison de LZ77 et du codage Huffman.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la compression. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la décompression. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la décompression. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la décompression. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la décompression. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive). |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrait l'archive vers le flux fourni. |
| [extract(String path)](#extract-java.lang.String-) | Extrait l'archive vers le fichier indiqué par le chemin. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait le contenu de l'archive vers le répertoire fourni. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive gzip. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
| [getLength()](#getLength--) | Obtient la taille d'un fichier original. |
| [getName()](#getName--) | Le nom du fichier original. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtient la taille d'un fichier original. |
| [open()](#open--) | Ouvre l'archive pour l'extraction et fournit un flux contenant le contenu de l'archive. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Enregistre l'archive dans le flux fourni. |
| [save(String destinationFileName)](#save-java.lang.String-) | Enregistre l'archive dans le fichier de destination fourni. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Définit le contenu à compresser dans l'archive. |
| [setSource(File file)](#setSource-java.io.File-) | Définit le contenu à compresser dans l'archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Définit le contenu à compresser dans l'archive. |
| [setSource(String path)](#setSource-java.lang.String-) | Définit le contenu à compresser dans l'archive. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la compression.

L'exemple suivant montre comment compresser un fichier.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Ce constructeur ne décompresse pas. Voir la méthode [open()](../../com.aspose.zip/gziparchive\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | La source de l’archive. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la décompression.

Ouvrir une archive depuis un flux et l'extraire vers un `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

Ce constructeur ne décompresse pas. Voir la méthode [open()](../../com.aspose.zip/gziparchive\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | La source de l’archive. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options pour charger l'archive. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive) préparée pour la décompression.

Ouvrez une archive depuis un fichier par son chemin et extrayez‑la dans un `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Ce constructeur ne décompresse pas. Voir la méthode [open()](../../com.aspose.zip/gziparchive\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin du fichier d'archive. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Initialise une nouvelle instance de la classe [GzipArchive](../../com.aspose.zip/gziparchive).

Ouvrez une archive depuis un fichier par son chemin et extrayez‑la dans un `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive("archive.gz")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

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

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Flux de destination. Doit être accessible en écriture. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrait l'archive vers le fichier indiqué par le chemin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

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
|  | destinationDirectory | java.lang.String | Le chemin du répertoire où placer les fichiers extraits. |

Si le répertoire n'existe pas, il sera créé. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive gzip.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive gzip.
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


Obtient la taille d'un fichier original.

Lors de la décompression, cette propriété peut contenir une taille incorrecte. Si la taille du fichier décompressé dépasse 4 Go, cette propriété donnera une valeur erronée en raison de la limite de 32 bits dans l'en-tête.

**Returns:**
java.lang.Long - taille d'un fichier original
### getName() {#getName--}
```
public final String getName()
```


Le nom du fichier original.

**Returns:**
java.lang.String - le nom du fichier original
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Obtient la taille d'un fichier original.

Lors de la décompression, cette propriété peut contenir une taille incorrecte. Si la taille du fichier décompressé dépasse 4 Go, cette propriété donnera une valeur erronée en raison de la limite de 32 bits dans l'en-tête.

**Returns:**
long - taille d'un fichier original.
### open() {#open--}
```
public final InputStream open()
```


Ouvre l'archive pour l'extraction et fournit un flux contenant le contenu de l'archive.

Extrait l'archive et copie le contenu extrait vers le flux de fichier.

```

``````

try (GzipArchive archive = new GzipArchive("archive.gz")) {
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | Flux de destination. |

`outputStream` doit être accessible en écriture. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Enregistre l'archive dans le fichier de destination fourni.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Utilisez cette méthode pour composer une archive tar.gz conjointe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Archive tar à compresser. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Définit le contenu à compresser dans l'archive.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | Le flux d'entrée pour l'archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Définit le contenu à compresser dans l'archive.

Ouvrez une archive depuis un fichier par son chemin et extrayez‑la dans un `MemoryStream`

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.gz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

