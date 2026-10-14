---
title: "ZArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio Z compress."
type: docs
weight: 153
url: /it/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio Z (compress). Usala per comporre o estrarre archivi Z.

Vedi [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ZArchive()](#ZArchive--) | Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la compressione. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Estrae l'archivio Z in un file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae l'archivio Z in uno stream. |
| [extract(String path)](#extract-java.lang.String-) | Estrae l'archivio Z in un file per percorso. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae il contenuto dell'archivio nella directory fornita. |
| [getFileEntries()](#getFileEntries--) | Restituisce le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio Z. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Salva l'archivio Z nello stream fornito. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Salva l'archivio Z nello stream fornito. |
| [save(String destinationFileName)](#save-java.lang.String-) | Salva l'archivio Z nel file di destinazione fornito. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Salva l'archivio Z nel file di destinazione fornito. |
| [setSource(File file)](#setSource-java.io.File-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Imposta il contenuto da comprimere all'interno dell'archivio. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la compressione.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | le opzioni con cui caricare l'archivio |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso alla sorgente dell'archivio |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [ZArchive](../../com.aspose.zip/zarchive) preparata per la decompressione.

Questo costruttore non decomprime. Vedi il metodo [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso alla sorgente dell'archivio |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | le opzioni con cui caricare l'archivio |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Estrae l'archivio Z in un file.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
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


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


Estrae l'archivio Z in un file per percorso.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | java.io.OutputStream | lo stream di destinazione |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Salva l'archivio Z nello stream fornito.

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource("data.bin");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Salva l'archivio Z nel file di destinazione fornito.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| file | java.io.File | le informazioni del file che saranno aperte come stream di input |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Imposta il contenuto da comprimere all'interno dell'archivio.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourcePath | java.lang.String | il percorso del file che sarà aperto come stream di input |

