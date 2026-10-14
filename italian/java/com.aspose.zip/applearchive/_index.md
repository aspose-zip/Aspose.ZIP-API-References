---
title: "AppleArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file Apple Archive .aar."
type: docs
weight: 16
url: /it/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Questa classe rappresenta un file Apple Archive (.aar). Usala per creare file Apple Archive.

Apple e Apple Archive sono marchi registrati di Apple Inc.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) con le impostazioni utilizzate per le voci composte. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) con le impostazioni utilizzate per le voci composte. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory specificata. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory specificata. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crea una singola voce all'interno dell'archivio. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crea una singola voce all'interno dell'archivio. |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file dell'archivio nella directory fornita. |
| [getEntries()](#getEntries--) | Ottiene le voci che costituiscono l'archivio. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Ottiene le impostazioni utilizzate per le voci appena composte. |
| [isSolid()](#isSolid--) | Restituisce un valore che indica se l'archivio utilizza la compressione solida. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Salva l'archivio nello stream fornito. |
| [save(String destinationFileName)](#save-java.lang.String-) | Salva l'archivio nel file di destinazione fornito. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) con le impostazioni utilizzate per le voci composte.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) con le impostazioni utilizzate per le voci composte.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Impostazioni utilizzate durante la creazione di un nuovo Apple Archive. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | La sorgente dell'archivio. |

Questo costruttore non decomprime alcuna voce. Vedi i metodi [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) e [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) per la decompressione. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | java.io.InputStream | La sorgente dell'archivio. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opzioni per caricare l'archivio esistente. |

Questo costruttore non decomprime alcuna voce. Vedi i metodi [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) e [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) per la decompressione. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | path | java.lang.String | Il percorso completo o relativo al file dell'archivio. |

Questo costruttore non decomprime alcuna voce. Vedi i metodi [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) e [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) per la decompressione. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [AppleArchive](../../com.aspose.zip/applearchive) e compone un elenco di voci che può essere estratto dall'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | Il percorso completo o relativo al file dell'archivio. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opzioni per caricare l'archivio esistente. |

Questo costruttore non decomprime alcuna voce. Vedi i metodi [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) e [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) per la decompressione. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | java.io.File | Directory da comprimere. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Aggiunge all'archivio tutti i file e le directory in modo ricorsivo nella directory specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| directory | java.io.File | Directory da comprimere. |
| includeRootDirectory | boolean | Indica se includere o meno la directory radice stessa. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Crea una singola voce all'interno dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | Il nome della voce. |
| fileInfo | java.io.File | I metadati del file da comprimere. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Crea una singola voce all'interno dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | Il nome della voce. |
| fileInfo | java.io.File | I metadati del file da comprimere. |
| openImmediately | boolean | True, se si apre il file immediatamente, altrimenti il file viene aperto al salvataggio dell'archivio. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Crea una singola voce all'interno dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | Il nome della voce. |
| source | java.io.InputStream | Il flusso di input per la voce. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Crea una singola voce all'interno dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | Il nome della voce. |
| path | java.lang.String | Il percorso del file da comprimere. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Crea una singola voce all'interno dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String | Il nome della voce. |
| path | java.lang.String | Il percorso del file da comprimere. |
| openImmediately | boolean | True, se si apre il file immediatamente, altrimenti il file viene aperto al salvataggio dell'archivio. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae tutti i file dell'archivio nella directory fornita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Il percorso della directory in cui posizionare i file estratti. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Ottiene le voci che costituiscono l'archivio.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - voci che costituiscono l'archivio.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Ottiene il formato dell'archivio.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Ottiene le impostazioni utilizzate per le voci appena composte.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Restituisce un valore che indica se l'archivio utilizza la compressione solida. In modalità solida, tutti i dati delle voci sono compressi come un unico flusso e l'estrazione di singole voci non è disponibile. Usa invece [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--).

**Returns:**
boolean - un valore che indica se l'archivio utilizza la compressione solida.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Salva l'archivio nello stream fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | Stream di destinazione. |

`output` deve essere scrivibile. Alcune impostazioni di compressione, come LZ4, richiedono anche un flusso ricercabile. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Salva l'archivio nel file di destinazione fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationFileName | java.lang.String | Il percorso dell'archivio da creare. |

