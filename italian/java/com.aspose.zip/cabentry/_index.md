---
title: "CabEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno di un archivio cab."
type: docs
weight: 46
url: /it/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno di un archivio cab.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getModificationTime()](#getModificationTime--) | Restituisce la data e l'ora dell'ultima modifica. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [open()](#open--) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa dell'istanza della classe [CabEntry](../../com.aspose.zip/cabentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

Estrai una voce dell'archivio CAB.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
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

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto |

**Returns:**
java.io.File - le informazioni sul file di un file composto
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


Restituisce la data e l'ora dell'ultima modifica.

**Returns:**
java.util.Date - data e ora dell'ultima modifica.
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome della voce all'interno dell'archivio.

**Returns:**
java.lang.String - il nome della voce all'interno dell'archivio
### open() {#open--}
```
public final InputStream open()
```


Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce.

Utilizzo:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
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


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
