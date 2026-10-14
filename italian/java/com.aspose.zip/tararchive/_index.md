---
title: "TarArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio tar."
type: docs
weight: 125
url: /it/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio tar. Usala per comporre, estrarre o aggiornare archivi tar.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TarArchive()](#TarArchive--) | Inizializza una nuova istanza della classe [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [Archive](../../com.aspose.zip/archive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Inizializza una nuova istanza della classe [TarArchive](../../com.aspose.zip/tararchive) e compone un elenco di voci che può essere estratto dall'archivio. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Aggiunge all'archivio tutti i file e le directory ricorsivamente nella directory specificata. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Aggiunge all'archivio tutti i file e le directory ricorsivamente nella directory specificata. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Aggiunge all'archivio tutti i file e le directory ricorsivamente nella directory specificata. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Aggiunge all'archivio tutti i file e le directory ricorsivamente nella directory specificata. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crea una singola voce all'interno dell'archivio. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Rimuove la prima occorrenza di una voce specifica dall'elenco delle voci. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Rimuove la voce dall'elenco delle voci per indice. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file dell'archivio nella directory fornita. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Estrae l'archivio gzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Estrae l'archivio gzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Estrae l'archivio LZ4 fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Estrae l'archivio LZ4 fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Estrae l'archivio LZMA fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Estrae l'archivio LZMA fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Estrae l'archivio lzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Estrae l'archivio lzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Estrae l'archivio in formato xz fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Estrae l'archivio in formato xz fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Estrae l'archivio in formato Z fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Estrae l'archivio in formato Z fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Estrae l'archivio Zstandard fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Estrae l'archivio Zstandard fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti. |
| [getEntries()](#getEntries--) | Ottiene le voci di tipo [TarEntry](../../com.aspose.zip/tarentry) che costituiscono l'archivio. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio tar. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Salva l'archivio nello stream fornito. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream fornito. |
| [save(String destinationFileName)](#save-java.lang.String-) | Salva l'archivio nel file di destinazione fornito. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio nel file di destinazione fornito. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Salva l'archivio nello stream con compressione gzip. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream con compressione gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Salva l'archivio su file tramite percorso con compressione gzip. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio su file tramite percorso con compressione gzip. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Salva l'archivio nello stream con compressione LZ4. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream con compressione LZ4. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Salva l'archivio nel file specificato dal percorso con compressione LZ4. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio nel file specificato dal percorso con compressione LZ4. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Salva l'archivio nello stream con compressione LZMA. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream con compressione LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Salva l'archivio nel file specificato dal percorso con compressione lzma. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio nel file specificato dal percorso con compressione lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Salva l'archivio nello stream con compressione lzip. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream con compressione lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Salva l'archivio su file tramite percorso con compressione lzip. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio su file tramite percorso con compressione lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Salva l'archivio nello stream con compressione xz. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream con compressione xz. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Salva l'archivio nello stream con compressione xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Salva l'archivio su file tramite percorso con compressione xz. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio su file tramite percorso con compressione xz. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Salva l'archivio su file tramite percorso con compressione xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Salva l'archivio nello stream con compressione Z. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream con compressione Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Salva l'archivio su file tramite percorso con compressione Z. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio su file tramite percorso con compressione Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Salva l'archivio nello stream con compressione Zstandard. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Salva l'archivio nello stream con compressione Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Salva l'archivio su file tramite percorso con compressione Zstandard. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Salva l'archivio su file tramite percorso con compressione Zstandard. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Inizializza una nuova istanza della classe [TarArchive](../../com.aspose.zip/tararchive).

Il seguente esempio mostra come comprimere un file.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Questo costruttore non estrae alcuna voce. Vedi il metodo [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) per l'estrazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la sorgente dell'archivio |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Inizializza una nuova istanza della classe [TarArchive](../../com.aspose.zip/tararchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | java.io.File | directory da comprimere |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Aggiunge all'archivio tutti i file e le directory ricorsivamente nella directory specificata.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory da comprimere |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Aggiunge all'archivio tutti i file e le directory ricorsivamente nella directory specificata.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

Il nome della voce è impostato esclusivamente nel parametro `name`. Il nome del file fornito nel parametro `file` non influisce sul nome della voce.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | il nome della voce |
| file | java.io.File | i metadati del file o della cartella da comprimere |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Crea una singola voce all'interno dell'archivio.

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

Il nome della voce è impostato esclusivamente nel parametro `name`.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | il nome della voce |
| source | java.io.InputStream | il flusso di input per l'entry |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Crea una singola voce all'interno dell'archivio.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

Il nome della voce è impostato esclusivamente nel parametro `name`. Il nome del file fornito nel parametro `path` non influisce sul nome della voce.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | il nome della voce |
| path | java.lang.String | percorso del file da comprimere |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Crea una singola voce all'interno dell'archivio.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, \"data.bin\");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | la voce da rimuovere dall'elenco delle voci |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Rimuove la voce dall'elenco delle voci per indice.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Se la directory non esiste, verrà creata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | java.lang.String | il percorso della directory in cui posizionare i file estratti |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Estrae l'archivio gzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio gzip viene completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

Il flusso di estrazione GZip non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Estrae l'archivio gzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio gzip viene completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

Il flusso di estrazione GZip non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Estrae l'archivio LZ4 fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio LZ4 viene completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | source | java.io.InputStream | La sorgente dell'archivio. |

Il flusso di estrazione LZ4 non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Estrae l'archivio LZ4 fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio LZ4 viene completamente estratto all'interno di questo metodo, il suo contenuto è conservato internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | path | java.lang.String | Il percorso al file di archivio. |

Il flusso di estrazione LZ4 non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Estrae l'archivio LZMA fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio LZMA è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

Il flusso di estrazione LZMA non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Estrae l'archivio LZMA fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio LZMA è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

Il flusso di estrazione LZMA non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Estrae l'archivio lzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio lzip è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

Il flusso di estrazione Lzip non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Estrae l'archivio lzip fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio lzip è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

Il flusso di estrazione Lzip non è ricercabile per natura dell'algoritmo di compressione. L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Estrae l'archivio in formato xz fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio xz è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Estrae l'archivio in formato xz fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio xz è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

L'archivio Tar fornisce la possibilità di estrarre record arbitrari, quindi deve operare su un flusso ricercabile internamente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Estrae l'archivio in formato Z fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio Z è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Estrae l'archivio in formato Z fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio Z è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Estrae l'archivio Zstandard fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio Zstandard è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | java.io.InputStream | la sorgente dell'archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Estrae l'archivio Zstandard fornito e compone un [TarArchive](../../com.aspose.zip/tararchive) dai dati estratti.

Importante: l'archivio Zstandard è completamente estratto all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Ottiene le voci di tipo [TarEntry](../../com.aspose.zip/tarentry) che costituiscono l'archivio.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - voci di tipo [TarEntry](../../com.aspose.zip/tarentry) che costituiscono l'archivio
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio tar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio tar
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Ottiene il formato dell'archivio.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Salva l'archivio nello stream fornito.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | flusso di destinazione. |

`output` deve essere scrivibile |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Salva l'archivio nel file di destinazione fornito.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

È possibile salvare un archivio nello stesso percorso da cui è stato caricato. Tuttavia, ciò non è consigliato perché questo approccio utilizza la copia in un file temporaneo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Salva l'archivio nello stream con compressione gzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | flusso di destinazione. |

`output` deve essere scrivibile |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Salva l'archivio su file tramite percorso con compressione gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Salva l'archivio nello stream con compressione LZ4.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | java.io.OutputStream | Stream di destinazione. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Salva l'archivio nel file specificato dal percorso con compressione LZ4.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | Il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Salva l'archivio nello stream con compressione LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Importante: l'archivio tar è composto e poi compresso all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | flusso di destinazione. |

`output` deve essere scrivibile |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Salva l'archivio nel file specificato dal percorso con compressione lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Importante: l'archivio tar è composto e poi compresso all'interno di questo metodo, il suo contenuto è mantenuto internamente. Attenzione al consumo di memoria.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Salva l'archivio nello stream con compressione lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | flusso di destinazione. |

`output` deve essere scrivibile |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Salva l'archivio su file tramite percorso con compressione lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Salva l'archivio nello stream con compressione xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | flusso di destinazione. |

`output`Il flusso deve essere scrivibile |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Salva l'archivio nello stream con compressione xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Salva l'archivio su file tramite percorso con compressione xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | insieme di impostazioni specifiche per l'archivio xz: dimensione del dizionario, dimensione del blocco, tipo di controllo |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Salva l'archivio nello stream con compressione Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| output | java.io.OutputStream | lo stream di destinazione |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Salva l'archivio su file tramite percorso con compressione Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Salva l'archivio nello stream con compressione Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | flusso di destinazione. |

`output` deve essere scrivibile |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Salva l'archivio su file tramite percorso con compressione Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso dell'archivio da creare. Se il nome file specificato punta a un file esistente, verrà sovrascritto |
| format | [TarFormat](../../com.aspose.zip/tarformat) | definisce il formato dell'intestazione tar. Il valore null verrà trattato come USTar quando possibile |

