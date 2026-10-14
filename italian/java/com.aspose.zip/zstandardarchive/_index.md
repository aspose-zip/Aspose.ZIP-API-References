---
title: "ZstandardArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio Zstandard."
type: docs
weight: 156
url: /it/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio Zstandard. Usala per comporre archivi Zstandard.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparata per la compressione. |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparata per la decompressione. |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparata per la decompressione. |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae l'archivio nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae l'archivio nel file specificato dal percorso. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae il contenuto dell'archivio nella directory fornita. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio zstandard. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [open()](#open--) | Apre l'archivio per l'estrazione e fornisce uno stream con il contenuto dell'archivio. |
| [save(File destination)](#save-java.io.File-) | Salva l'archivio nel file di destinazione fornito. |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | Salva l'archivio nel file di destinazione fornito. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Salva l'archivio nello stream fornito. |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | Salva l'archivio nello stream fornito. |
| [save(String destinationFileName)](#save-java.lang.String-) | Salva l'archivio nel file di destinazione fornito. |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | Salva l'archivio nel file di destinazione fornito. |
| [setSource(File file)](#setSource-java.io.File-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(String path)](#setSource-java.lang.String-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparata per la compressione.

Il seguente esempio mostra come comprimere un file.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource("data.bin");
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

Questo costruttore non decomprime. Vedi il metodo [open()](../../com.aspose.zip/zstandardarchive\\#open--) per la decompressione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la sorgente dell'archivio |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparata per la decompressione.

Apri un archivio da uno stream e estrailo in un `ByteArrayOutputStream`

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

Questo costruttore non decomprime. Vedi il metodo [open()](../../com.aspose.zip/zstandardarchive\\#open--) per la decompressione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


Inizializza una nuova istanza della classe [ZstandardArchive](../../com.aspose.zip/zstandardarchive).

Apri un archivio da file tramite percorso e estrailo in un `ByteArrayOutputStream`

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | stream di destinazione. Deve essere scrivibile |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae l'archivio nel file specificato dal percorso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto |

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


Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio zstandard.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio zstandard
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


Ottiene la lunghezza della voce in byte.

**Returns:**
java.lang.Long - la lunghezza della voce in byte
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome della voce all'interno dell'archivio.

**Returns:**
java.lang.String - il nome della voce all'interno dell'archivio
### open() {#open--}
```
public final InputStream open()
```


Apre l'archivio per l'estrazione e fornisce uno stream con il contenuto dell'archivio.

Estrae l'archivio e copia il contenuto estratto nello stream del file.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.File | il file che sarà aperto come stream di destinazione |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


Salva l'archivio nel file di destinazione fornito.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| outputStream | java.io.OutputStream | lo stream di destinazione |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


Salva l'archivio nello stream fornito.

Scrivi i dati compressi nello stream di risposta http.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


Salva l'archivio nel file di destinazione fornito.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.io.File | il riferimento a un file da comprimere |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Imposta il contenuto da comprimere all'interno dell'archivio.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | percorso del file da comprimere |

