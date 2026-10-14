---
title: "XzArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio xz."
type: docs
weight: 146
url: /it/java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio xz. Usala per creare ed estrarre archivi xz.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [XzArchive()](#XzArchive--) | Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) e compone l'archivio in formato xz. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) e compone l'archivio in formato xz. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione. |
| [XzArchive(InputStream source, XzLoadOptions options)](#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-) | Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione. |
| [XzArchive(String path, XzLoadOptions options)](#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-) | Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Estrae l'archivio xz in un file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae l'archivio xz in uno stream. |
| [extract(String path)](#extract-java.lang.String-) | Estrae l'archivio xz in un file per percorso. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae il contenuto dell'archivio nella directory fornita. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio xz. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [getUncompressedSize()](#getUncompressedSize--) | Ottiene la dimensione non compressa dei dati del file in byte. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Salva l'archivio xz nello stream fornito. |
| [save(String destinationFileName)](#save-java.lang.String-) | Salva l'archivio xz nel file di destinazione fornito. |
| [setSource(File file)](#setSource-java.io.File-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) e compone l'archivio in formato xz.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) e compone l'archivio in formato xz.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | insieme di impostazioni specifiche per l'archivio xz: dimensione del dizionario, dimensione del blocco, tipo di controllo |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |

### XzArchive(InputStream source, XzLoadOptions options) {#XzArchive-java.io.InputStream-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(InputStream source, XzLoadOptions options)
```


Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) | Opzioni per caricare l'archivio. |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | percorso alla sorgente dell'archivio |

### XzArchive(String path, XzLoadOptions options) {#XzArchive-java.lang.String-com.aspose.zip.XzLoadOptions-}
```
public XzArchive(String path, XzLoadOptions options)
```


Inizializza una nuova istanza della classe [XzArchive](../../com.aspose.zip/xzarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | percorso alla sorgente dell'archivio |
| options | [XzLoadOptions](../../com.aspose.zip/xzloadoptions) |  |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Estrae l'archivio xz in un file.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | stream per memorizzare i dati decompressi |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae l'archivio xz in un file per percorso.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | java.io.OutputStream | flusso di destinazione |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Salva l'archivio xz nel file di destinazione fornito.

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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.io.File | file, che sarà aperto come stream di input |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Imposta il contenuto da comprimere all'interno dell'archivio.

```

``````

try (XzArchive archive = new XzArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.xz");
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourcePath | java.lang.String | percorso al file che sarà aperto come stream di input |

