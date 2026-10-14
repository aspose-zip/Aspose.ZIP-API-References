---
title: "CpioEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno di un archivio cpio."
type: docs
weight: 58
url: /it/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno di un archivio cpio.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Ottiene l'ora dell'ultima scrittura. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [getParent()](#getParent--) | Ottiene l'archivio a cui appartiene la voce. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se la voce rappresenta una directory. |
| [open()](#open--) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa dell'istanza della classe [CpioEntry](../../com.aspose.zip/cpioentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

Estrai una voce dall'archivio cpio.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto |

**Returns:**
java.io.File - le informazioni del file estratto.
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Ottiene l'ora dell'ultima scrittura.

**Returns:**
java.util.Date - l'ora dell'ultima scrittura
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
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Ottiene l'archivio a cui appartiene la voce.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Ottiene un valore che indica se la voce rappresenta una directory.

**Returns:**
boolean - un valore che indica se la voce rappresenta una directory.
### open() {#open--}
```
public final InputStream open()
```


Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce.

Utilizzo:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
