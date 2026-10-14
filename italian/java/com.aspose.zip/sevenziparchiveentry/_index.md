---
title: "SevenZipArchiveEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno di un archivio 7z."
type: docs
weight: 105
url: /it/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno di un archivio 7z.

Esegui il cast di un'istanza di [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) a [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) per determinare se l'entry è crittografato o meno.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getCompressedSize()](#getCompressedSize--) | Restituisce la dimensione del file compresso. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Ottiene un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
| [getCompressionSettings()](#getCompressionSettings--) | Ottiene le impostazioni per la compressione o la decompressione. |
| [getLength()](#getLength--) | Ottiene la lunghezza. |
| [getModificationTime()](#getModificationTime--) | Restituisce la data e l'ora dell'ultima modifica. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [getUncompressedSize()](#getUncompressedSize--) | Ottiene la dimensione del file originale. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se la voce rappresenta una directory. |
| [open()](#open--) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |
| [open(String password)](#open-java.lang.String-) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Imposta un evento che viene sollevato quando una porzione di stream grezzo è compressa. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

Estrai una voce dell'archivio zip con password.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | stream di destinazione. Deve essere scrivibile |
| password | java.lang.String | password opzionale per la decrittazione |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae la voce nel file system utilizzando il percorso fornito.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract("data.bin");
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

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto |
| password | java.lang.String | password opzionale per la decrittazione |

**Returns:**
java.io.File - le informazioni del file estratto.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Restituisce la dimensione del file compresso.

**Returns:**
long - la dimensione del file compresso
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

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
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


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Leggi dal flusso per ottenere il contenuto originale del file. Vedi la sezione esempi.

**Returns:**
java.io.InputStream - il flusso che rappresenta il contenuto della voce
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce.

Utilizzo:

```

``````

SevenZipArchive archive = new SevenZipArchive("archive.7z");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
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

Il mittente dell'evento è un'istanza di [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry).

Non viene invocato in modalità solida e in modalità multithread per le voci LZMA2.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento che viene sollevato quando una porzione di stream grezzo è compressa |

