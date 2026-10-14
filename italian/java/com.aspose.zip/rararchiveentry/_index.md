---
title: "RarArchiveEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno dell'archivio."
type: docs
weight: 98
url: /it/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno dell'archivio.

Esegui il cast di un'istanza di [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) a [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) per determinare se l'entry è crittografato o meno.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getCompressedSize()](#getCompressedSize--) | Ottiene la dimensione del file compresso. |
| [getCreationTime()](#getCreationTime--) | Ottiene la data e l'ora di creazione. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Ottiene un evento che viene sollevato quando una parte del flusso grezzo viene estratta. |
| [getLastAccessTime()](#getLastAccessTime--) | Ottiene la data e l'ora dell'ultimo accesso. |
| [getLength()](#getLength--) | Ottiene la lunghezza. |
| [getModificationTime()](#getModificationTime--) | Restituisce la data e l'ora dell'ultima modifica. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [getUncompressedSize()](#getUncompressedSize--) | Ottiene la dimensione del file originale. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se la voce rappresenta una directory. |
| [open()](#open--) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso. |
| [open(String password)](#open-java.lang.String-) | Apre la voce per l'estrazione e fornisce un flusso con il contenuto della voce decompresso. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Imposta un evento che viene sollevato quando una parte del flusso grezzo viene estratta. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.


Estrai una voce dell'archivio rar con password.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
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


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
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


Estrai due voci dell'archivio rar.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
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
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Ottiene la dimensione del file compresso.

**Returns:**
long - la dimensione del file compresso
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Ottiene la data e l'ora di creazione.

**Returns:**
java.util.Date - data e ora di creazione.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Ottiene un evento che viene sollevato quando una parte del flusso grezzo viene estratta.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
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

Leggi dal flusso per ottenere il contenuto originale del file. Vedi la sezione esempi.

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
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Il mittente dell'evento è un'istanza di [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento che viene sollevato quando una porzione di stream grezzo è estratta. |

