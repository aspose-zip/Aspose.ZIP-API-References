---
title: "LzmaArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio LZMA."
type: docs
weight: 86
url: /it/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Questa classe rappresenta un file di archivio LZMA. Usala per creare o estrarre archivi LZMA.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) e compone l'archivio in formato lzma. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) e compone l'archivio in formato lzma. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparata per la decompressione. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparata per la decompressione. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Estrae l'archivio lzma in un file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae l'archivio lzma in uno stream. |
| [extract(String path)](#extract-java.lang.String-) | Estrae l'archivio lzma in un file tramite percorso. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae il contenuto dell'archivio nella directory fornita. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio lzma. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getLength()](#getLength--) | Ottiene la lunghezza. |
| [getName()](#getName--) | Il nome del file originale. |
| [save(File destination)](#save-java.io.File-) | Salva l'archivio lzma nel file di destinazione fornito. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Salva l'archivio lzma nello stream fornito. |
| [save(String destinationFileName)](#save-java.lang.String-) | Salva l'archivio lzma nel file di destinazione fornito. |
| [setSource(File file)](#setSource-java.io.File-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) e compone l'archivio in formato lzma.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) e compone l'archivio in formato lzma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | insieme di impostazioni per un archivio lzma specifico |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Inizializza una nuova istanza della classe [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparata per la decompressione.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.io.File | il file per memorizzare i dati decompressi |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae l'archivio lzma in uno stream.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file che conterrà i dati decompressi |

**Returns:**
java.io.File - le informazioni del file estratto.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae il contenuto dell'archivio nella directory fornita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | il percorso della directory in cui posizionare i file estratti. |

Se la directory non esiste, verrà creata |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio lzma.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio lzma.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Ottiene il formato dell'archivio.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Ottiene la lunghezza.

**Returns:**
java.lang.Long - lunghezza
### getName() {#getName--}
```
public final String getName()
```


Il nome del file originale.

**Returns:**
java.lang.String - il nome del file originale
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Salva l'archivio lzma nel file di destinazione fornito.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lzma\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | java.io.OutputStream | flusso di destinazione |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Salva l'archivio lzma nel file di destinazione fornito.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.lzma\");
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

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.io.File | il file, che verrà aperto come stream di input |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Imposta il contenuto da comprimere all'interno dell'archivio.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save(\"archive.lzma\");
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

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourcePath | java.lang.String | percorso del file, che verrà aperto come flusso di input |

