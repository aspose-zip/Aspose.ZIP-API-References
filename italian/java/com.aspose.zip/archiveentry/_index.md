---
title: "ArchiveEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno dell'archivio."
type: docs
weight: 27
url: /it/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno dell'archivio.

Esegue il cast di un'istanza di [ArchiveEntry](../../com.aspose.zip/archiveentry) a [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) per determinare se la voce è crittata o meno.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getComment()](#getComment--) | Ottiene il commento della voce all'interno dell'archivio. |
| [getCompressedSize()](#getCompressedSize--) | Ottiene la dimensione del file compresso. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
| [getCompressionSettings()](#getCompressionSettings--) | Ottiene le impostazioni per la compressione o la decompressione. |
| [getDataSource()](#getDataSource--) | Origine della voce se la voce è stata aggiunta all'archivio, non estratta. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Ottiene un evento che viene sollevato quando una parte del flusso grezzo viene estratta. |
| [getLength()](#getLength--) | Ottiene la lunghezza. |
| [getModificationTime()](#getModificationTime--) | Restituisce la data e l'ora dell'ultima modifica. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [getUncompressedSize()](#getUncompressedSize--) | Ottiene la dimensione del file originale. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se la voce rappresenta una directory. |
| [open()](#open--) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso. |
| [open(String password)](#open-java.lang.String-) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Imposta un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Imposta un evento che viene sollevato quando una parte del flusso grezzo viene estratta. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Imposta la data e l'ora dell'ultima modifica. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

Estrai una voce dell'archivio zip con password.

```

``````

try (FileInputStream zipFile = new FileInputStream(\"archive.zip\")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(outputStream, \"p@s$\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | Flusso di destinazione. Deve essere scrivibile. |
| password | java.lang.String | Password opzionale per la decrittazione. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae la voce nel file system utilizzando il percorso fornito.

Estrai due voci dell'archivio ZIP, ognuna con la propria password

```

``````

try (FileInputStream zipFile = new FileInputStream(\"archive.zip\")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(\"first.bin\", \"first_pass\");
archive.getEntries().get(1).extract(\"second.bin\", \"second_pass\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | Il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto. |
| password | java.lang.String | Password opzionale per la decrittazione. |

**Returns:**
java.io.File - le informazioni del file estratto.
### getComment() {#getComment--}
```
public final String getComment()
```


Ottiene il commento della voce all'interno dell'archivio.

**Returns:**
java.lang.String - commento della voce all'interno dell'archivio
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Ottiene la dimensione del file compresso.

**Returns:**
long - dimensione del file compresso
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

In questo esempio il gestore di eventi è usato per l'annullamento dopo i primi cento MB dell'entry sono stati estratti.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

Leggi dallo stream per ottenere il contenuto originale del file.

**Returns:**
java.io.InputStream - Lo stream che rappresenta il contenuto dell'entry.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso.


Utilizzo:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

Il mittente dell'evento è un'istanza di [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento che viene sollevato quando una porzione di stream grezzo è compressa |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Imposta un evento che viene sollevato quando una parte del flusso grezzo viene estratta.

In questo esempio il gestore di eventi è usato per calcolare la quota della dimensione elaborata in percentuale.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Il mittente dell'evento è un'istanza di [ArchiveEntry](../../com.aspose.zip/archiveentry). È possibile annullare l'estrazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | un evento che viene sollevato quando una porzione di stream grezzo è estratta. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Imposta la data e l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date | data e ora dell'ultima modifica |

