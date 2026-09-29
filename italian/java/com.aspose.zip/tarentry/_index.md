---
title: "TarEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno di un archivio tar."
type: docs
weight: 126
url: /it/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno di un archivio tar.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getModificationTime()](#getModificationTime--) | Ottiene l'ora di modifica del file o della directory. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [getUncompressedSize()](#getUncompressedSize--) | Restituisce la dimensione di un file originale. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se la voce rappresenta una directory. |
| [open()](#open--) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome della voce all'interno dell'archivio. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

Estrai una voce dell'archivio tar.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto |

**Returns:**
java.io.File - le informazioni del file estratto.
### getLength() {#getLength--}
```
public final Long getLength()
```


Ottiene la lunghezza della voce in byte.

**Returns:**
java.lang.Long - la lunghezza della voce in byte
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Ottiene l'ora di modifica del file o della directory.

**Returns:**
java.util.Date - l'ora di modifica del file o della directory.
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome della voce all'interno dell'archivio.

**Returns:**
java.lang.String - il nome della voce all'interno dell'archivio
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Restituisce la dimensione di un file originale.

Ha lo stesso valore di `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - la dimensione di un file originale.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Ottiene un valore che indica se la voce rappresenta una directory.

**Returns:**
boolean - un valore che indica se la voce rappresenta una directory
### open() {#open--}
```
public final InputStream open()
```


Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce.


Utilizzo:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

