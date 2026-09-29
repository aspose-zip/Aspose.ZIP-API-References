---
title: "IsoArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un archivio ISO ISO 9660."
type: docs
weight: 71
url: /it/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Rappresenta un archivio ISO (ISO 9660).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e crea un archivio ISO vuoto per aggiungere nuovi file e directory. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Aggiunge una directory all'immagine ISO. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Aggiunge un file all'immagine ISO. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Aggiunge un file all'immagine ISO. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Aggiunge un file all'immagine ISO. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutte le voci nella directory specificata. |
| [getEntries()](#getEntries--) | Ottiene le voci di tipo [IsoEntry](../../com.aspose.zip/isoentry) che costituiscono l'archivio. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Salva l'immagine ISO nello stream specificato. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Salva l'immagine ISO nello stream specificato. |
| [save(String path)](#save-java.lang.String-) | Salva l'immagine ISO nel percorso specificato. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Salva l'immagine ISO nel percorso specificato. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e crea un archivio ISO vuoto per aggiungere nuovi file e directory.

Il seguente esempio mostra come creare un nuovo archivio ISO vuoto e aggiungere file ad esso:

```

``````

// Crea un nuovo archivio ISO vuoto
try (IsoArchive isoArchive = new IsoArchive()) {
// Aggiungi file all'archivio ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Salva l'archivio ISO in un file
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Questo costruttore non estrae alcuna voce.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la sorgente dell'archivio |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Questo costruttore non estrae alcuna voce.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [IsoArchive](../../com.aspose.zip/isoarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | java.lang.String | la directory in cui estrarre le voci |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Ottiene le voci di tipo [IsoEntry](../../com.aspose.zip/isoentry) che costituiscono l'archivio.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - voci di tipo [IsoEntry](../../com.aspose.zip/isoentry) che costituiscono l'archivio iso
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio iso
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Ottiene il formato dell'archivio.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Salva l'immagine ISO nello stream specificato.

Il seguente esempio mostra come salvare un archivio ISO in uno stream di memoria:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Crea un nuovo archivio ISO vuoto
try (IsoArchive isoArchive = new IsoArchive()) {
// Aggiungi file all'archivio ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Salva l'archivio ISO in uno stream di memoria
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.OutputStream | lo stream in cui l'immagine ISO verrà salvata |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | le opzioni con cui salvare l'archivio ISO |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Salva l'immagine ISO nel percorso specificato.

Il seguente esempio mostra come salvare un archivio ISO in un file:

```

``````

// Crea un nuovo archivio ISO vuoto
try (IsoArchive isoArchive = new IsoArchive()) {
// Aggiungi file all'archivio ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Salva l'archivio ISO in un file
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso in cui l'immagine ISO verrà salvata |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | le opzioni con cui salvare l'archivio ISO |

