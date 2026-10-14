---
title: "SnappyArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio snappy."
type: docs
weight: 121
url: /it/java/com.aspose.zip/snappyarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class SnappyArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Questa classe rappresenta un file di archivio snappy. Usala per creare o estrarre archivi snappy.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SnappyArchive()](#SnappyArchive--) | Inizializza una nuova istanza della classe [SnappyArchive](../../com.aspose.zip/snappyarchive) preparata per la compressione. |
| [SnappyArchive(InputStream source)](#SnappyArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [SnappyArchive](../../com.aspose.zip/snappyarchive) preparata per la decompressione. |
| [SnappyArchive(String path)](#SnappyArchive-java.lang.String-) | Inizializza una nuova istanza della classe [SnappyArchive](../../com.aspose.zip/snappyarchive) preparata per la decompressione. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Estrae l'archivio snappy in un file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae l'archivio snappy in uno stream. |
| [extract(String path)](#extract-java.lang.String-) | Estrae l'archivio snappy in un file tramite percorso. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae il contenuto dell'archivio nella directory fornita. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio snappy. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getLength()](#getLength--) | Ottiene la lunghezza. |
| [getName()](#getName--) | Il nome del file originale. |
| [save(File destination)](#save-java.io.File-) | Salva l'archivio snappy nel file di destinazione fornito. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Salva l'archivio snappy nello stream fornito. |
| [save(String destinationFileName)](#save-java.lang.String-) | Salva l'archivio snappy nel file di destinazione fornito. |
| [setSource(File file)](#setSource-java.io.File-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
### SnappyArchive() {#SnappyArchive--}
```
public SnappyArchive()
```


Inizializza una nuova istanza della classe [SnappyArchive](../../com.aspose.zip/snappyarchive) preparata per la compressione.

Il seguente esempio mostra come comprimere un file.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



### SnappyArchive(InputStream source) {#SnappyArchive-java.io.InputStream-}
```
public SnappyArchive(InputStream source)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The source of the archive. |

### SnappyArchive(String path) {#SnappyArchive-java.lang.String-}
```
public SnappyArchive(String path)
```


Initializes a new instance of the [SnappyArchive](../../com.aspose.zip/snappyarchive) class prepared for decompressing.

```

``````

      try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
          try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
              try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                  archive.extract(extractedFile);
              }
          }
      } catch (IOException ex) {
      }
 
```

Questo costruttore non decomprime. Vedi il metodo [extract(java.io.OutputStream)](../../com.aspose.zip/snappyarchive\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso alla sorgente dell'archivio |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Estrae l'archivio snappy in un file.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts snappy archive to a stream.

```

``````

     try (FileInputStream sourceSnappyFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (SnappyArchive archive = new SnappyArchive(sourceSnappyFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | lo stream per memorizzare i dati decompressi |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae l'archivio snappy in un file tramite percorso.

```

``````

try (FileInputStream snappyFile = new FileInputStream("sourceFileName")) {
try (SnappyArchive archive = new SnappyArchive(snappyFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

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

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the snappy archive
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


Gets length.

**Returns:**
java.lang.Long - length.
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.snappy"));
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.File | il file, che sarà aperto come stream di destinazione |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Salva l'archivio snappy nello stream fornito.

```

``````

try (FileOutputStream snappyFile = new FileOutputStream("archive.snappy")) {
try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save(snappyFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves snappy archive to the destination file provided.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.snappy");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Imposta il contenuto da comprimere all'interno dell'archivio.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as an input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (SnappyArchive archive = new SnappyArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.snappy");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | lo stream di input per l'archivio |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Imposta il contenuto da comprimere all'interno dell'archivio.

```

``````

try (SnappyArchive archive = new SnappyArchive()) {
archive.setSource("data.bin");
archive.save("archive.snappy");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | the path to the file which will be opened as an input stream |

